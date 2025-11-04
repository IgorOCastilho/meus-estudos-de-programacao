# 🧠 Dia de Estudos em Programação
📅 **Data:**  04 de Novembro de 2025 

---

## 📘 Tema
Estrutura de repetição `while` — jogo de adivinhação com dois números secretos.

---

## 🧾 Resumo rápido
Neste exercício, criei um jogo em Python que utiliza a estrutura `while` com **condições compostas** (`and` e `or`).  
O jogador precisa adivinhar **dois números secretos**, tendo **cinco tentativas**.  
O loop continua enquanto o jogador ainda tiver tentativas **e** não tiver acertado os dois números.  
Durante o jogo, o programa informa se cada número foi adivinhado e quantas tentativas restam.

---

## 🧩 Explicação passo a passo
- Foram criadas duas variáveis: `numeroSecreto1` e `numeroSecreto2`, com valores fixos.
- O programa controla o número de tentativas com `tentativas = 5`.
- Duas variáveis booleanas (`adivinhou1` e `adivinhou2`) guardam se o jogador já acertou ou não.
- O laço `while` repete o jogo enquanto:
  - ainda houver tentativas (`tentativas > 0`),  
  - e o jogador não tiver acertado os dois números.
- Cada tentativa compara o palpite com os números secretos.
- Se o jogador acerta um número, o programa marca a variável como `True`.
- O jogo termina quando o jogador acerta os dois ou as tentativas acabam.

---

## ⚠️ Dificuldades ou dúvidas
Ao fazer o código, tive dificuldade em entender a lógica para usar `or`, `not` e `and` de forma que o programa fizesse sentido.  
Minha maior dificuldade foi nesta parte:  
`while tentativas > 0 and (not adivinhou1 == True or not adivinhou2 == True)`  
Mas no final deu certo e o código funcionou como eu queria!

---

## 💻 Código de exemplo
```python
numeroSecreto1 = 7
numeroSecreto2 = 3

tentativas = 5

adivinhou1 = False
adivinhou2 = False

# Continua o loop enquanto ainda houver tentativas
# e o jogador não tiver adivinhado os dois números
while tentativas > 0 and (not adivinhou1 == True or not adivinhou2 == True):
    print(f'Tentativas restantes: {tentativas}')

    palpite1 = int(input('Adivinhe o primeiro número secreto (1-10): '))
    palpite2 = int(input('Adivinhe o segundo número secreto (1-10): '))

    if palpite1 == numeroSecreto1:
        print('Você adivinhou o primeiro número!')

        adivinhou1 = True

    if palpite2 == numeroSecreto2:
        print('Você adivinhou o segundo número!')

        adivinhou2 = True

    if not adivinhou1 == True or not adivinhou2 == True:
        print('Tente novamente. ')

        tentativas -= 1

if adivinhou1 == True and adivinhou2 == True:
    print('Parabéns, você adivinhou ambos os números!')

else:
    print(f'Você não conseguiu adivinhar os números. Eles eram {numeroSecreto1} e {numeroSecreto2}')

```
## 💬 Reflexão pessoal
Hoje fiquei quase uma hora pensando e quebrando a cabeça, mas consegui resolver algo que parecia difícil kkk 😅.
No final valeu a pena, porque consegui fazer o jogo funcionar direitinho e entender melhor o uso de and e or dentro do while.
