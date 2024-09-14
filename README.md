
# Sudoku Game

## Sobre 
Este projeto é um jogo de tabuleiro Sudoku desenvolvido como parte de um projeto acadêmico. O jogo oferece uma experiência desafiadora com tabuleiros variados, selecionados aleatoriamente a partir de uma base de 100 tabuleiros, cada um com um nível de dificuldade diferente.

## Tecnologias Utilizadas
- Linguagem: C/C++
- Biblioteca gráfica: Allegro 5

## Funcionalidades

- **Sorteio de Tabuleiros:** A cada nova partida, um tabuleiro é escolhido aleatoriamente entre 100 possibilidades, com diferentes níveis de dificuldade:

  - 0 - Fácil   
  
  - 1 - Médio

  - 2 - Difícil

  - 3 - Osco (extremamente difícil)

- **Registro de Pontos:**  Ao completar o tabuleiro, o jogo verifica o nome do jogador no arquivo de pontuação. Se o jogador já tiver completado o mesmo tabuleiro, os pontos são somados aos anteriores. Caso contrário, é criado um novo registro com a identificação do tabuleiro e a pontuação correspondente.


- **Cálculo de Pontos:** É calculada com base na dificuldade do jogo e no tempo (em segundos) que o jogador levou para resolvê-lo. A fórmula usada para o cálculo é a seguinte:

```bash
Pontuação = 1285 + (97418 × (dificuldade + 1)) ÷ tempo
```
