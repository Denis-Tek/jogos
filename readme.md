# 🕹️ Coleção de Jogos Clássicos

[![GitHub Pages](https://img.shields.io/badge/Jogar%20Online-GitHub%20Pages-2563eb?style=for-the-badge&logo=github)](https://denis-tek.github.io/jogos/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#tecnologias-utilizadas)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#tecnologias-utilizadas)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2020+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#tecnologias-utilizadas)

Uma coleção interativa de brinquedos eletrônicos retrô, passatempos de tabuleiro e puzzles casuais recriados para a web com **foco em design tátil**, **síntese sonora em tempo real** e **arquitetura autônoma em arquivo único**.

🔗 **Acesse o Launcher Principal:** [https://denis-tek.github.io/jogos/](https://denis-tek.github.io/jogos/)

---

## 🎮 Catálogo de Jogos

| Jogo | Categoria | Descrição | Link Direto |
| :--- | :--- | :--- | :--- |
| **[Genius Estrela](./genius-estrela/)** | Memória & Som | Recriação fiel do brinquedo eletrônico dos anos 80 com 4 arcos luminosos, visor LED de 4 segmentos, 3 modos de jogo e 4 níveis de dificuldade. | [Jogar Genius Estrela](https://denis-tek.github.io/jogos/genius-estrela/) |
| **[Resta Um](./resta-um/)** | Raciocínio & Tabuleiro | O clássico *Peg Solitaire* em tabuleiro circular de madeira nobre com 5 variantes, 4 acabamentos de peças e solucionador inteligente integrado. | [Jogar Resta Um](https://denis-tek.github.io/jogos/resta-um/) |
| **[Food Hunt](./food-hunt/)** | Puzzle & Estratégia | Quebra-cabeça casual onde você gerencia 5 slots de cores para comandar formigas pixeladas que escavam desenhos e fotos enviadas pelo jogador. | [Jogar Food Hunt](https://denis-tek.github.io/jogos/food-hunt/) |
| **[Water Sort Puzzle](./water-sort/)** | Lógica & Organização | Quebra-cabeça de tubos de ensaio onde você separa líquidos coloridos com fases validadas via DFS, paleta de alto contraste e temas claro/escuro. | [Jogar Water Sort](https://denis-tek.github.io/jogos/water-sort/) |
| **[Campo Minado Pro](./campo-minado/)** | Lógica & Dedução | Versão responsiva do clássico *Minesweeper* com 1º clique seguro, abertura rápida (*Chording*), dica lógica e temas Dark Moderno e Clássico Anos 90. | [Jogar Campo Minado](https://denis-tek.github.io/jogos/campo-minado/) |
| **[Paciência Clássica](./paciencia/)** | Cartas & Estratégia | Versão completa do *Klondike Solitaire* com compra de 1 ou 3 cartas, detector de impasses via BFS, dicas inteligentes e temas Esmeralda e Meia-Noite. | [Jogar Paciência](https://denis-tek.github.io/jogos/paciencia/) |
| **[Cubo Mágico 3x3](./cubo-magico/)** | Quebra-Cabeça 3D | Simulador 3D interativo com motor gráfico próprio em Canvas 2D, notação oficial WCA, cronômetro de *Speedcubing*, *Auto-Solve* e temas claro/escuro. | [Jogar Cubo Mágico](https://denis-tek.github.io/jogos/cubo-magico/) |
| **[Sudoku Pro](./sudoku/)** | Lógica & Números | Quebra-cabeça numérico com geração de solução única via *backtracking*, modo lápis, dicas pedagógicas (*Naked/Hidden Single*) e temas claro/escuro. | [Jogar Sudoku Pro](https://denis-tek.github.io/jogos/sudoku/) |
| **[Dots & Boxes](./dots-and-boxes/)** | Estratégia & Tabuleiro | O clássico *Jogo dos Pontinhos* em SVG vetorial com modos 1P vs IA (3 níveis com análise de cadeias) ou 2 Jogadores, 3 tamanhos de grade e temas claro/escuro. | [Jogar Dots & Boxes](https://denis-tek.github.io/jogos/dots-and-boxes/) |
| **[Two Dots](./two-dots/)** | Puzzle & Conexões | Quebra-cabeça minimalista de conexão de pontos iguais em grade `6×6` com eliminação global de cor por circuitos fechados (*loops*), 3 modos e escala pentatônica. | [Jogar Two Dots](https://denis-tek.github.io/jogos/two-dots/) |
| **[Tetris](./tetris/)** | Arcade & Lógica | Clássico empilhador de tetrominós em matriz `10×20` com gerador *7-Bag*, rotação com *wall kicks*, peça fantasma (*Ghost Piece*), reserva (*Hold*) e progressão de velocidade. | [Jogar Tetris](https://denis-tek.github.io/jogos/tetris/) |
| **[Jogo de Damas](./damas/)** | Raciocínio & Tabuleiro | Edição de luxo em tabuleiro `8×8` com regras brasileiras (*Dama Voadora* e *Lei da Maioria*), modo casual, 2 jogadores e IA com algoritmo Minimax Alfa-Beta. | [Jogar Damas](https://denis-tek.github.io/jogos/damas/) |
| **[Snake](./snake/)** | Arcade & Reflexos | Clássico Jogo da Cobrinha em Canvas 2D com temas **Neon Moderno** e **Nokia 3310**, arenas com ou sem paredes, fruta bônus temporária e D-Pad tátil. | [Jogar Snake](https://denis-tek.github.io/jogos/snake/) |

---

## 🛠️ Tecnologias Utilizadas

Todo o ecossistema foi projetado sob o conceito **Single-File Self-Contained Architecture** (cada aplicação encapsulada em seu próprio `index.html`), garantindo portabilidade instantânea, carregamento ultrarrápido e compatibilidade nativa com qualquer navegador moderno ou hospedagem estática:

* **HTML5 Semântico, Canvas 2D & SVG Vetorial:** Estruturação acessível (ARIA), ilustrações vetoriais embutidas para o menu inicial, grades interativas com áreas de toque ampliadas (`hit-area`) e renderização acelerada em 60 FPS no `<canvas>` (incluindo projeção 3D em software com matrizes ortonormais $3\times3$).
* **CSS3 Moderno & Tailwind CSS:** Uso de variáveis dinâmicas (`Custom Properties`), `CSS Grid`, `Flexbox`, `clamp()`, `100dvh`, `ResizeObserver`, Web Animations API e gradientes radiais multicamada para texturas físicas e layouts *zero-scroll*.
* **JavaScript Nativo (ES2020+):** Lógica de estados, algoritmos de busca, grafos e inteligência artificial (`Minimax` com poda Alfa-Beta, `DFS` com `BigInt` Bitboard e poda de estados, `BFS` com tabela de transposição e *Flood-Fill*, *backtracking* com verificação de unicidade, detecção de ciclos/loops em grafos, avaliação heurística de cadeias e deduções lógicas), clusterização de cores (*K-Means*), embaralhamento *7-Bag* com *Wall Kicks*, *Input Buffering* com interpolação de quadros, álgebra vetorial 3D, eventos unificados (`Pointer Events` / *Long Press*) e atalhos de teclado.
* **Web Audio API:** Motor de síntese sonora 100% procedural (osciladores, escalas pentatônicas e envelopes ADSR) que gera em tempo real os tons musicais, fluxos líquidos, efeitos táteis e fanfarras — sem depender de arquivos `.mp3` ou `.wav`.
* **Web Storage API (`localStorage`):** Persistência local automática dos recordes, fases desbloqueadas e preferências de tema/áudio em cada jogo.

---

## 📁 Estrutura do Repositório

```text
jogos/
├── index.html                 # Launcher principal com filtros, busca e leitura de recordes
├── README.md                  # Documentação geral do repositório
├── genius-estrela/
│   ├── index.html             # Aplicação completa do Genius da Estrela
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica e regras do Genius
├── resta-um/
│   ├── index.html             # Aplicação completa do Resta Um (Peg Solitaire)
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, variantes e algoritmos do Resta Um
├── food-hunt/
│   ├── index.html             # Aplicação completa do Food Hunt: Formigas Pixeladas
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Food Hunt
├── water-sort/
│   ├── index.html             # Aplicação completa do Water Sort Puzzle
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Water Sort
├── campo-minado/
│   ├── index.html             # Aplicação completa do Campo Minado Pro
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Campo Minado
├── paciencia/
│   ├── index.html             # Aplicação completa da Paciência Clássica (Klondike)
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos da Paciência
├── cubo-magico/
│   ├── index.html             # Aplicação completa do Cubo Mágico 3x3 (Simulador 3D)
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, controles e algoritmos do Cubo Mágico
├── sudoku/
│   ├── index.html             # Aplicação completa do Sudoku Pro
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Sudoku
├── dots-and-boxes/
│   ├── index.html             # Aplicação completa do Dots & Boxes (Jogo dos Pontinhos)
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Dots & Boxes
├── two-dots/
│   ├── index.html             # Aplicação completa do Two Dots — Puzzle de Conexões
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Two Dots
├── tetris/
│   ├── index.html             # Aplicação completa do Tetris
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, controles e regras do Tetris
├── damas/
│   ├── index.html             # Aplicação completa do Jogo de Damas — Edição de Luxo
│   ├── imagem.png             # Captura de tela do jogo em execução
│   └── README.md              # Documentação técnica, regras e algoritmos do Jogo de Damas
└── snake/
    ├── index.html             # Aplicação completa do Snake — Jogo da Cobrinha
    ├── imagem.png             # Captura de tela do jogo em execução
    └── README.md              # Documentação técnica, controles e regras do Snake
```

---

## 🚀 Como Executar Localmente

Como não há etapa de compilação (*build*) ou instalação de pacotes:

1. Clone este repositório:
   ```bash
   git clone https://github.com/Denis-Tek/jogos.git
   ```
2. Abra o arquivo `index.html` da raiz (ou de qualquer subpasta) diretamente no seu navegador preferido.

---

Desenvolvido por **[Denis-Tek](https://github.com/Denis-Tek)**.