# 📘 Atividade: Jogo da Forca

## 🎯 Objetivo

Pratique strings, laços, condicionais e seleção aleatória criando um jogo da forca em Python. O jogador deve descobrir uma palavra antes de esgotar as tentativas disponíveis.

## 📝 Tarefas

### 🛠️ Implementar a Lógica Principal do Jogo

#### Descrição

Complete a lógica principal usando a lista de palavras e os espaços indicados no código inicial. Selecione uma palavra aleatoriamente e permita que o jogador tente descobri-la.

#### Requisitos

O programa concluído deve:

- Selecionar aleatoriamente uma palavra da lista predefinida.
- Exibir o progresso da palavra com letras adivinhadas e espaços para as letras restantes.
- Contar e exibir as tentativas incorretas restantes.
- Encerrar quando a palavra for descoberta ou quando as tentativas acabarem, informando vitória ou derrota.

### 🛠️ Validar Palpites e Melhorar o Feedback

#### Descrição

Trate entradas inválidas ou repetidas para que o jogo responda de forma clara e mantenha o estado corretamente durante cada rodada.

#### Requisitos

O programa concluído deve:

- Aceitar apenas um palpite de letra por vez e ignorar entradas inválidas sem descontar uma tentativa.
- Informar quando uma letra já tiver sido escolhida, sem descontar uma tentativa.
- Mostrar as letras já tentadas e indicar se cada novo palpite está ou não na palavra.