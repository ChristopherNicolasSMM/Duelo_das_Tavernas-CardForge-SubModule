# Duelo das Tavernas — Fermento & Honra

Collection consolidada a partir do GDD v2.1 + manual oficial + arte já produzida.
Este README documenta o que foi feito e as decisões tomadas para integrar tudo
ao CardForge v2.

## O que mudou no repositório

- **`collections/duelo_das_tavernas` (antigo) → renomeado para `collections/generico_rpg_001`.**
  Esse schema (Cervejaria/Personagem/Item/Local/Habilidade com stats de RPG genérico)
  era um conceito anterior/mais genérico, diferente do jogo fechado no GDD v2.1.
  Os 5 templates e os dados de exemplo foram preservados sem alteração, só o nome mudou.
- **`collections/duelo_das_tavernas` (novo)**: criado do zero para representar o jogo real
  ("Fermento & Honra — O Duelo das Tavernas"), com os dados das 180 cartas + 6 decks/personagens.

## Estrutura de dados (`data.json`)

Uma única tabela (186 linhas), diferenciada pela coluna `tipo_carta`:

| tipo_carta | Linhas | Template indicado |
|---|---|---|
| `Carta de Jogo` | 180 (30 × 6 decks) | **Duelo - Carta de Jogo** |
| `Personagem` | 6 (um por deck) | **Duelo - Personagem** |

Colunas principais: `name`, `deck`, `categoria` (Ataque/Defesa/Cura/Habilidade/Especial),
`nivel` (Baixo/Médio/Alto), `tipo_display` (rótulo pronto pra carta, ex: "ATAQUE · Baixo"),
`efeito` (texto pronto pra render), `efeito_original` (texto com a notação 🛡️ do GDD,
só pra referência/planilha), `ataque`/`defesa`/`cura` (valores numéricos), `art`
(nome do arquivo em `assets/library`), `image_prompt` (prompt de ilustração por carta).

**⚠️ Renomeei a coluna `Tipo` → `categoria`.** O importador de CSV/XLSX do CardForge
(`core/data/reader.py`) tem um alias que renomeia automaticamente uma coluna chamada
`tipo` para `type_line` (herança do schema Magic). Se eu tivesse mantido `tipo`, um
reimport futuro via Dados → Upload silenciosamente trocaria o nome da coluna. `categoria`
não colide com nenhum alias.

## Templates

- **`Duelo - Carta de Jogo`** (novo, derivado de `Duelo - Habilidade`): usado pelas 180
  cartas de jogo. Testei o render de verdade (motor PIL do próprio CardForge) e ajustei:
  - Adicionei uma linha para o nome do **deck** abaixo do nome da carta.
  - O campo de subtítulo agora mostra `tipo_display` (tipo + nível).
  - A caixa de efeito ficou mais alta (~16mm) pra acomodar textos até 255 caracteres.
  - **Troquei a fonte do nome da carta de `Rye-Regular` para `Mplantin` (bold).** A fonte
    decorativa Rye rendeva alguns acentos (`ção`, `ã`) como um glifo quebrado/tofu em
    certos nomes (ex: "Regeneração Sombria"). Mplantin é a mesma fonte já usada no corpo
    do texto e renderiza todos os nomes corretamente — testei ~10 nomes com acentuação
    pesada depois da troca.
  - Notação `🛡️×N` do CSV vira `Absorve N` no campo `efeito` usado pelo template (a fonte
    não tem esse emoji). O texto original com o símbolo fica em `efeito_original`.
  - Adicionei um ícone por tipo de carta (espadas/escudo/coração/pergaminho/chama, de
    `assets/icons_png/`) no lugar da estrela genérica que estava fixa no template —
    campo `icone_tipo`, calculado a partir de `categoria`.
- **`Duelo - Personagem`** (reaproveitado como estava): usado pelos 6 decks/heróis.
  Mapeamento: `nivel` ← Dificuldade (Iniciante/Intermediário/Avançado), `classe` ←
  Arquétipo · Estilo Cervejeiro, `descricao` ← Habilidade Passiva (nome + texto),
  `lore` ← trecho narrativo do GDD (não usado por nenhuma layer ainda, disponível se
  quiser adicionar). Os campos `hp`/`atk`/`def` do template ficam em branco — o GDD não
  define esses stats pros decks-personagem; dá pra reaproveitar depois se fizer sentido.
