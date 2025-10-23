# Dia de Estudos em Programação

## 📅 21 de Outubro de 2025
**Tema:** Estruturas de repetição em Python  
**O que aprendi:** while, break, continue, laços aninhados  
**Código de exemplo:**
```python

## Explicação: 
## Nesse programa eu uso essa estrutura de controle ‘while’, que faz um loop a onde eu posso fazer uma sequência com o número que define.
## Usando o ‘print()’ para imprimir na tela os texto ou strig que escrevi, como MENU, PARA VER O CONTADOR e PARA SAIR.
## Depois utilizo a função ‘input()’ para pedir ao usuário que DIGITE UMA OPCAO.
## Ao passar a opção para o programa, ele usa outra função ‘if’ que pergunta: se a opção for  igual a 1, defina o contador de 1 a 10.
## Se a opção for igual a 2, defina encerrando.
## E se o usuário acabar digitando qualquer coisa que não seja o que o programa está pedindo ele manda uma mensagem de erro.
## E o ‘break’ é uma instrução que encerra imediatamente o loop, com o (for ou while).

## Dificuldade: Entender quando usar break

while True:
    print('/n Menu')
    print('1 - Para ver o contador de 1 a 10. ')
    print('2 - Para sair. ')

    opcao = input('Digite uma opção: ')

    if opcao == '1':
        numero = 1
        while numero < 11:
            print(numero)
            numero += 1
    elif opcao == '2':
        print('Encerrando...')
        break
    else:
        print('Algo errado tente novamente! ')

