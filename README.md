
# Sudoku Game

<div align="center">

[Sobre](#sobre) • [Tecnologias](#tecnologias-utilizadas) • [Funcionalidades](#funcionalidades) • [Pré requisitos](#pré-requisitos) • [Execução](#como-executar)

</div>

## Sobre 
Este projeto foi desenvolvido como parte da disciplina de Laboratório de Programação do curso de Ciência da Computação da [Universidade Federal de Santa Maria](https://www.ufsm.br/). 

- O objetivo principal é criar um jogo de tabuleiro **Sudoku** utilizando a biblioteca Allegro 5, O projeto explora as funcionalidades gráficas da biblioteca para criar uma interface visual interativa e aprimorar a experiência do usuário. O jogo apresenta tabuleiros variados, selecionados aleatoriamente a partir de uma base de 100 tabuleiros, cada um com um nível de dificuldade diferente.

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
## Pré requisitos
- Sistema Operacional:

Linux: qualquer distribuição compatível.

Windows: deve ter o WSL (Windows Subsystem for Linux) instalado. [Guia de instalação do WSL.](https://learn.microsoft.com/pt-br/windows/wsl/install)

- Biblioteca Allegro 5:

A versão 5.2.9.1 ou superior é necessária para rodar este projeto.
Certifique-se de que essa versão está instalada, seguindo as instruções descritas na seção de [Instalação Allegro 5.](https://github.com/Thalisson-Souza/Jogo-da-Velha-com-Allegro-5/blob/main/Instala%C3%A7%C3%A3o-Allegro5.md)

## Licença

Este projeto está licenciado sob a [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Thalisson-Souza/Sudoko-Game/blob/main/LICENSE)
