# Dia de Estudos em Programação
📅 21 de Outubro de 2025

## 📘 Tema
Estruturas de repetição em Python

## 🧾 Resumo rápido
O `while` é uma estrutura de repetição que executa um bloco de código enquanto a condição for verdadeira.

## 🧩 Explicação
- Usei o `print()` para criar um menu de opções.
- O `input()` coleta a escolha do usuário.
- Se a opção for `1`, o programa conta de 1 a 10.
- Se for `2`, usa `break` para encerrar o loop.
- Caso contrário, mostra uma mensagem de erro.

## ⚠️ Dificuldade
Entender quando usar o `break`.

## 💻 Código de exemplo
```python
while True:
    print('\nMenu')
    print('1 - Para ver o contador de 1 a 10.')
    print('2 - Para sair.')
    
    opcao = input('Digite uma opção: ')
    
    if opcao == '1':
        numero = 1
        while numero <= 10:
            print(numero)
            numero += 1
    elif opcao == '2':
        print('Encerrando...')
        break
    else:
        print('Opção inválida.')


