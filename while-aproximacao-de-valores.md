# 🧠 Dia de Estudos em Programação
📅 **Data:**  31 de Outubro de 2025 

---

## 📘 Tema
Aproximação de valores

---

## 🧾 Resumo rápido
Esse programa utiliza um loop `while` para controlar duas variáveis ao mesmo tempo (x e y).
A cada repetição, o valor de `x` aumenta e o de `y` diminui, até que a condição `x < 10 and y > 10` deixe de ser verdadeira.
No final, o programa exibe uma mensagem informando que o loop foi concluído e mostra os valores finais de `x` e `y`.

---

## 🧩 Explicação passo a passo
- x, y = 5, 15
👉 Define duas variáveis ao mesmo tempo:
x começa com o valor 5 e y com o valor 15.
- while x < 10 and y > 10:
  👉 Inicia o loop while que só vai continuar enquanto as duas condições forem verdadeiras:
    x for menor que 10
    y for maior que 10
    Assim que uma delas for falsa, o loop termina.
- print(f'X: {x}, Y: {y}')
  👉 Mostra na tela o valor atual de x e y em cada repetição.
- x += 1
  👉 Aumenta o valor de x em 1 a cada volta do loop.
- y -= 1
  👉 Diminui o valor de y em 1 a cada volta do loop.
  Quando uma das condições do while não for mais verdadeira (x chegar a 10 ou y cair para 10), o loop termina.
- print('Loop concluído!')
  👉 Exibe uma mensagem informando que o laço foi finalizado.
- print(f'Valores finais - x: {x}, y: {y}')
  👉 Mostra os valores finais de x e y depois que o loop terminou.

---

## ⚠️ Dificuldades ou dúvidas
Também foi importante compreender a função dos operadores += e -=, que são usados para incrementar e decrementar os valores das variáveis dentro do loop.
Depois que isso ficou claro, o raciocínio ficou mais simples e o código funcionou exatamente como esperado.

---

## 💻 Código de exemplo
x, y = 5, 15

while x < 10 and y > 10:
    print(f'X: {x}, Y: {y}')

    x += 1
    y -= 1

print('Loop concluido!')
print(f'Valores finais - x: {x}, y: {y}')

```
## 💬 Reflexão pessoal
Gostei muito de aprender esse código, porque ele abriu mais a minha mente e me fez perceber que posso usar duas variáveis na mesma linha de código.
Isso me ajudou a entender melhor como o Python permite trabalhar com várias condições ao mesmo tempo, deixando o código mais dinâmico e eficiente. 
