# 🧱 Tetris Pro

Versão moderna, responsiva e fiel às regras oficiais (*Tetris Guideline*) do clássico jogo de quebra-cabeça **Tetris**, desenvolvida em um único arquivo HTML5, CSS3 e JavaScript puro, sem dependências externas.

🔗 **Jogar online:** [https://denis-tek.github.io/jogos/tetris/](https://denis-tek.github.io/jogos/tetris/)

![Preview do Tetris Pro](imagem.png)

---

## ✨ Recursos e Mecânicas

* **Padrão Oficial (*Tetris Guideline*):**
  * **Matriz `10×20`:** Tabuleiro clássico com 2 linhas superiores ocultas de *buffer* para geração suave das peças.
  * **Gerador Aleatório *7-Bag*:** Garante distribuição equilibrada das 7 peças (*I, J, L, O, S, T, Z*) em ciclos embaralhados, evitando sequências injustas.
  * **Sistema de Rotação SRS (*Super Rotation System*):** Inclui tabelas oficiais de *Wall Kick* (inclusive para a peça **I**) permitindo encaixes precisos junto às paredes e pilhas de blocos.
  * **Peça Fantasma (*Ghost Piece*):** Projeção translúcida na base da coluna indicando exatamente onde o tetrominó irá aterrissar.
  * **Reserva (*Hold*) e Fila de Próximas Peças:** Permite guardar uma peça para uso estratégico e visualizar horizontalmente os próximos 3 tetrominós.
  * **Lock Delay & Combos:** Atraso de 500ms ao tocar o solo (com até 15 movimentos/rotações de ajuste), além de pontuação progressiva para *Single*, *Double*, *Triple*, *Tetris* (4 linhas), *Back-to-Back*, *Combos*, *Soft Drop* e *Hard Drop*.
* **Interface Otimizada (`100dvh` sem rolagem):**
  * Faixa horizontal superior para **Reserva** e **Próximas 3 Peças**.
  * Área central maximizada com redimensionamento dinâmico em alta definição (`devicePixelRatio`).
  * Faixa horizontal inferior de contadores (**Pontos**, **Nível** e **Linhas**) e recorde persistente via `localStorage`.
  * Alternância instantânea entre **Tema Escuro** e **Tema Claro**.
* **Áudio Retrô Sintetizado:** Efeitos sonoros gerados em tempo real via *Web Audio API* (movimento, rotação, encaixe, limpeza de linhas, *Tetris*, subida de nível e *Game Over*), sem necessidade de arquivos de áudio externos.

---

## 🎮 Controles

### Computador (Teclado)
| Tecla | Ação |
| :--- | :--- |
| `←` / `→` | Mover peça para esquerda / direita (com repetição contínua DAS/ARR) |
| `↓` | *Soft Drop* (queda acelerada +1 ponto por linha) |
| `Espaço` | *Hard Drop* (queda instantânea +2 pontos por linha) |
| `↑` ou `X` | Girar no sentido horário |
| `Z` ou `Ctrl` | Girar no sentido anti-horário |
| `C` ou `Shift` | Guardar / Trocar peça na **Reserva (Hold)** |
| `P` ou `Esc` | Pausar / Retomar partida |

### Dispositivos Móveis e Touch
* **Gestos diretos no tabuleiro:** Arraste horizontalmente para mover, deslize rápido para baixo para *Hard Drop*, arraste lentamente para baixo para *Soft Drop* e toque para girar no sentido horário.
* **Controles Arcade na tela:** Barra inferior dedicada com botões táteis para movimento contínuo, rotações (horária e anti-horária), *Hold* e *Hard Drop* (também ativável no desktop pelo botão de controle no topo).

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 Canvas API:** Renderização nítida dos blocos com chanfros, iluminação interna e grade responsiva.
* **CSS3 (Custom Properties, Flexbox & Grid):** Layout adaptativo em tela cheia (`100dvh`) com suporte a temas claro e escuro.
* **JavaScript (ES6+):** Loop de jogo baseado em `requestAnimationFrame` com controle de delta de tempo, SRS *Wall Kicks*, *7-Bag RNG* e persistência local.
* **Web Audio API:** Sintetizador polifônico leve para efeitos sonoros interativos.

---

## 📂 Estrutura do Projeto

```text
tetris/
├── index.html      # Aplicação completa (HTML, CSS e JavaScript integrados)
├── imagem.png      # Captura de tela utilizada na visualização do projeto
└── README.md       # Documentação do jogo