
# 📘 Assignment: Hangman Game

## 🎯 Objective

Pratique strings, laços, condicionais e seleção aleatória criando um jogo da Forca em Python. O jogador deve descobrir uma palavra antes de esgotar as tentativas disponíveis.

## 📝 Tasks

### 🛠️ Implement the Core Game

#### Description

Complete a lógica principal do jogo usando a lista de palavras e os espaços indicados no código inicial.

#### Requirements

O programa concluído deve:

- Selecionar aleatoriamente uma palavra da lista predefinida.
- Exibir o progresso da palavra com letras adivinhadas e espaços para as letras restantes.
- Contar e exibir as tentativas incorretas restantes.
- Encerrar quando a palavra for descoberta ou quando as tentativas acabarem, informando vitória ou derrota.

### 🛠️ Validate Guesses and Improve Feedback

#### Description

Trate entradas inválidas ou repetidas para que o jogo responda de forma clara e mantenha o estado corretamente.

#### Requirements

O programa concluído deve:

- Aceitar apenas um palpite de letra por vez e ignorar entradas inválidas sem descontar uma tentativa.
- Informar quando uma letra já tiver sido escolhida, sem descontar uma tentativa.
- Mostrar as letras já tentadas e indicar se cada novo palpite está ou não na palavra.