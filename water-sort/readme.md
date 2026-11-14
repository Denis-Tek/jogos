# 🧪 Water Sort Puzzle

Um jogo casual de lógica e quebra-cabeça desenvolvido em **HTML5, CSS3 e JavaScript puro (Vanilla JS)**, empacotado em um **único arquivo autônomo (`index.html`)** sem dependências externas, frameworks ou arquivos de áudio de terceiros.

## 📸 Preview

![Preview do Water Sort Puzzle](imagem.png)

## 🎮 Sobre o Jogo

O objetivo do **Water Sort Puzzle** é organizar líquidos coloridos misturados em tubos de ensaio até que cada frasco contenha apenas uma única cor e esteja completamente cheio.

### Regras

1. **Seleção e Despejo:** Clique ou toque em um tubo para selecioná-lo e depois clique no tubo de destino.
2. **Compatibilidade de Cores:** Você só pode despejar um líquido sobre outro se ambos forem da **mesma cor** e houver espaço disponível no tubo de destino.
3. **Tubos Vazios:** Qualquer cor pode ser transferida para um tubo totalmente vazio.
4. **Conclusão:** Ao preencher um tubo com 4 camadas da mesma cor, ele é automaticamente selado com uma rolha de cortiça.

## ✨ Principais Recursos

* **Geração de Fases Garantidamente Solucionáveis:**
  * Utiliza embaralhamento validado por um **Solver DFS (Busca em Profundidade)** com poda de estados equivalentes e *fallback* de embaralhamento reverso, assegurando que nenhuma fase impossível seja gerada.
  * Escalada progressiva de dificuldade: inicia com **3 cores + 2 tubos vazios** e avança gradualmente até **12 cores + 2 tubos vazios**.

* **Paleta 100% Cromática de Alto Contraste:**
  * **Grupo Prioritário (9 cores):** Vermelho, Azul, Amarelo, Verde, Laranja, Roxo, Ciano, Rosa e Marrom — sorteados primeiro para evitar confusão visual entre tons próximos.
  * **Grupo de Expansão (5 cores):** Verde-Lima, Índigo, Coral, Azul-Petróleo e Dourado — ativados automaticamente apenas em fases que exigem 10 ou mais cores.

* **Áudio Sintetizado em Tempo Real (Web Audio API):**
  * Efeitos sonoros gerados proceduralmente via código (seleção, fluxo de água despejando, erro, acorde de conclusão de tubo e fanfarra de vitória), sem necessidade de carregar arquivos `.mp3` ou `.wav`.

* **Layout Responsivo Zero-Scroll (`100dvh`):**
  * Dimensionamento fluido via CSS (`clamp()`) que adapta automaticamente as garrafas em 1 ou 2 fileiras equilibradas, eliminando qualquer barra de rolagem em dispositivos móveis e desktops.

* **Temas Claro e Escuro + Persistência:**
  * Alternância instantânea entre **Tema Escuro** e **Tema Claro**, salvando automaticamente o nível atual e preferências de áudio/tema no `localStorage`.

* **Ferramentas de Apoio:**
  * **Desfazer:** Histórico completo de jogadas na fase atual.
  * **Reiniciar:** Restaura a configuração inicial exata da fase.
  * **+1 Tubo:** Adiciona 1 tubo vazio extra por fase para ajudar em situações complexas.

## 🚀 Como Executar

Por ser uma aplicação *zero-dependency* em arquivo único:

1. Clone este repositório:

   ```bash
   git clone https://github.com/denis-tek/water-sort-puzzle.git
   ```

2. Acesse a pasta do projeto e abra o arquivo `index.html` diretamente em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).

## 📁 Estrutura do Projeto

```text
water-sort-puzzle/
├── index.html   # Aplicação completa (HTML + CSS + Solver + Web Audio + UI)
├── imagem.png   # Captura de tela do jogo em execução
└── README.md    # Documentação do projeto
```

## 🛠️ Tecnologias Utilizadas

* **HTML5 Semântico**
* **CSS3 Moderno** (Custom Properties, Flexbox, `clamp()`, `100dvh`, Web Animations API)
* **JavaScript (ES6+)**
* **Web Audio API** (Síntese sonora procedural)
* **Web Storage API (`localStorage`)**