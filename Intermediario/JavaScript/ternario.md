# **Operador Ternário**

O **operador ternário** é uma ferramenta poderosa e concisa em JavaScript para tomar decisões em uma única linha de código. Ele é amplamente utilizado para simplificar instruções condicionais, substituindo blocos `if-else` em situações mais simples.

---

### **Sintaxe Básica:**
```javascript
    condição ? valorSeVerdadeiro : valorSeFalso
```
- **`condição`:** Uma expressão que retorna `true` ou `false`.
- **`valorSeVerdadeiro`:** O que é retornado se a condição for verdadeira.
- **`valorSeFalso`:** O que é retornado se a condição for falsa.

---

## **Por que usar o Operador Ternário?**

- **Conciso:** Reduz linhas de código em comparação com `if-else`.
- **Legibilidade:** Em casos simples, torna o código mais claro.
- **Flexibilidade:** Pode ser usado em expressões, atribuições ou até dentro de templates literais.

---

## **Exemplo Básico**

Imagine que você quer verificar se uma pessoa é maior de idade:

### **Com if-else:**
```javascript
let idade = 20;
let mensagem;

if (idade >= 18) {
    mensagem = "Maior de idade";
} else {
    mensagem = "Menor de idade";
}
console.log(mensagem); // "Maior de idade"
```

### **Com operador ternário:**
```javascript
let idade = 20;
let mensagem = idade >= 18 ? "Maior de idade" : "Menor de idade";
console.log(mensagem); // "Maior de idade"
```

O ternário faz o mesmo trabalho em uma única linha!

---
