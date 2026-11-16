# 🧩 Sudoku Pro

[![Jogar Agora](https://img.shields.io/badge/Jogar%20Agora-Sudoku%20Pro-0284c7?style=for-the-badge&logo=google-chrome&logoColor=white)](https://denis-tek.github.io/jogos/sudoku/)
[![Voltar ao Menu](https://img.shields.io/badge/Menu-Coleção%20de%20Jogos-334155?style=for-the-badge)](https://denis-tek.github.io/jogos/)

Implementação moderna, responsiva e sem dependências externas do clássico **Sudoku**, desenvolvida em arquivo único (`index.html`) com geração garantida de solução única, modo lápis e dicas pedagógicas baseadas em técnicas reais de dedução lógica.

🔗 **Link para execução online:** [https://denis-tek.github.io/jogos/sudoku/](https://denis-tek.github.io/jogos/sudoku/)

---

## 📸 Preview

![Sudoku Pro em execução](./imagem.png)

---

## ✨ Funcionalidades e Controles

* **Geração Algorítmica com Solução Única:**
  * Utiliza *backtracking* com poda simétrica e contagem de soluções em tempo real para assegurar que cada tabuleiro possua estritamente **uma única solução lógica**.
* **4 Níveis de Dificuldade:**
  * **Fácil** (42 pistas), **Médio** (34 pistas), **Difícil** (28 pistas) e **Expert** (24 pistas).
* **Dica Inteligente Pedagógica (`💡`):**
  * Analisa o tabuleiro em busca de deduções humanas — como **Naked Single** e **Hidden Single** em linhas e colunas — preenchendo a célula e explicando o raciocínio aplicado.
* **Modo Lápis / Anotações (`✏️`):**
  * Registra candidatos de `1` a `9` em células vazias e remove automaticamente anotações conflitantes na linha, coluna e quadrante $3 \times 3$ ao confirmar um número.
* **Feedback Visual & Temas:**
  * Destaca simultaneamente a célula ativa, sua linha, coluna, bloco $3 \times 3$, ocorrências iguais e conflitos, com alternância entre **Tema Claro** e **Tema Escuro** em layout *zero-scroll* (`100dvh`).
* **Atalhos de Teclado e Toque:**
  * `Setas Direcionais` navegam pelo tabuleiro; `1` a `9` inserem números/anotações; `N` alterna entre Caneta e Lápis; `Backspace`/`Delete`/`0` apagam; `Ctrl+Z` desfaz a última jogada.

---

## 🛠️ Tecnologias e Algoritmos

* **HTML5 & CSS3 (CSS Grid + Custom Properties):** Estrutura acessível com atributos ARIA, layout responsivo ajustado em `100dvh` sem barras de rolagem e temas dinâmicos.
* **JavaScript (ES6+) — Backtracking & Inferência Lógica:** Gerador de tabuleiros com verificação de unicidade (`countSolutions`) e motor heurístico de técnicas lógicas de resolução.
* **Web Audio API & `localStorage`:** Síntese procedural dos efeitos sonoros sem arquivos externos e salvamento automático de estatísticas, melhores tempos e preferências visuais.