- **`Duelo - Padrão (Cervejaria)`**: trazido como estava, não usado ainda. Fica disponível
  caso queira gerar cartas de rótulo real (ABV/IBU/EBC) a partir dos dados do projeto
  Rótulos Valirian.
- **Item / Local**: não recriados nesta collection — não existem no GDD v2.1 atual.

## Arte já disponível

Copiada para `assets/library/` (resolvida automaticamente pelo motor de render — ver
`_resolve_asset_path` em `core/render/preview_renderer.py`):

- 14 ilustrações de carta do deck **Pacto das Sombras** (já vinculadas na coluna `art`
  das respectivas linhas em `data.json`)
- 5 artes-herói extras do Pacto das Sombras (`pacto_das_sombras_hero_01..05.jpg`) —
  a primeira já está vinculada à linha `Personagem` do deck
- Capa do manual e um verso de carta alternativo em `assets/box_art/` (não usados por
  nenhum template ainda — o `back.png` atual dos templates já é um verso "dragão +
  VALIRIAN" consistente com o GDD, deixei como está)

**Faltam ilustrações para ~150 cartas** (os outros 5 decks). A fila completa de prompts
está em `docs/Duelo_das_Tavernas_Dados_e_Prompts.xlsx`, aba "Prompts de Imagem",
marcando o que já tem arte e o que falta.

## Arquivos em `docs/`

- **`manual/Valirian_Manual_Oficial.html`** — manual oficial (13 seções: regras, os 6
  personagens, modos de jogo, FAQ, glossário). Revisei contra o GDD v2.1 (D20 da
  Tempestade de Trigo, 25 Pints no modo Duelo, etc.) — está consistente e completo,
  não precisou de correção de conteúdo.
- **`gdd/Valirian_GDD_v2.1.md`** — Game Design Document, fonte de verdade para regras,
  lore e direção visual.
- **`Duelo_das_Tavernas_Dados_e_Prompts.xlsx`** — 9 abas: `Import_CardForge` (espelha
  `data.json` 1:1, pronta pra reimportar via Dados → Upload se quiser editar fora do
  app), uma aba por deck (leitura humana, colorida por tipo de carta), `Personagens`,
  e `Prompts de Imagem` (fila de ilustração).

## QA — validação em lote

Rodei o motor de render de verdade (não só inspeção visual) nas 186 linhas de
`data.json`: 186/186 renderizam sem erro, nenhum texto de efeito estoura a caixa
(máx. 5 linhas cabem, o texto mais longo do dataset não passa disso), e conferi
largura de texto pra nome/deck/tipo_display/classe contra a largura das caixas —
só um nome ("Escudo da Irmandade (Def)") passa por ~1px, imperceptível.

## Pendências / próximos passos

1. Gerar as ~150 ilustrações restantes (prompts prontos na planilha)
2. Decidir se quer usar o template "Padrão (Cervejaria)" pros rótulos reais
3. Ajustes finos de posição continuam possíveis no editor visual do CardForge


## Filtro por template (_template)

Como a coleção mistura dois templates no mesmo `data.json` (Carta de Jogo e
Personagem), adicionei a coluna reservada `_template` — já preenchida pras
186 linhas: `Duelo - Carta de Jogo` nas 180 cartas, `Duelo - Personagem` nos
6 decks-herói. Isso resolve um problema de arquitetura do CardForge: antes,
Gerar/Proxy aplicavam sempre um template a TODAS as linhas do dataset — ao
gerar com o template Personagem, as 180 cartas de combate também entravam.

Agora Gerar e Proxy filtram automaticamente: ao escolher um template, só as
linhas com `_template` igual a ele entram no lote. Linhas sem `_template`
(ou apontando pra um template que não existe) ficam de fora e avisam antes
de gerar — dá pra escolher "gerar mesmo assim" (ignora essas linhas) ou
voltar aos Dados e corrigir. Na tela de Dados, o campo aparece como dropdown
(botão "+ Coluna _template"), populado com os templates da coleção ativa —
evita erro de digitação.

Isso é código do próprio CardForge (não específico desta coleção) — vale
pra qualquer coleção com mais de um template.