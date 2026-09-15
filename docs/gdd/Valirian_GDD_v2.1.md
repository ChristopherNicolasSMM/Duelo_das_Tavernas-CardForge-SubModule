# FERMENTO & HONRA — O Duelo das Tavernas
## Game Design Document — Versão 2.1
### Cervejaria Valirian · Documento para Aprovação e Início de Desenvolvimento

---

## Sumário de Navegação

- [1. Visão Executiva](#1-visão-executiva)
- [2. Conceito e Posicionamento](#2-conceito-e-posicionamento)
- [3. Ficha do Produto](#3-ficha-do-produto)
- [4. Narrativa e Universo](#4-narrativa-e-universo)
- [5. Os Seis Personagens-Deck](#5-os-seis-personagens-deck)
- [6. Regras Completas do Jogo](#6-regras-completas-do-jogo)
- [7. Planilha de Decks — Arquivo Excel](#7-planilha-de-decks--arquivo-excel)
- [8. Comparação e Balanceamento](#8-comparação-e-balanceamento)
- [9. Modos de Jogo](#9-modos-de-jogo)
- [10. Direção Visual do Jogo](#10-direção-visual-do-jogo)
- [11. Componentes e Box Colecionador](#11-componentes-e-box-colecionador)
- [12. Estratégia de Lançamento](#12-estratégia-de-lançamento)
- [13. Roteiro de Desenvolvimento](#13-roteiro-de-desenvolvimento)
- [14. Prompt — Verso dos Cards](#14-prompt--verso-dos-cards)
- [15. Padrão de Efeitos — Regras de Texto](#15-padrão-de-efeitos--regras-de-texto)

---

## 1. Visão Executiva

**Fermento & Honra — O Duelo das Tavernas** é o card game oficial da Cervejaria Valirian.

O projeto transforma os rótulos do portfólio Valirian em personagens jogáveis de um card game competitivo. 
Cada deck representa uma cerveja com identidade, mecânica e narrativa únicas — alinhadas ao estilo cervejeiro e à arte do rótulo correspondente.

O jogo existe para **aprofundar o ecossistema da marca**, criando um produto colecionável que recompensa quem já conhece a Valirian e convida novos consumidores a descobrir o portfólio através do jogo.

> *"O jogo não existe sem a cerveja.*
> *O deck não existe sem o rótulo.*
> *Cada partida é uma celebração da experiência Valirian — nunca um produto separado."*

---

## 2. Conceito e Posicionamento

**Referência de mecânica:** Dungeon Mayhem (Wizards of the Coast) — card game ágil para 2–6 jogadores, cada personagem com deck único, habilidade passiva e mecânica própria e partidas de 15–30 minutos.

| Dimensão | Proposta |
|----------|----------|
| Para fãs da Valirian | Produto colecionável que aprofunda o vínculo com a marca |
| Para jogadores de card games | Jogo balanceado com identidade visual forte e história |
| Para o mercado artesanal | Experiência diferenciada além da garrafa |
| Para a marca Valirian | Expansão do ecossistema e visibilidade em eventos |

---

## 3. Ficha do Produto

| Atributo | Especificação |
|----------|---------------|
| Nome | Fermento & Honra — O Duelo das Tavernas |
| Tipo | Card Game Competitivo |
| Jogadores | 2 a 6 |
| Tempo por partida | 15–30 minutos |
| Faixa etária | 14+ |
| Total de cartas (box completo) | 180 cartas (6 decks × 30 cartas) |
| Linha | Edição Limitada / Colecionável |
| Licença | Produto oficial Cervejaria Valirian |

---

## 4. Narrativa e Universo

### Ambientação

O jogo se passa na **Taverna Valirian** — um lugar lendário onde aventureiros de todos os reinos se reúnem, a tradição sagrada da Taverna é o **Torneio do Barril**: todo lua cheia, cada cerveja do portfólio se manifesta como entidade personificada e disputa o título de **Mestre da Taverna**.

### Texto de abertura (manual)

> *"Nas terras de Valirian, diz-se que toda cerveja carrega uma alma.*

> *Não a alma do mestre cervejeiro — embora a dele esteja lá também — mas a alma de tudo o que ela representa: a floresta de onde vieram os lúpulos, a montanha que filtrou a água, o fogo que tostou o malte.*

>  *Quando a lua cheia banha o barril sagrado, essas almas ganham forma, e disputam, não com espadas, não com magias — com cartas, estratégia e a honra do seu estilo.*

>  *Que o melhor Mestre da Taverna vença. E que todos brindem ao final."*

---

## 5. Os Seis Personagens-Deck

Cada deck: **30 cartas**, **habilidade passiva única**, **mecânica central** coerente com o estilo cervejeiro.

### Distribuição de poder padrão (todos os decks)

| Nível | Quantidade | % | Descrição |
|-------|-----------|---|-----------|
| Baixo | 21 cartas | 70% | Efeitos padrão que mantêm o fluxo |
| Médio | 7 cartas | 23% | Efeitos condicionais ou com bônus |
| Alto | 2 cartas | 7% | Cartas "vire o jogo" com custo elevado |

---

### 5.1 Pacto das Sombras — Porter

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Porter |
| Arquétipo | Controlador / Sombrio |
| Estilo de Jogo | Controla o jogo, força descartes, brilha no fim da partida |
| Habilidade Passiva | *Manto das Trevas* — No início do turno, se você tiver ≤3 cartas na mão, compre 1 |
| Mecânica Central | Cartas que ganham força quando o jogador está em desvantagem |
| Dificuldade | Intermediário |

> *"Há magias que não deveriam ser invocadas. Há pactos que custam mais do que se imagina. O Pacto das Sombras é uma Porter encorpada e escura — como os segredos que ela guarda. Quem bebe, aceita o acordo."*

---

### 5.2 Sangue de Druida — Irish Red Ale

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Irish Red Ale |
| Arquétipo | Equilibrado / Conector |
| Estilo de Jogo | Conecta ações, ganha bônus por sequências, recompensa consistência |
| Habilidade Passiva | *Ciclo da Natureza* — Se você jogar ≥2 cartas no turno, cure 1 de vida |
| Mecânica Central | Combos e sequências que se potencializam |
| Dificuldade | Avançado |

> *"Nas florestas antigas, os druidas conhecem o fluxo da vida. Sangue de Druida celebra esse equilíbrio — terrosa, encorpada, com alma de madeira e raízes profundas."*

---

### 5.3 Elixir da Dríade — Session Juice IPA

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Session Juice IPA |
| Arquétipo | Curativo / Protetor |
| Estilo de Jogo | Cura aliados e si mesmo, protege, mecânicas de "presente" |
| Habilidade Passiva | *Essência da Floresta* — No final do turno, se você curou alguém, compre 1 carta |
| Mecânica Central | Curas que geram benefícios adicionais |
| Dificuldade | Iniciante–Intermediário |

> *"Dizem que dríades nascem das árvores mais antigas. O Elixir da Dríade carrega esse dom — suave, refrescante, com profundidade que só quem prova entende."*

---

### 5.4 Orvalho de Valirian — Witbier

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Witbier |
| Arquétipo | Ágil / Surpresa |
| Estilo de Jogo | Cartas baratas, ataques rápidos, alta mobilidade |
| Habilidade Passiva | *Primeiro Orvalho* — A 1ª carta jogada no turno não conta como ação principal |
| Mecânica Central | Muitas jogadas pequenas por turno; velocidade como vantagem |
| Dificuldade | Iniciante |

> *"Nas primeiras horas da manhã, quando o sol ainda não rompeu a névoa, o orvalho se forma. Quem prova esse líquido ao amanhecer ganha agilidade e clareza."*

---

### 5.5 Juramento do Aventureiro — Amber Ale

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Amber Ale |
| Arquétipo | Versátil / Adaptável |
| Estilo de Jogo | Deck com todos os tipos, bônus por "missões", adapta-se ao oponente |
| Habilidade Passiva | *Código do Aventureiro* — No início do jogo, escolha 1 tipo; cartas desse tipo têm +1 de efeito |
| Mecânica Central | Adaptação — o jogador define o foco e otimiza em torno dele |
| Dificuldade | Intermediário |

> *"Todo aventureiro sabe: o mundo não espera você se preparar. Juramento do Aventureiro é uma Amber Ale equilibrada, confiável, pronta para qualquer desafio."*

---

### 5.6 Tempestade de Trigo — Weiss

| Campo | Definição |
|-------|-----------|
| Estilo Cervejeiro | Weiss |
| Arquétipo | Explosivo / Imprevisível |
| Estilo de Jogo | Efeitos aleatórios, cartas poderosas com risco embutido |
| Habilidade Passiva | *Fúria dos Ventos* — Role D20 no início do turno: 1-10 = 1 dano próprio; 11-18 = compre 1; 19-20 = 3 dano em oponente + compre 1 |
| Mecânica Central | Aleatoriedade controlada — efeitos fortes com possibilidade de falha |
| Dificuldade | Intermediário |

> *"O trigo balança com o vento, mas quando a tempestade chega, até as montanhas tremem. Uma Weissbier imprevisível — refrescante como a brisa, com um trovão escondido."*

---

### Resumo rápido dos 6 decks

| Deck | Estilo | Arquétipo | Passiva | Dificuldade |
|------|--------|-----------|---------|-------------|
| Pacto das Sombras | Porter | Controlador | Compra se mão ≤3 | Intermediário |
| Sangue de Druida | Irish Red Ale | Conector | Cura 1 se jogar ≥2 cartas | Avançado |
| Elixir da Dríade | Session Juice IPA | Curativo | Compra 1 se curou no turno | Iniciante–Interm. |
| Orvalho de Valirian | Witbier | Ágil | Ação extra na 1ª carta | Iniciante |
| Juramento do Aventureiro | Amber Ale | Versátil | Escolhe tipo com +1 de efeito | Intermediário |
| Tempestade de Trigo | Weiss | Imprevisível | D20 no início do turno | Intermediário |

---

## 6. Regras Completas do Jogo

### 6.1 Objetivo e Preparação

**Objetivo:** Ser o último jogador com Pints de Glória acima de zero.

**Preparação:**
1. Cada jogador escolhe um deck e o embaralha
2. Cada jogador compra 5 cartas (mão inicial)
3. Todos começam com **20 Pints de Glória**
4. Determine a ordem: role o D20 Valirian — maior vai primeiro

> Variação 2 jogadores (Duelo): comece com **25 Pints de Glória** cada.

---

### 6.2 Estrutura do Turno

| Passo | Ação |
|-------|------|
| 1 — Comprar | Compre 1 carta do baralho e adicione à mão |
| 2 — Habilidade Passiva (pré) | Verifique se a condição foi atendida e resolva |
| 3 — Jogar Cartas | Jogue 1 carta (ação principal). Se mão estiver vazia, compre 2 e jogue 1 |
| 4 — Habilidade Passiva (pós) | Verifique habilidades de "final de turno" |
| 5 — Ajustar Mão | Descarte até ter ≤5 cartas; compre de volta até 5 |
| 6 — Passar a Vez | Próximo jogador inicia seu turno |

---

### 6.3 Tipos de Cartas

| Tipo | Cor da Borda | Símbolo | Função |
|------|--------------|---------|--------|
| Ataque | Âmbar #C8840A | 💥 | Causa dano (reduz Pints de Glória do alvo) |
| Defesa | Aço #6B8FA8 | 🛡️ | Absorve dano; permanece em campo até ser destruída |
| Cura | Floresta #1E3D1E | 🌿 | Recupera Pints de Glória (máx. 20) |
| Habilidade | Ouro #C8A028 | ✨ | Efeitos especiais (compra, descarte, manipulação) |
| Especial | Chama #D4520E | ⚡ | Versões poderosas com custo ou condição |

---

### 6.4 Níveis de Poder das Cartas

| Nível | % | Cartas | Descrição |
|-------|---|--------|-----------|
| Baixo | 70% | 21 | Efeitos padrão; mantêm o fluxo do jogo |
| Médio | 23% | 7 | Efeitos condicionais ou com bônus situacional |
| Alto | 7% | 2 | Cartas "vire o jogo"; risco ou custo elevado |

---

### 6.5 Regras Especiais

**Baralho vazio:** Embaralhe o descarte e continue.

**Mão cheia:** Não pode ter mais de 5 antes do Passo 5. Se forçado a comprar, descarte imediatamente até 5.

**Múltiplos alvos:** Dano de área é calculado e aplicado a cada alvo separadamente, considerando defesas individuais.

**Defesas com efeito ao serem destruídas:** O efeito ativa antes de ir para o descarte.

**Interação entre Defesas:** Com múltiplas ativas, o defensor escolhe qual absorve o dano primeiro.

---

### 6.6 Condição de Vitória

Último jogador com Pints de Glória > 0 é declarado **Mestre da Taverna Valirian**.

**Empate:** Se uma carta eliminar todos os jogadores restantes simultaneamente, todos brindam e preparam uma nova partida.

---

### 6.7 Habilidades Passivas — Referência

| Personagem | Habilidade | Verificação |
|------------|------------|-------------|
| Pacto das Sombras | Se mão ≤3 → compre 1 | Início do turno |
| Sangue de Druida | Se jogar ≥2 cartas → cure 1 | Final do turno |
| Elixir da Dríade | Se curou alguém → compre 1 | Final do turno |
| Orvalho de Valirian | 1ª carta não é ação principal | Ao jogar 1ª carta |
| Juramento do Aventureiro | 1 tipo de carta escolhido tem +1 de efeito | Configuração inicial |
| Tempestade de Trigo | Role D20: 1-10 dano próprio / 11-18 compra / 19-20 ataque+compra | Início do turno |

---

### 6.8 Glossário

| Termo | Definição |
|-------|-----------|
| Pints de Glória | Pontos de vida do jogador (máx. 20, ou 25 no Duelo) |
| Nocauteado | Jogador com 0 Pints de Glória — eliminado |
| Mestre da Taverna | Título do vencedor da partida |
| Pilha de Descarte | Onde cartas usadas são depositadas viradas para cima |
| Defesa Ativa | Carta de Defesa em campo aguardando absorver dano |
| Mão | Cartas que o jogador segura; máximo de 5 |
| Ação Principal | A carta obrigatória jogada por turno |

---

## 7. Planilha de Decks — Arquivo Excel

Os 6 decks completos (180 cartas) estão no arquivo **`Valirian_Fermento_Honra_Decks.xlsx`**, com uma aba por deck.

### Colunas da planilha

| Coluna | Conteúdo | Limite |
|--------|----------|--------|
| # | Número da carta (1–30) | — |
| Nome da Carta | Nome épico da carta | — |
| Tipo | Ataque / Defesa / Cura / Habilidade / Especial | — |
| Nível | Baixo / Médio / Alto | — |
| Efeito | Texto do efeito exibido na carta | **≤255 chars** (hard limit 300) |
| Ataque | Valor de dano (se aplicável) | — |
| Defesa | Valor de absorção (se aplicável) | — |
| Cura | Valor de cura (se aplicável) | — |
| Char Count | Contagem automática + flag de alerta | Auto |
| Descrição da Imagem | Prompt para geração de ilustração IA | ≤300 chars |

### Código de cores da planilha

| Cor da linha/coluna | Significado |
|--------------------|-------------|
| Borda âmbar (header deck) | Nome e subtítulo do deck |
| Fundo âmbar tênue (Tipo: Ataque) | Carta de ataque |
| Fundo azul tênue (Tipo: Defesa) | Carta de defesa |
| Fundo verde tênue (Tipo: Cura) | Carta de cura |
| Fundo dourado tênue (Tipo: Habilidade) | Carta de habilidade |
| Fundo laranja tênue (Tipo: Especial) | Carta especial |
| Texto vermelho (Char Count) | Efeito excede 240 chars — revisar |

---

## 8. Comparação e Balanceamento

### Resumo de arquétipos

| Deck | Arquétipo | Força Principal | Fraqueza Principal |
|------|-----------|-----------------|-------------------|
| Pacto das Sombras | Controlador | Controle de mão adversária, late game | Baixa cura |
| Sangue de Druida | Conector | Combos e cura constante | Vulnerável a controle de mão |
| Elixir da Dríade | Curativo | Cura em área e proteção | Baixo dano ofensivo |
| Orvalho de Valirian | Ágil | Múltiplas ações por turno | Baixo dano por carta |
| Juramento do Aventureiro | Versátil | Adaptação a qualquer situação | Depende de escolha inicial |
| Tempestade de Trigo | Imprevisível | Efeitos explosivos | Aleatoriedade pode prejudicar |

### Análise de matchup — Pacto das Sombras vs. Sangue de Druida

| Cenário | Análise |
|---------|---------|
| Sangue de Druida ataca | Precisa de ≥2 cartas/turno. Se Pacto forçar descartes com *Sussurros*, os combos são quebrados |
| Pacto das Sombras ataca | Força descartes e controla o ritmo. Druida precisa manter mão cheia — difícil sob pressão |
| Equilíbrio geral | Pacto controla, Druida comba. Quem impuser o ritmo primeiro tende a vencer |

---

## 9. Modos de Jogo

### 9.1 Duelo — 2 Jogadores
Clássico 1v1. Cada jogador começa com **25 Pints de Glória**. Primeiro a nocautear o oponente vence.

### 9.2 Batalha da Taverna — 3–4 Jogadores
Todos contra todos. **20 Pints de Glória** cada.
**Regra adicional — Favor da Taverna:** Ao ser nocauteado, dê 1 carta aleatória da mão a um sobrevivente à escolha.

### 9.3 Festa da Colheita — 5–6 Jogadores
Jogo rápido todos contra todos. **20 Pints** cada.
**Regra adicional — Recompensa do Caçador:** Ao nocautear um oponente, cure 2 Pints de Glória.

### 9.4 A Ira do Barril Amaldiçoado — Cooperativo (Expansão Futura)
Todos os jogadores contra um "Chefão" com deck especial. Vitória se o grupo sobreviver por 10 rodadas ou causar dano coletivo suficiente.

---

## 10. Direção Visual do Jogo

### Identidade visual aplicada

| Elemento | Especificação |
|----------|---------------|
| Ilustrações de personagens | Versão de combate dos personagens dos rótulos; estilo Realismo Narrativo com influência fantástica |
| Verso das cartas | Ver Seção 14 — Prompt completo |
| Bordas por tipo | Ataque: Âmbar / Defesa: Aço / Cura: Floresta / Habilidade: Ouro / Especial: Chama |
| Tipografia | Títulos: Cinzel Decorative / Textos de efeito: Lora / Microtextos: Cinzel |
| Arte da caixa | 6 personagens ao redor de mesa de taverna, cada um com sua caneca — cena panorâmica épica |

### Paleta de cores

| Cor | Hex | Uso |
|-----|-----|-----|
| Âmbar do Mestre | #C8840A | Bordas de ataque, destaques |
| Chama da Forja | #D4520E | Bordas de cartas especiais |
| Floresta Profunda | #1E3D1E | Bordas de cura |
| Aço Encantado | #6B8FA8 | Bordas de defesa |
| Ouro da Coroa | #C8A028 | Bordas de habilidade |
| Pergaminho | #F5E6C8 | Textos principais |
| Tinta das Sombras | #120E06 | Fundo das cartas e caixa |

---

## 11. Componentes e Box Colecionador

| Item | Descrição | Qtd. |
|------|-----------|------|
| Decks de cartas | 30 cartas por personagem, em sleeves individuais | 6 decks |
| Total de cartas | — | 180 |
| Marcadores de Pints | Formato de barril miniatura, trilho de 20 posições | 6 |
| Manual Ilustrado | 32 páginas, regras + lore + galeria | 1 |
| D20 Valirian | Dado de vinte faces com logo | 1 |
| Cartas de Referência | Resumo de regras por personagem | 6 |
| Box externo | Caixa rígida com fecho magnético, arte épica | 1 |

---

## 12. Estratégia de Lançamento

| Edição | Conteúdo | Tiragem | Preço Sugerido |
|--------|----------|---------|----------------|
| Edição do Aventureiro | Box completo com 6 decks | 500 unidades | R$ 249–299 |
| Decks Avulsos | Cada deck individual | 200 por deck | R$ 49–59 |

| Segmento | Canal | Estratégia |
|----------|-------|------------|
| Clientes Valirian | Direto (eventos, loja) | Pré-venda exclusiva para comunidade |
| Colecionadores | Lojas especializadas | Demonstrações e resenhas |
| Público RPG/Board Games | Feiras e eventos | Demonstração ao vivo |
| Eventos de cerveja | Festivais | Degustação + jogo simultâneos |

---

## 13. Roteiro de Desenvolvimento

| Fase | Atividade | Prazo |
|------|-----------|-------|
| 1 | Aprovação do GDD + prototipagem dos 2 decks MVP | 2 semanas |
| 2 | Playtest MVP e ajuste de mecânicas | 2 semanas |
| 3 | Desenvolvimento dos 4 decks restantes | 4 semanas |
| 4 | Arte e design (6 ilustrações + cartas + manual) | 7 semanas |
| 5 | Produção física (caixas, cartas, componentes) | 6 semanas |
| 6 | Pré-venda e lançamento | 3 semanas |
| **Total** | | **~24 semanas** |

### Critérios de aprovação do MVP (2 decks)

- Equilíbrio: nenhum deck vence mais de 65% das partidas (mín. 10 jogadores testadores)
- Clareza: menos de 20% têm dúvidas de regras durante a partida
- Tempo: 90% das partidas duram entre 15 e 35 minutos
- Diversão: 80%+ dos testadores querem jogar novamente

---

## 14. Prompt — Verso dos Cards

O verso de todas as cartas é **único e idêntico** para os 6 decks — não revela o deck do adversário, mantendo o mistério e a identidade visual da marca.

---

### Prompt para geração do verso (Midjourney / Stable Diffusion / DALL-E)

```
Fantasy epic card back design for a craft beer card game called "Fermento & Honra".
Central motif: a majestic dragon coiling around a medieval wooden beer barrel, 
rendered in gold and amber tones. The dragon is a seal/emblem, not a full scene 
— heraldic style with fine line detail. 

Above the dragon: wordmark "VALIRIAN" in ornate medieval serif (Cinzel Decorative style), 
color parchment/cream (#F5E6C8). Below the dragon: tagline "FERMENTO & HONRA" in small 
caps with wide letter spacing, color amber (#C8840A).

Background: deep dark warm black (#120E06) with subtle parchment texture and very faint 
repeating geometric diamond pattern. A thin decorative border with corner ornaments 
in aged gold (#C8A028) frames the entire card. Border style: interlocking chain with 
small fleur-de-lis at corners.

Overall mood: premium, epic, medieval tavern. Think Game of Thrones meets craft beer label.
Style: fantasy realism, high detail, rich texture, dramatic lighting from below.
Color palette: #120E06 (background), #C8840A (amber accents), #C8A028 (gold details), 
#F5E6C8 (parchment text), #D4520E (flame accent on dragon eyes).
Card dimensions: 63mm × 88mm (standard card), 300dpi minimum.
No gradients on background. Flat warm dark surface with fine texture overlay.
```

---

### Especificação técnica do verso

| Elemento | Especificação |
|----------|---------------|
| Dimensões | 63 × 88 mm (padrão Poker) |
| Resolução | 300 dpi mínimo |
| Fundo | #120E06 com textura de pergaminho sutil |
| Motivo central | Dragão heráldico em estilo selo/emblema, tonalidades ouro |
| Logo "VALIRIAN" | Cinzel Decorative Bold, cor #F5E6C8, acima do dragão |
| Tagline "FERMENTO & HONRA" | Cinzel Regular, cor #C8840A, abaixo do dragão, espaçamento largo |
| Borda | Fina, ornamental, cor #C8A028, cantos com ornamentos florais |
| Padrão de fundo | Losangos geométricos sutis em textura |
| Olhos do dragão | Ponto de luz #D4520E (chama) |
| Sangria | 3 mm em todos os lados |

---

### Variações do verso (se necessário)

Para edições especiais ou decks avulsos, o verso pode ter uma variação de cor de borda mantendo todos os outros elementos:

| Deck | Cor da borda (variação) | Hex |
|------|------------------------|-----|
| Pacto das Sombras | Roxo-escuro | #4A2060 |
| Sangue de Druida | Verde-floresta | #1E3D1E |
| Elixir da Dríade | Verde-esmeralda | #2E5C2E |
| Orvalho de Valirian | Azul-aço | #6B8FA8 |
| Juramento do Aventureiro | Âmbar-dourado | #C8840A |
| Tempestade de Trigo | Laranja-chama | #D4520E |

> **Recomendação:** Usar o verso padrão (âmbar dourado) para o box completo. Verso com cor variante apenas em decks avulsos para diferenciação visual na prateleira.

---

## 15. Padrão de Efeitos — Regras de Texto

Para manter a legibilidade nas cartas impressas em tamanho padrão (63×88mm), todos os textos de efeito seguem estas regras:

| Regra | Parâmetro |
|-------|-----------|
| Limite de caracteres por efeito | **≤255 caracteres** (hard limit: 300) |
| Fonte do efeito na carta | Lora Regular, 8–9pt |
| Área disponível para texto | ~50mm × 18mm (zona de efeito) |
| Quebra de linha automática | Sim (fontes até 9pt cabem ~4 linhas) |
| Abreviações permitidas | ≤ (menor ou igual), ≥ (maior ou igual), + (mais), 🛡️×N (N de defesa) |
| Formatação de condições | "Se [condição], [efeito]." sempre que houver bônus condicional |
| Formatação de custos | "Você sofre N de dano." ao final da descrição |

### Exemplos de efeito bem formatado

✓ **Bom (89 chars):**
`Cause 3 de dano. Se o oponente tiver 10 ou menos de vida, cause +2 (total 5).`

✓ **Bom (96 chars):**
`🛡️×3. Quando destruída, cause 1 de dano ao atacante.`

✓ **Aceitável (219 chars):**
`Olhe as 3 cartas do topo do baralho. Coloque-as de volta em qualquer ordem. Se a passiva foi 19-20 neste turno, compre 1 carta adicional.`

✗ **Longo demais — reescrever (312 chars):**
`Cause 4 de dano em um oponente e todos os outros sofrem 2. Você pode curar 2 de vida se tiver menos de 10 Pints. Além disso, um aliado à escolha compra 1 carta. Se você escolheu Ataque no início do jogo, cause +1 adicional em todos os alvos.`

---

*Game Design Document — Versão 2.1*
*Fermento & Honra — O Duelo das Tavernas*
*Cervejaria Valirian · contato@valirian.com.br · @nanocervejariavalirian*
