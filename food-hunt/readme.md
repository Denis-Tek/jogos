# 🐜 Food Hunt: Formigas Pixeladas

[![Jogar Agora](https://img.shields.io/badge/Jogar%20Agora-Food%20Hunt-16a34a?style=for-the-badge&logo=google-chrome&logoColor=white)](https://denis-tek.github.io/jogos/food-hunt/)
[![Voltar ao Menu](https://img.shields.io/badge/Menu-Coleção%20de%20Jogos-334155?style=for-the-badge)](https://denis-tek.github.io/jogos/)

Quebra-cabeça estratégico casual (*puzzle*) desenvolvido em arquivo único (`index.html`), onde o jogador gerencia o suprimento de cores em **5 slots ativos** para comandar formigas trabalhadoras que escavam e devoram imagens pixelizadas de fora para dentro, percorrendo exclusivamente caminhos e túneis abertos.

🔗 **Link para execução online:** [https://denis-tek.github.io/jogos/food-hunt/](https://denis-tek.github.io/jogos/food-hunt/)

---

## 📸 Preview

![Food Hunt: Formigas Pixeladas em execução](./imagem.png)

---

## ✨ Funcionalidades e Regras do Jogo

* **Regra de Exposição Real (Bordas e Túneis):**
  * O objetivo é devorar 100% dos pixels da bandeja utilizando os blocos distribuídos nas **5 colunas inferiores**.
  * As formigas alcançam apenas pixels **expostos** (conectados por um corredor aberto até a borda externa). Pixels internos permanecem soterrados até que as camadas externas sejam escavadas.
* **Gerenciamento de 5 Slots Ativos (Potes):**
  * Tocar no bloco do topo de qualquer coluna ocupa um **slot vazio** entre os 5 potes disponíveis; blocos da mesma cor ocupam slots independentes até serem esvaziados.
  * Cores sem pixels expostos no momento exibem um **cadeado e borda vermelha**, aguardando abertura de passagem.
  * **Prevenção de Impasse (*Deadlock*):** Preencher os 5 slots com cores soterradas trava o formigueiro — utilize os **Destravadores** limitados estrategicamente.
* **Conversor de Imagens Integrado (Upload de Fotos):**
  * Carregue qualquer foto do celular ou computador com quantização automática de paleta (**6, 8 ou 10 cores**), remoção opcional de fundo branco/transparente e ajuste de grade (`20×20`, `26×26` ou `32×32`).
* **3 Desenhos Clássicos & 3 Níveis de Dificuldade:**
  * Fases prontas (*Ratinho na Folha*, *Melancia* e *Hambúrguer*) e modos **Fácil** (3 Destravadores), **Médio** (2 Destravadores) e **Difícil** (1 Destravador), além de seletor de velocidade (`1x`, `2x` e `4x`).

---

## 🧠 Tecnologias e Algoritmos

* **HTML5 Canvas 2D:** Renderização fluida em 60 FPS da bandeja 3D, pixels chanfrados, partículas e formigas articuladas que assumem dinamicamente a cor do pixel coletado.
* **Flood-Fill Perimetral & BFS (*Breadth-First Search*):** Detecção em tempo real dos espaços conectados à saída externa e cálculo da menor rota ortogonal pelos túneis abertos na ida e na volta ao formigueiro.
* **K-Means Clustering:** Algoritmo nativo para agrupamento inteligente de cores ao converter imagens enviadas pelo jogador, mantendo contabilidade exata entre os pixels da grade e os blocos das colunas.
* **Web Audio API & CSS3/Tailwind:** Síntese procedural de efeitos sonoros sem arquivos externos e interface *mobile-first* responsiva.