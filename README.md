# River Attack 🛩️

Jogo de avião pelo rio, inspirado nos clássicos de rolagem vertical. Um único arquivo (`index.html`), sem dependências, feito para o celular.

## Como jogar

- **Celular:** arraste o dedo para pilotar (para cima acelera, para baixo freia) e segure o botão 🔥 para atirar. Um segundo dedo em qualquer lugar da tela também atira.
- **Computador:** setas ou A/D para mover, ↑/↓ acelera e freia, Espaço atira.
- **Combustível:** voe por cima dos tanques para reabastecer, ou explode eles com um tiro (+80 pontos). Ficou sem combustível, perdeu uma vida.
- **Pontes:** destrua a ponte no fim de cada fase (+500). Bater nela é fatal.
- Vida extra a cada 3000 pontos.
- Cada ponte destruída muda o cenário: dia claro, entardecer, noite, pântano, deserto e gelo.

## Publicar na Vercel

1. Importe este repositório na Vercel (framework preset: **Other**, sem build).
2. Depois do deploy, copie o link e cole na constante `GAME_URL` no começo do script do `index.html`. Ela é usada no botão "Desafiar no WhatsApp".

## Ajustes rápidos (no começo do script)

| Constante | O que faz |
|---|---|
| `GAME_URL` | Link do jogo enviado no desafio pelo WhatsApp |
| `SEC` | Tamanho de cada fase (em fatias do rio) |

Dificuldade, velocidade e combustível estão nas funções `genRow`, `update` e `spawnEnemy`.
