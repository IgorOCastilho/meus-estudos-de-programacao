# 🧠 Dia de Estudos em Programação
📅 **Data:**  29 de Outubro de 2025 

---

## 📘 Tema
Calculadora Simples

---

## 🧾 Resumo rápido  
Esse programa realiza cálculos automáticos de adição (+), subtração (-), multiplicação (*) e divisão (/).
Foi desenvolvido de forma simples para praticar o uso das estruturas condicionais if, elif e else, que controlam as operações escolhidas pelo usuário.

---

## 🧩 Explicação passo a passo
- while True: cria um loop infinito que mantém o menu em execução até o usuário escolher sair.
- print(...) exibe o menu de opções com as operações disponíveis.
- input(...) lê a opção digitada pelo usuário.
- if / elif / else determinam qual operação será executada (adição, subtração, multiplicação ou divisão).
- No caso da divisão, o código verifica se o divisor é diferente de zero para evitar erro.
- break encerra o loop quando o usuário escolhe a opção “Sair”.  

---

## ⚠️ Dificuldades ou dúvidas
Durante o desenvolvimento, a principal dificuldade foi lembrar de tratar a divisão por zero.
No início, o programa funcionava, mas apresentava erro quando o usuário digitava 0 como divisor.
Depois de entender melhor a lógica, foi possível resolver adicionando uma condição if num2 != 0.

Também precisei reforçar o entendimento sobre o uso do try e except, que evita travamento e trata erros de digitação.

---

## 💻 Código de exemplo
```python
# Calculadora Simples
while True:
    print('\n=====  Calculadora Simples =====')
    print('''      
    1 - Adição
    2 - Subtração
    3 - Multiplicação
    4 - Divisão
    5 - Sair
    ''')

    try:
        opcao = int(input('Digite uma das opções acima (1-5): '))
    except ValueError:
        print(' Por favor, digite apenas números!')
        continue

    if opcao == 5:
        print('Encerrando a calculadora... ')
        break

    elif opcao == 1:
        num1 = int(input('Digite o primeiro número: '))
        num2 = int(input('Digite o segundo número: '))
        print(f'Resultado: {num1} + {num2} = {num1 + num2}')

    elif opcao == 2:
        num1 = int(input('Digite o primeiro número: '))
        num2 = int(input('Digite o segundo número: '))
        print(f'Resultado: {num1} - {num2} = {num1 - num2}')

        if num1 < num2:
            print(f'''
 O número negativo indica que o segundo valor ({num2}) 
é maior que o primeiro ({num1}), resultando em valor negativo.
            ''')

    elif opcao == 3:
        num1 = int(input('Digite o primeiro número: '))
        num2 = int(input('Digite o segundo número: '))
        print(f'Resultado: {num1} * {num2} = {num1 * num2}')

    elif opcao == 4:
        num1 = int(input('Digite o primeiro número: '))
        num2 = int(input('Digite o segundo número: '))

        if num2 != 0:
            resultado = num1 / num2
            print(f'Resultado: {num1} / {num2} = {resultado:.2f}')
        else:
            print(' Erro: não é possível dividir por zero!')

    else:
        print(' Opção inválida. Tente novamente!')


```
## 💬 Reflexão pessoal

Ao fazer esse projeto, consegui praticar o uso de condicionais e loops, reforçando o quanto é importante planejar o código antes de começar a digitar.
Percebi que quanto mais eu organizo a lógica, mais fácil fica encontrar erros e corrigir.
Foi um exercício simples, mas muito útil para entender como um programa pode tomar decisões diferentes com base na escolha do usuário.
