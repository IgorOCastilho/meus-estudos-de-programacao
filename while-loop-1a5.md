# 🧠 Dia de Estudos em Programação
📅 **Data:** 24 de Outubro de 2025 

---

## 📘 Tema
Contador com Parada Automática

---

## 🧾 Resumo rápido 
Esse programa cria um contador simples de 1 até 100, utilizando um laço while.
Durante a execução, ele imprime cada número na tela, mas foi configurado para parar automaticamente quando o número chegar a 5, usando o comando break.

---

## 🧩 Explicação passo a passo
- Variável `numero` recebe 1  
- `while` Continua o loop enquanto o número for menor que 100.  
- Incrementa `numero` em 1 para próxima iteração, se a condição acima não for verdadeira.  
- `if` Verifique se o número é igual a 5.
- `break` Se o número for 5 sai do loop imediatamente  

---

## ⚠️ Dificuldades ou dúvidas
- Entender quando usar `break` e `continue`.

---

## 💻 Código de exemplo
```python
numero = 1 
while numero < 100: 
    print(numero)
    numero += 1 
    if numero == 5: 
        print(numero)
        break 

```
## 💬 Reflexão pessoal

Hoje entendi melhor como o while funciona.
Antes eu achava que ele era parecido com o for, mas agora percebo que o while é melhor quando não sei quantas vezes quero repetir algo.
Gostei de ver o programa funcionando com break, e percebi que pequenos erros de indentação causam grandes problemas.
