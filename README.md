
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

- **Inserção de Nome:** O jogador insere seu nome no início do jogo, o que permite o registro de pontos e a consulta posterior.

- **Registro de Pontos:** Ao completar o tabuleiro, o jogo verifica se o nome do jogador já está presente no arquivo de pontuação:

  - Acúmulo de Pontos: Se o jogador já tiver completado o mesmo tabuleiro anteriormente, os pontos são acumulados com os registrados anteriormente.
  - Novo Registro por Tabuleiro: Se o jogador completar um tabuleiro diferente, um novo registro de pontos é criado com a identificação do novo tabuleiro e sua respectiva pontuação.

- **Cálculo de Pontos:** É calculada com base na dificuldade do jogo e no tempo (em segundos) que o jogador levou para resolvê-lo. A fórmula usada para o cálculo é a seguinte:

```bash
Pontuação = 1285 + (97418 × (dificuldade + 1)) ÷ tempo
```
