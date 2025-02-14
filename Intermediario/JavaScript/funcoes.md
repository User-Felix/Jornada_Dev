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

### Usando function dentro de Arrays:

Podemos guardar uma função em um array para chamar ela de dentro do array?

Sim, isso é útil quando você deseja criar um conjunto de funções reutilizáveis e acessá-las dinamicamente, podemos até substituir o uso do if e switch case.

Você pode armazenar funções em um array e chamá-las através do índice do array:



```javascript
    // Definindo algumas funções
    function saudacao() {
        console.log("Olá!");
    }

    function despedida() {
        console.log("Tchau!");
    }

    function olaNome(nome) {
        console.log(`Olá, ${nome}!`);
    }

    // Criando um array de funções
    const funcoes = [saudacao, despedida, olaNome];

    // Chamando funções pelo índice
    funcoes[0](); // Executa saudacao(), imprime "Olá!"
    funcoes[1](); // Executa despedida(), imprime "Tchau!"
    funcoes[2]("Wendy"); // Imprime "Olá, Wendy"
```

### Usando arrow functions diretamente no array:


```javascript
    const funcoes = [
        () => console.log("Função 1"),
        () => console.log("Função 2"),
        (nome) => console.log(`Olá, ${nome}!`)
    ];

    funcoes[0](); // Imprime "Função 1"
    funcoes[1](); // Imprime "Função 2"
    funcoes[2]("Maria"); // Imprime "Olá, Maria!"
```
### Trocando o If e o Switch case:

No exemplo a função simples chamada convertToHex que converte uma determinada cor (representada por uma string) em seu equivalente hexadecimal.

Font: Roger Melo

```javascript

    const convertToHex = color => {
        const colors = {
            red: '#A31419',
            green: '#18A337',
            blue: '#4C91F0',
            yellow: '#F0EA6F',
            purple: '#8132A3'
        }

        return colors[color] 
            ? `O hexadecimal para a cor ${color} é ${colors[color]}` 
            : `Não temos o equivalente hexadecimal para ${color}`; 
    }

    const colors = ['red','green','blue','yellow','purple']

    console.log(convertToHex('blue'))

```