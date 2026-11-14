# 💣 Campo Minado Pro

Uma versão moderna, responsiva e completa do clássico jogo **Campo Minado** (*Minesweeper*), desenvolvida em arquivo único (`HTML5`, `CSS3`/`Tailwind CSS` e `JavaScript` puro) com suporte nativo para **Desktop** e **Mobile**, áudio sintetizado em tempo real e alternância instantânea entre tema **Dark Moderno** e **Clássico Anos 90**.

---

## ✨ Funcionalidades Principais

* **🛡️ 1º Clique Sempre Seguro (*Safe First Click*):** As minas são distribuídas apenas após a sua primeira jogada, garantindo que a célula clicada e seus 8 vizinhos estejam livres para abrir uma clareira inicial baseada em lógica.
* **🌊 Abertura em Cascata (*Flood Fill* BFS):** Algoritmo iterativo de busca em largura que revela instantaneamente áreas vazias adjacentes sem risco de estouro de pilha.
* **⚡ Abertura Rápida (*Chording*):** Clique (ou dê duplo clique) em um número já revelado que já possua a quantidade exata de bandeiras ao seu redor para abrir todas as células vizinhas restantes de uma só vez.
* **🎨 Duplo Tema Visual:**
  * **🌙 Dark Moderno:** Interface translúcida com *glassmorphism*, cores suaves de alto contraste e animações fluidas.
  * **🕹️ Clássico Anos 90:** Visual nostálgico inspirado no Windows 95, com bordas chanfradas 3D e display digital estilo LED.
* **📱 Experiência Mobile First & Desktop:**
  * Barra inferior rápida para alternar entre **⛏️ Modo Cavar** e **🚩 Modo Bandeira**.
  * Suporte a **Toque Longo (*Long Press* de 350ms)** com indicador visual e vibração tátil para marcar bandeiras com agilidade em telas sensíveis ao toque.
  * Ajuste de zoom inteligente (`Auto`, `Grande`, `Compacto`) para tabuleiros extensos.
* **🔊 Áudio Procedural (*Web Audio API*):** Efeitos sonoros sintetizados diretamente no navegador para escavação, cascata, bandeiras, explosão e fanfarra de vitória — sem necessidade de arquivos `.mp3` ou `.wav` externos.
* **💡 Dica Inteligente & Recordes Locais:** Sistema que identifica deduções lógicas seguras no tabuleiro e salva automaticamente seus melhores tempos por dificuldade via `localStorage`.

---

## 🎮 Níveis de Dificuldade

| Dificuldade | Dimensões (Colunas × Linhas) | Total de Minas |
| :--- | :---: | :---: |
| **Iniciante** | `9 × 9` | `10` |
| **Intermediário** | `16 × 16` | `40` |
| **Especialista** | `30 × 16` | `99` |
| **Personalizado** | `5×5` até `40×30` | `1` até `(L × A) - 9` |

---

## 🕹️ Como Jogar

### 💻 No Computador (Mouse)
* **Clique Esquerdo:** Revela a célula (ou executa *Chording* em números já abertos).
* **Clique Direito:** Alterna entre **🚩 Bandeira**, **❓ Dúvida** e célula limpa.

### 📱 No Celular / Tablet (Touch)
* **Toque Simples:** Executa a ação selecionada na barra inferior (**⛏️ Cavar** ou **🚩 Bandeira**).
* **Segurar o Toque (350ms):** Coloca ou remove uma **🚩 Bandeira** diretamente, independentemente do modo selecionado.

---

## 🚀 Como Executar Localmente

Por ser construído em arquitetura **Single-File** sem dependências de build, basta clonar o repositório e abrir o arquivo `index.html` diretamente em qualquer navegador moderno:

```bash
git clone https://github.com/seu-usuario/campo-minado-pro.git
cd campo-minado-pro
```

---

## 🛠️ Tecnologias Utilizadas

* **HTML5** (Estrutura semântica e acessível)
* **Tailwind CSS (via CDN)** & **CSS3 Custom Properties** (Temas dinâmicos e layout responsivo)
* **JavaScript (ES6+)** (Lógica de jogo, algoritmos de busca e manipulação de DOM)
* **Web Audio API** (Síntese sonora em tempo real)
* **LocalStorage API** (Persistência de recordes por dificuldade)