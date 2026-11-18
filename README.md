<div align="center">

# 🐦 Flappy Bird em Godot

**Um clone de Flappy Bird feito na Godot 4, com três fases, parallax, moedas e recorde.**

![Godot](https://img.shields.io/badge/Godot%204-478CBF?logo=godotengine&logoColor=white)
![GDScript](https://img.shields.io/badge/GDScript-355570?logo=godotengine&logoColor=white)

<img src="imagens_readme/flappy_leo1.png" alt="Pássaro azul voando entre obstáculos de pedra, com uma moeda à frente" width="300">

### 🎬 [Ver o vídeo demonstrativo](https://youtu.be/ZRAgJsmeNho)

</div>

---

## 🎮 O que é

Um jogo de pássaro que voa entre obstáculos, feito na **Godot 4** como estudo de desenvolvimento de jogos. A cada partida o pássaro ganha uma cor aleatória, e o cenário, os obstáculos e a música mudam conforme a pontuação sobe.

## ⌨️ Controles

| Tecla | Ação |
|---|---|
| `Espaço`, `Enter` ou clique | Bater as asas / começar a partida |
| `Esc` | Fechar o jogo |

## ✨ Funcionalidades

- **Física de voo.** O pássaro cai com a gravidade, sobe a cada toque e inclina o bico conforme a velocidade.
- **Fundo com parallax.** As camadas do cenário andam em velocidades diferentes, dando sensação de profundidade.
- **Obstáculos gerados sozinhos.** Um novo par de obstáculos aparece a cada 2 segundos, numa altura aleatória.
- **Moedas.** Cada obstáculo traz uma moeda no vão. Pegar a moeda vale 1 ponto.
- **Três fases.** O cenário, os obstáculos e a música mudam conforme a pontuação:

  | Pontos | Fase |
  |---|---|
  | 0 a 30 | 🌲 Campo, obstáculos de pedra |
  | 31 a 60 | ❄️ Neve |
  | 61 ou mais | 🏜️ Deserto |

- **Cor aleatória.** O pássaro ganha uma combinação de cores diferente em cada partida.
- **Game over e recorde.** Ao bater, aparece a tela com a pontuação da partida e o recorde atual, e um aviso de "Novo recorde!" quando ele é superado.

## ▶️ Como rodar

1. Instale a [Godot 4](https://godotengine.org/download/) (o projeto está configurado na versão **4.3**).
2. Clone o repositório:

   ```bash
   git clone https://github.com/LeandroCustodio2002/flappyBird.git
   ```

3. Na Godot, clique em **Importar** e selecione o arquivo `project.godot` da pasta.
4. Aperte **F5** para jogar.

## 📚 Tutorial

O arquivo [`TUTORIAL.md`](TUTORIAL.md) ensina a montar o jogo do zero, passo a passo e com prints: estrutura de pastas, script global, personagem, parallax, obstáculos, moedas, pontuação e tela de game over.

## 📁 Estrutura

| Pasta | Conteúdo |
|---|---|
| `cenas/` | Cenas do jogo: tela inicial (`tutorial`), partida (`main`), personagem, obstáculo, moeda, cenário, menu de game over e música |
| `scripts/` | Lógica em GDScript. O `Global.gd` guarda vida, pontos, fase, recorde e a cor do pássaro |
| `sprites/` | Pássaro, moeda, obstáculos e cenários das três fases |
| `sons/` | Efeitos de voo, moeda e morte, e as músicas de fundo |
| `font_style/` | Fonte usada nos textos |
| `imagens_readme/` | Imagens do README e do tutorial |

## 🙏 Créditos

- **Pássaro e moedas:** imagens da internet ([pássaro](https://www.pngitem.com/middle/iimbwJh_flappy-bird-bird-png-transparent-png/), [moedas](https://www.seekpng.com/ima/u2e6y3o0t4t4t4w7/)).
- **Fundo com parallax:** [bitbrain/godot-tutorials](https://github.com/bitbrain/godot-tutorials/tree/main/parallax-scrolling/godot-project/parallax).
- **Obstáculos e chão das três fases:** autorais.
- **Músicas de fundo:** trilha sonora de *Terraria* (Re-Logic).
