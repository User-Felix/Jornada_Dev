Um ***array*** em JavaScript é uma estrutura de dados usada para armazenar múltiplos valores em uma única variável. É como uma lista onde cada elemento pode ser acessado por sua posição, chamada de índice. **Arrays** são muito úteis para organizar e manipular coleções de dados.

Características Básicas:

Índices:

- Os elementos de um array são organizados em índices numéricos que começam em 0.

- Exemplo:
```js
    let frutas = ["maçã", "banana", "laranja"];
    console.log(frutas[0]); // "maçã" (primeiro elemento)
    console.log(frutas[1]); // "banana" (segundo elemento)
    console.log(frutas[2]); // "laranja" (terceiro elemento)
```
Comprimento do Array:

A propriedade **.length** retorna o número total de elementos no array.
Exemplo:

```js
    console.log(frutas.length); // 3
    Tipos de Dados em Arrays:
```

Um array pode conter qualquer tipo de dado: números, strings, objetos, outros arrays, ou uma mistura de todos.

Exemplo:

```js
    let misto = [42, "texto", true, [1, 2, 3]];
    console.log(misto[3]); // [1, 2, 3]
    Como Criar Arrays
    Usando Colchetes [] (mais comum):
```

```js
let cores = ["azul", "vermelho", "verde"];
console.log(cores[1]); // "vermelho"
```

Modificar:

```js
cores[1] = "amarelo";
console.log(cores); // ["azul", "amarelo", "verde"]
```

Arrays Vazios:

Você pode criar um array vázio e adicionar elementos mais tarde.

```js
    let vazio = [];
    vazio[0] = "primeiro";
    vazio[1] = "segundo";
    console.log(vazio); // ["primeiro","segundo"]
```

Falaremos mais de arrays no próximo nível!