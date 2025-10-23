# 🧠 Dia de Estudos em Programação
📅 **Data:** 23 de Outubro de 2025

---

## 📘 Tema
Estrutura de repetição while — comparação de valores para encontrar o maior número digitado pelo usuário.

---

## 🧾 Resumo rápido 
Neste exercício, usei um laço while para criar um programa que identifica o maior número digitado pelo usuário.
O programa continua pedindo novos números até que o usuário digite 0, que encerra o loop.
Durante cada repetição, o programa compara o número atual com o maior número armazenado até o momento e atualiza o valor quando encontra um número maior.

---

## 🧩 Explicação passo a passo
- Começa com numero = 0 — o valor inicial que será comparado.
- O usuário digita um número.
- Enquanto ele não digitar 0, o programa continua rodando.
- Se o número digitado for maior que o anterior, ele é salvo em numero.
- Quando o usuário digita 0, o loop para, e o programa mostra o maior número digitado. 

---

## ⚠️ Dificuldades ou dúvidas  
- Minha dificuldade foi entender a lógica da comparação — como fazer o programa descobrir qual número digitado era o maior.
  
---

## 💻 Código de exemplo
<!-- Coloque um exemplo completo -->
```python
numero = 0

usuario = int(input('Digite um número para saber o maior número digitado: '))

while usuario != 0:
    if usuario > numero:
        numero = usuario    
    usuario = int(input('Digite outro número (ou 0 para sair): '))

print('O maior número digitado foi:', numero)


---
```
💬 Reflexão pessoal
Hoje fiquei quase uma hora quebrando a cabeça, mas consegui resolver algo que parecia difícil 😅.
No final valeu a pena, porque consegui fazer meu código funcionar direitinho!
