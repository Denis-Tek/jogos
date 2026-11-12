# 🕹️ Coleção de Jogos Clássicos

[![GitHub Pages](https://img.shields.io/badge/Jogar%20Online-GitHub%20Pages-2563eb?style=for-the-badge&logo=github)](https://denis-tek.github.io/jogos/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#tecnologias-utilizadas)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#tecnologias-utilizadas)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2020+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#tecnologias-utilizadas)

Uma coleção interativa de brinquedos eletrônicos retrô e jogos de tabuleiro clássicos recriados para a web com **zero dependências externas**, foco em **design tátil realista**, **síntese sonora em tempo real** e **arquitetura autônoma em arquivo único**.

🔗 **Acesse o Launcher Principal:** [https://denis-tek.github.io/jogos/](https://denis-tek.github.io/jogos/)

---

## 🎮 Catálogo de Jogos

| Jogo | Categoria | Descrição | Link Direto |
| :--- | :--- | :--- | :--- |
| **[Genius Estrela](./genius-estrela/)** | Memória & Som | Recriação fiel do brinquedo eletrônico dos anos 80 com 4 arcos luminosos, visor LED de 7 segmentos, 3 modos de jogo e 4 níveis de dificuldade. | [Jogar Genius Estrela](https://denis-tek.github.io/jogos/genius-estrela/) |
| **[Resta Um](./resta-um/)** | Raciocínio & Tabuleiro | O clássico *Peg Solitaire* em tabuleiro circular de madeira nobre com 5 variantes, 4 acabamentos de peças e solucionador inteligente integrado. | [Jogar Resta Um](https://denis-tek.github.io/jogos/resta-um/) |

---

## 🛠️ Tecnologias Utilizadas

Todo o ecossistema foi projetado sob o conceito **Single-File Self-Contained Architecture** (cada aplicação encapsulada em seu próprio `index.html`), garantindo portabilidade instantânea, carregamento ultrarrápido e compatibilidade nativa com qualquer navegador moderno ou hospedagem estática:

* **HTML5 Semântico & SVG Vetorial:** Estruturação acessível e ilustrações vetoriais embutidas para os ícones e componentes gráficos do menu inicial.
* **CSS3 Moderno:** Uso intensivo de variáveis dinâmicas (`Custom Properties`), `CSS Grid`, `Flexbox`, gradientes radiais e cônicos multicamada para simular texturas físicas (plástico chanfrado, madeira entalhada, baquelite e visores LED) e animações fluidas via GPU.
* **JavaScript Nativo (ES2020+):** Lógica de estados, máquinas de turno, manipulação de eventos unificados (`Pointer Events` para mouse e toque), atalhos de teclado e uso de `BigInt` para operações bit-a-bit de alta performance.
* **Web Audio API:** Motor de síntese sonora 100% procedural (osciladores e envelopes ADSR) que gera em tempo real os tons musicais do Genius, o som de erro característico, o estalo de peças de madeira/baquelite e fanfarras de vitória — sem depender de arquivos `.mp3` ou `.wav`.
* **Web Storage API (`localStorage`):** Persistência local automática dos recordes obtidos em cada jogo, sincronizados tanto dentro das partidas quanto nos selos exibidos no menu principal.

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
└── resta-um/
    ├── index.html             # Aplicação completa do Resta Um (Peg Solitaire)
    ├── imagem.png             # Captura de tela do jogo em execução
    └── README.md              # Documentação técnica, variantes e algoritmos do Resta Um
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