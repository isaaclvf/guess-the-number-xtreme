# Relatório do Jogo de Adivinhação com Circuitos Lógicos Digitais no Logisim

## Introdução:
Este relatório descreve o projeto de um jogo de adivinhação desenvolvido usando circuitos lógicos digitais no programa Logisim. O jogo foi criado com o objetivo de ensinar conceitos de circuitos sequenciais, incluindo máquinas de estados, elementos de memória e manipulação de números binários. O jogo é projetado para ser jogado por dois jogadores, que se alternam dando palpites para adivinhar um número secreto.

## Objetivo
O principal objetivo deste projeto é proporcionar um ambiente prático para aprender e aplicar conceitos de circuitos lógicos sequenciais. Esse projeto depende de elementos-chave dessa disciplina, como máquinas de estados, elementos de memória, conversão de números binários e lógica de controle.

## Componentes

### Cronômetro

!["Cronômetro"](/img/cronometro.gif "Cronômetro")

O jogo é controlado por um cronômetro que mantém o tempo disponível para cada jogador. Cada jogador tem um limite de tempo para fazer seus palpites. Quando o tempo de um jogador esgotar, ele é impedido de continuar fazendo chutes.

O cronômetro é composto por outros circuitos menores encadeados, que representam as unidades e dezenas de medida de tempo.

!["Circuito que representa unidades de tempo"](/img/unidade.png "Circuito que representa unidades de tempo")

### Circuito Core

!["Circuito core"](/img/core.gif)

Este circuito contém a lógica principal do jogo. Ele recebe os palpites dos jogadores, compara-os com o número secreto e decide se os palpites estão corretos ou não. O circuito também controla a lógica do jogo, alternando entre os jogadores e atualizando o placar.

### Placar

!["Placar do jogo"](/img/placar.png "Placar do jogo")

O placar é responsável por manter um registro da pontuação dos jogadores A e B. Cada vez que um jogador acerta o palpite, seu placar é incrementado. O jogo termina quando um dos jogadores alcança 15 pontos.

### Conversor de Números

![Conversor de números sem sinalização](/img/sinal.png "Conversor de números sem sinalização")

 Este circuito é usado para converter números de 4 bits sem sinalização de negativo em números de 4 bits, onde o primeiro bit indica o sinal (positivo ou negativo). Isso é útil para representar os palpites dos jogadores e o número secreto.

## Funcionamento

![Funcionamento do jogo principal](/img/main.gif "Funcionamento do jogo principal")

- No início do jogo, o número secreto é gerado aleatoriamente e é mantido oculto.
- Os jogadores A e B se alternam dando palpites para os valores de X e Y. Eles usam o conversor de números para fornecer seus palpites em formato binário de 4 bits.
- O circuito core compara os palpites dos jogadores com o número secreto. Se um jogador acertar o palpite, seu placar é incrementado.
- O jogo continua até que um dos jogadores alcance 15 pontos ou quando o tempo disponível para ambos os jogadores se esgotar.
- Quando o jogo termina, é exibida uma mensagem indicando o vencedor ou se o jogo terminou em empate.

## Conclusão
Este projeto educacional de um jogo de adivinhação com circuitos lógicos digitais no Logisim é uma maneira eficaz de ensinar conceitos importantes de circuitos sequenciais, como máquinas de estados e elementos de memória. Além disso, ele envolve a conversão de números binários e operações lógicas, proporcionando aos alunos uma experiência prática e interativa de aprendizado. Esse jogo não apenas demonstra a aplicação dos princípios teóricos, mas também torna o processo de aprendizado mais envolvente e divertido para os alunos.