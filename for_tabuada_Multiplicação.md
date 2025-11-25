# 🧠 Dia de Estudos em Programação
📅 **Data:** 25 de Novembro de 2025

---

## 📘 Tema
Estrutura de repetição `for` — criação de uma tabuada de multiplicação em Python.

---

## 🧾 Resumo rápido
Neste exercício, usei o `for` para criar uma **tabuada de multiplicação**.  
O programa pede ao usuário um número e, em seguida, mostra todos os resultados de `0` até `10`, multiplicando o número escolhido por cada valor do intervalo.

---

## 🧩 Explicação passo a passo
- O programa começa exibindo o título da tabuada com `print()`.
- O usuário digita um número inteiro.
- O laço `for` percorre um intervalo de `0` até `10` usando `range(11)`.
- Em cada repetição, o valor atual (`i`) é multiplicado pelo número digitado.
- O resultado é exibido formatado com `f-string`.
- Ao final, o programa mostra uma mensagem de encerramento.

---

## ⚠️ Dificuldades ou dúvidasMinha dificuldade aconteceu porque eu usei a mesma variável numero dentro do loop for, assim: for numero in range(11):.
Isso acabou invertendo a lógica do programa, e a tabuada não saía como eu queria — o valor em sequência ficava do lado esquerdo, e eu não conseguia entender o porquê.
Depois percebi que estava sobrescrevendo a variável que guardava o número digitado pelo usuário.

---

## 💻 Código de exemplo
```python
print('\n¨¨TABUADA DE MULTIPLICAÇÃO¨¨\n')

numero = int(input('Digite um número inteiro: '))

for i in range(11):
    print(f'{numero} * {i} = {i * numero}')

print('\nFim da tabuada.')

```
## 💬 Reflexão pessoal

Hoje eu percebi como uma coisa simples pode mudar totalmente o funcionamento do meu código.
Eu estava usando a mesma variável numero dentro do for (for numero in range(11):), e isso estava invertendo a lógica da tabuada sem eu entender o porquê.

Fiquei confuso no começo, porque o resultado não aparecia do jeito que eu queria e eu não conseguia encontrar o erro.
Depois que percebi que a variável do loop estava substituindo o número digitado pelo usuário, tudo fez sentido.

No final, foi bom quebrar a cabeça um pouco, porque isso me ajudou a entender melhor como as variáveis funcionam dentro de loops em Python.
