
Um **array** é uma estrutura de dados que pode armazenar vários valores em uma única variável como já falamos no nivel iniciante. Agora vamos aprender a fazer iterações.

***Exemplo:***
```javascript
    const frutas = ["Maçã", "Banana", "Laranja"];
    console.log(frutas); // ["Maçã", "Banana", "Laranja"]
```

Vamos começar criando o array:

```js
   const numeros = [1, 2, 3, 4, 5]; 
```

Acessando elementos:

```js
    const numeros = [1, 2, 3, 4, 5];
    for (let i = 0; i < numeros.length; i++) {
        console.log(numeros[i]);
    }
```

***For...in***
O laço for...in é usado para iterar sobre as chaves de um objeto.
Ele percorre todas as propriedades enumeráveis do objeto, incluindo aquelas herdadas do protótipo, se não forem filtradas.


```js
    const numeros = [1, 2, 3, 4, 5];
    for (const i in numeros) {
        console.log(i, numeros[i]); // Imprime índices como strings: '0', '1', '2'
    }

```

***For...of***

O laço for...of é uma maneira simples de iterar diretamente pelos valores do array.
Ele não dá acesso ao índice, apenas ao valor de cada elemento.


```js
    for (const numero of numeros) {
    console.log(numero);
}

```

***ForEach()***

O método forEach executa uma função callback para cada elemento do array.
A função recebe o valor do elemento como argumento (e opcionalmente o índice e o próprio array).
Ele executa ações específicas em cada elemento.

```js
    numeros.forEach((numero) => {
        console.log(numero);
    });
```

***Map()***

O método map cria um novo array aplicando a função callback a cada elemento.
O array original permanece inalterado.

Útil para transformar os elementos do array.


```js
    const numeros = [1, 2, 3, 4, 5];
    const dobro = numeros.map(num => num * 2);
    console.log(dobro); // [2, 4, 6, 8]

```

***Filter()***

O método filter cria um novo array contendo apenas os elementos que passam no teste fornecido pela função callback.
A função callback retorna true para incluir o elemento no novo array e false para excluí-lo.

```js
  const numeros = [1, 2, 3, 4, 5];
    const pares = numeros.filter(num => num % 2 === 0);
    console.log(pares); // [2, 4]  
```

***Reduce()***

O método reduce aplica uma função acumuladora a cada elemento do array, resultando em um único valor.
Recebe dois argumentos principais:
O acumulador (acc), que armazena o valor acumulado.
O elemento atual (num).
Um valor inicial (neste caso, 0) pode ser fornecido como o segundo argumento.

```js
    const numeros = [1, 2, 3, 4, 5];
    const soma = numeros.reduce((acc, num) => acc + num, 0);
    console.log(soma); // 10
```


***Métodos para Ordenar e Buscar***

***find()***

Retorna o primeiro elemento que passa em um teste.

```js
    const numeros = [1, 2, 3, 4];
    const maiorQueDois = numeros.find(num => num > 2);
    console.log(maiorQueDois); // 3

```

***findIndex()***

Retorna o índice do primeiro elemento que passa no teste.

```js
    const numeros = [1, 2, 3, 4];
    const indice = numeros.findIndex(num => num > 2);
    console.log(indice); // 2
```

***sort()***

O método permite ordenar os elementos de um array.

```js
    const numeros = [4, 2, 5, 1, 3];
    numeros.sort((a, b) => a - b); // Crescente
    console.log(numeros); // [1, 2, 3, 4, 5]

```