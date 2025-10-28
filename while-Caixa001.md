# 🧠 Dia de Estudos em Programação
📅 **Data:**  28 de Outubro de 2025 

---

## 📘 Tema
💰 Simulador de Caixa Eletrônico

---

## 🧾 Resumo rápido
Foi desenvolvido um programa de simulação de caixa eletrônico em Python, utilizando o operador while para criar um loop interativo com o usuário.
O menu apresenta quatro opções principais:
Verificar Saldo
Depositar Dinheiro
Sacar Dinheiro
Sair
O programa repete as opções até o usuário escolher sair, aplicando estruturas condicionais (if, elif, else) para tratar cada operação. Ele também realiza atualizações no saldo conforme depósitos e saques são feitos, simulando o funcionamento básico de um caixa eletrônico real.

---

## 🧩 Explicação passo a passo
- while True: inicia um loop infinito que mantém o menu rodando até o usuário escolher sair.
- print(...) exibe o menu de opções para o usuário.
- input(...) lê a escolha do usuário; em seguida você converte para número com int(...) para poder comparar.
- if / elif / else são as condicionais que tratam cada operação do menu (ver saldo, depósito, saque, sair) e também entradas inválidas.
- Atualizações de saldo:
- depósito: saldo += deposito
- saque: saldo -= saque (apenas se houver saldo suficiente)
- break encerra o loop quando a opção “Sair” é escolhida.
- (Opcional, mas recomendado) try/except trata erros de digitação (ex.: letra quando se espera número).

🔧 Pontos de melhoria rapidinhos
- Validar entrada: usar try/except para opcao, deposito e saque.
- Regras de negócio: impedir depósito ≤ 0 e saque ≤ 0 ou maior que o saldo.
- Formatação: mostrar valores com duas casas decimais ({saldo:.2f}).

---

## ⚠️ Dificuldades ou dúvidas
Durante a criação do programa, a principal dificuldade foi entender como atualizar o valor do saldo após depósitos e saques.
No início, o código realizava as operações, mas o valor não era armazenado corretamente — até compreender que era necessário usar o operador de atribuição (+= e -=) para somar ou subtrair diretamente da variável saldo.

---

## 💻 Código de exemplo
```python
saldo = 1000.00

while True:
    print('\n=====  Caixa Eletrônico =====')
    print('''
    1 - Verificar Saldo 
    2 - Depositar Dinheiro
    3 - Sacar Dinheiro
    4 - Sair
    ''')

    try:
        opcao = int(input('Digite uma das opções acima (1-4): '))
    except ValueError:
        print(' Digite apenas números!')
        continue

    if opcao == 1:
        print(f'Seu saldo atual é de R$ {saldo:.2f}.')

    elif opcao == 2:
        deposito = float(input('Quanto gostaria de depositar? R$ '))
        if deposito > 0:
            saldo += deposito
            print(f' Depósito de R$ {deposito:.2f} realizado com sucesso.')
            print(f'Saldo atual: R$ {saldo:.2f}')
        else:
            print(' Valor inválido. O depósito deve ser maior que zero.')

    elif opcao == 3:
        saque = float(input('Qual o valor do saque? R$ '))
        if saque <= 0:
            print(' O valor do saque deve ser maior que zero.')
        elif saque > saldo:
            print(' Saque inválido! Saldo insuficiente.')
        else:
            saldo -= saque
            print(f' Saque de R$ {saque:.2f} realizado com sucesso.')
            print(f'Saldo restante: R$ {saldo:.2f}')

    elif opcao == 4:
        print(' Agradecemos por usar o Caixa Eletrônico. Até logo!')
        break

    else:
        print(' Opção inválida. Tente novamente.')

```
## 💬 Reflexão pessoal

Ao desenvolver esse código, consegui compreender melhor como utilizar o comando try / except.
Percebi que ele facilita bastante a lógica do programa, pois evita erros quando o usuário digita valores incorretos e permite tratar essas situações de forma mais controlada.
Isso me ajudou a entender que programar não é apenas fazer o código funcionar, mas também prever possíveis erros e garantir que o programa continue executando corretamente.

