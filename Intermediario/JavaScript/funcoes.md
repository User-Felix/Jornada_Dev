### Voltando a falar de funções


***O que são Arrow Functions?***

Arrow functions são uma sintaxe mais concisa e moderna para definir funções em JavaScript. Elas foram introduzidas no ES6 e são uma maneira elegante de escrever funções, especialmente quando se trata de funções curtas.


```js
    const NomeDaConstante (parâmetros) => { corpo da função };
```
Declaramos uma arrow functiom dessa forma:

```js
    const dobro = (x) => { x * 2 };
```
Porêm...
Podemos dar uma enxugada nela e escrever um pouco menos:
```js
    const dobro = x => x * 2;
```

Exemplo das duas funções:

```js
    // Função tradicional
    function soma(a, b) {
    return a + b;
    }

    // Arrow function equivalente
    const soma = (a, b) => a + b;
```


### Currying: Compondo Funções

Currying é uma técnica que permite **transformar uma função que recebe múltiplos argumentos em uma série de funções que recebem um argumento de cada vez**:

```js
    function somarCurried(x) {
        return function(y) {
            return x + y;
        };
    }

    let somar5 = somarCurried(5); // Retorna uma função que soma 5 a outro valor
    console.log(somar5(3)); // Exibe 8

```

O Currying **promove a composição de funções**, tornando o código mais modular e reutilizável.
