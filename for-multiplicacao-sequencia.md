# 🧠 Dia de Estudos em Programação
📅 **Data:**  11 de Novembro de 2025 

---

## 📘 Tema
Estrutura de repetição `for` — multiplicação sequencial de números (1 a 5).

---

## 🧾 Resumo rápido
Neste estudo, criei um programa usando o laço `for` para multiplicar todos os números de **1 a 5**, acumulando o resultado em uma variável chamada `resultado`.  
Esse tipo de lógica é útil para entender **acumuladores**, **variação de valores dentro do loop** e **cálculo de fatorial**, já que multiplicar 1×2×3×4×5 gera o valor 120.

---

## 🧩 Explicação passo a passo
- A variável `resultado` começa com o valor **1**, pois será usada para multiplicação.
- O `for` percorre a sequência de números de **1 até 5** (`range(1, 6)`).
- Em cada repetição, `resultado` é multiplicado pelo valor atual de `numero`.
- O programa mostra o resultado parcial a cada ciclo.
- No final, imprime o resultado total da multiplicação.

---

## ⚠️ Dificuldades ou dúvidas
Não estava conseguindo achar a lógica no começo, porque eu achava que não precisava criar a variável `resultado` para que o cálculo final fizesse sentido.  
Depois percebi que a variável acumuladora é essencial para armazenar a multiplicação parcial e chegar ao valor final corretamente.

---

## 💻 Código de exemplo
```python
resultado = 1

for numero in range(1, 6):
    resultado *= numero
    print(f'Multiplicando por {numero}, o resultado parcial é {resultado}')

print(f'O resultado final da multiplicação é {resultado}')


```
## 💬 Reflexão pessoal
Olhando esse código, parece ser simples — mas para mim não foi.  
Quebrei a cabeça por algumas horas para conseguir chegar no resultado final.  
A minha maior dificuldade foi entender que eu realmente precisava da variável `resultado` para armazenar o valor parcial e conseguir multiplicar pelo número atual dentro do loop.  
Depois que entendi esse raciocínio, tudo fez sentido.


