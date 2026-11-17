# 🐍 Snake — Jogo da Cobrinha

Releitura moderna, responsiva e nostálgica do clássico **Jogo da Cobrinha (Snake)**, desenvolvida em **arquivo único autônomo (`index.html`)** com alternância instantânea entre o tema **Neon Moderno** (iluminação glow, partículas e interpolação fluida a 60 FPS) e o icônico modo retrô **Nokia 3310** (tela LCD monocromática).

🔗 **Link para execução online:** <https://denis-tek.github.io/jogos/snake/>

## 📸 Preview

## ✨ Funcionalidades e Regras do Jogo

* **Dois Temas Visuais Alternáveis:**

  * **Neon Moderno:** Grade escura, iluminação *glow*, cauda afilada com movimento interpolado, olhos que acompanham a fruta e explosão de partículas ao pontuar.

  * **Nokia 3310 Clássico:** Tela LCD verde (`#9bbc0f`), blocos pixelados monocromáticos, fonte retrô *Press Start 2P* e efeito de matriz LCD.

* **Dois Modos de Arena:**

  * **Com Paredes:** Colidir com as bordas da arena encerra a partida (regra tradicional).

  * **Sem Paredes (Portal):** Ao atravessar uma borda, a cobra ressurge suavemente no lado oposto da tela.

* **Velocidades & Fruta Bônus:**

  * Três velocidades iniciais (**Lento**, **Normal** e **Rápido**) com aceleração gradual conforme a pontuação aumenta.

  * **Fruta Bônus Temporária:** A cada 5 frutas coletadas, uma fruta dourada (`+50` pontos) surge na arena acompanhada de uma barra de tempo regressiva.

* **Controles Multiplataforma & Persistência:**

  * Fila de comandos (*Input Buffering*) que impede giros acidentais de 180° em toques rápidos, suporte nativo a *swipe* e **D-Pad tátil** na tela, além de salvamento automático do recorde e preferências no `localStorage`.

## 🎮 Controles

| Ação | Teclado (Desktop) | Touch / Mobile | 
| ----- | ----- | ----- | 
| **Mover para Cima** | `↑` ou `W` | Deslizar para cima / Botão `▲` | 
| **Mover para Baixo** | `↓` ou `S` | Deslizar para baixo / Botão `▼` | 
| **Mover para Esquerda** | `←` ou `A` | Deslizar para esquerda / Botão `◀` | 
| **Mover para Direita** | `→` ou `D` | Deslizar para direita / Botão `▶` | 
| **Pausar / Continuar** | `Espaço`, `P` ou `Esc` | Botão de Pausa no topo | 
| **Iniciar / Reiniciar** | `Enter` ou `Espaço` | Botão na tela | 

## 🛠️ Tecnologias e Algoritmos

* **HTML5 Canvas API:** Renderização 2D acelerada a 60 FPS com suporte a telas Retina/HiDPI (`devicePixelRatio`).

* **CSS3 & Tailwind CSS (via CDN):** Layout responsivo *zero-scroll* (`100dvh`) adaptável a celulares, tablets e monitores widescreen.

* **JavaScript (ES6+):** Arquitetura orientada a objetos com *Game Loop* desacoplado, *Input Buffering* para prevenção de autocolisão e interpolação suave de quadros.

* **Web Audio API & `localStorage`:** Sintetizador de ondas (`sine`, `square`, `triangle`, `sawtooth`) para efeitos sonoros dinâmicos sem arquivos externos e persistência local de recordes.