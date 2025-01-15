
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

**Como o forEach funciona:**
O forEach percorre cada elemento do array em ordem.

**Callback:** Para cada elemento, ele executa a função de callback que você fornece como argumento. Essa função define as ações a serem realizadas para cada item.


**Parâmetros da Função de Callback:** A função de callback pode receber até três parâmetros:

**item:** O elemento atual do array sendo iterado.

**index:** O índice (posição) do elemento atual no array.

**array:** O array completo sobre o qual o forEach está sendo executado.


```js
    const redesSociais = ["YouTube", "Twitter", "Instagram", "Facebook"];

    redesSociais.forEach((redeSocial, index, array) => {
        console.log(`Rede social ${index}: ${redeSocial}`);
        console.log(`Array completo: ${array}`);
    });

```

Neste exemplo, o forEach itera sobre o array redesSociais, executando a função de callback para cada elemento. A função de callback, por sua vez, imprime o nome da rede social, o seu índice e o array completo no console.

```js
    function exibirInfoRedeSocial(redeSocial, index, array) {
        console.log(`Rede social ${index}: ${redeSocial}`);
        console.log(`Array completo: ${array}`);
    }

    const redesSociais = ["YouTube", "Twitter", "Instagram", "Facebook"];

    redesSociais.forEach(exibirInfoRedeSocial);

```

Neste exemplo, a função exibirInfoRedeSocial é declarada separadamente e reutilizada no forEach.

O forEach é uma ferramenta poderosa para trabalhar com arrays em JavaScript, simplificando a iteração e incentivando um estilo de código mais limpo e funcional.

***Map()***

O método map em JavaScript é uma função de alta ordem que permite criar um novo array a partir de um array existente, transformando cada elemento do array original.


```js
    const numeros = [1, 2, 3, 4, 5];
    const dobro = numeros.map(num => num * 2);
    console.log(dobro); // [2, 4, 6, 8]

```

**O map é usado quando você precisa criar um novo array com a mesma quantidade de itens do array original, mas com cada item modificado de alguma forma.** Ele não modifica o array original.

**Como o map funciona:**

**Iteração:** O método map percorre cada elemento do array original.

**Transformação:** Para cada elemento, o map executa uma função que você fornece como argumento. Essa função recebe o elemento atual como parâmetro e retorna um novo valor transformado.

**Criação do Novo Array:** Os valores retornados pela função para cada elemento são usados para criar um novo array.

**Exemplo:**

```js
    const numeros = [1];

    const numerosAoQuadrado = numeros.map(numero => numero * numero);

    console.log(numerosAoQuadrado); // [1]

```

Neste exemplo, a `função numero => numero * numero` eleva cada número ao quadrado. O map aplica essa função a cada elemento do array numeros, resultando em um novo array numerosAoQuadrado com os valores transformados.

**Parâmetros da Função:**

A função passada para o map pode receber até três parâmetros:

**item:** O elemento atual do array sendo iterado. Este parâmetro é obrigatório.
**index:** O índice do elemento atual no array.

**array:** O array original sendo iterado.

**Exemplo com Desestruturação:**

```js
    const series = [
        { nome: "Série A", genero: "Drama" },
        { nome: "Série B", genero: "Comédia" },
    ];

    const nomesDasSeries = series.map(({ nome }) => nome);

    console.log(nomesDasSeries); // ["Série A", "Série B"]

```

Neste exemplo, a desestruturação `{ nome }` é usada para extrair o valor da propriedade nome de cada objeto no array series.

A função passada para o map **deve retornar um valor** para que o novo array seja criado corretamente.

O método map **não modifica o array original**. Ele cria um novo array com os valores transformados.

O map é uma ferramenta poderosa para manipular arrays em JavaScript, permitindo que você transforme dados de forma eficiente e concisa.

***Filter()***

O método filter cria um novo array contendo apenas os elementos que passam no teste fornecido pela função callback.
A função callback retorna true para incluir o elemento no novo array e false para excluí-lo.

```js
    const numeros = [1, 2, 3, 4, 5];
    const pares = numeros.filter(num => num % 2 === 0);
    console.log(pares); // [2, 4]  
```

O método filter em JavaScript é uma função de alta ordem que cria um novo array contendo apenas os elementos de um array original que satisfazem uma determinada condição.

**Exemplo:** Imagine que você tem uma lista de números aleatórios entre 0 e 100 e deseja criar uma nova lista contendo apenas os números maiores que 37.

**Declaração do array original:**

```js
    const numerosAleatorios = ["Maça","Banana","Manga"];

```

**Utilização do método filter:**

```js
    const numerosMaioresQue37 = numerosAleatorios.filter(function(numero) {
        return numero > 37;
    });

```

**Explicação:**

O método filter recebe uma função como argumento. Essa função é executada para cada elemento do array original.

A função passada para o filter deve retornar um valor booleano (true ou false).

Se a função retornar true para um determinado elemento, esse elemento será incluído no novo array.

Se a função retornar false, o elemento será ignorado.

**No exemplo acima:**

A função function(numero) { return numero > 37; } verifica se cada número no array numerosAleatorios é maior que 37.

Se o número for maior que 37, a função retorna true e o número é adicionado ao novo array numerosMaioresQue37.

Se o número não for maior que 37, a função retorna false e o número é ignorado.

**Resultado:**

O array numerosMaioresQue37 conterá apenas os números do array original que são maiores que 37.

**Observações:**

O método filter não modifica o array original. Ele retorna um novo array.

A função passada para o filter pode receber até três parâmetros: o elemento atual, o índice do elemento e o próprio array.

No exemplo acima, foi utilizado apenas o parâmetro do elemento atual (numero).

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
**Para entender o reduce, imagine que você tem uma cesta de frutas e quer saber o peso total.** O reduce percorreria cada fruta, somando o peso de cada uma à um valor acumulado, até chegar ao peso total da cesta.

**Veja como o reduce funciona passo a passo:**

**Função:** O reduce recebe uma função como argumento. Essa função é aplicada a cada elemento do array.

**Acumulador (accumulator)**: É um valor que "acumula" o resultado da função a cada iteração do array. Na analogia da cesta de frutas, o acumulador seria o peso total a cada fruta adicionada.

**Elemento atual (current element)**: É o elemento do array que está sendo processado na iteração atual.

**Valor inicial (initial value)**: É opcional. Define o valor inicial do acumulador. Se não for definido, o primeiro elemento do array é usado como valor inicial do acumulador.

**Exemplo da soma de números:**

```js
    const numbers = [1];

    const sum = numbers.reduce((accumulator, currentNumber) => accumulator + currentNumber, 0);

    console.log(sum); // Output: 6

```

A função reduce recebe uma função que soma o accumulator ao currentNumber.

O valor inicial do accumulator é definido como 0.

A cada iteração, a função soma o número atual ao accumulator.

No final, o sum armazena o valor final do accumulator, que é a soma de todos os números no array.


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

Imagine que você tem uma lista de livros e quer encontrar o primeiro livro escrito por um autor específico. O método find percorreria a lista de livros, um por um, verificando se o autor do livro corresponde ao autor que você está procurando. Assim que encontrar um livro que corresponda à condição, ele para a busca e retorna o livro.

**Veja como o find funciona passo a passo:**

**Condição:** O método find recebe uma função como argumento. Essa função define a condição que precisa ser satisfeita para encontrar o elemento desejado. 

**Iteração:** O find executa a função de condição para cada elemento do array, um de cada vez.

**Verificação:** A cada iteração, a função de condição é verificada. Se a condição for verdadeira para o elemento atual, o find retorna o elemento e para de procurar.

**Retorno:**

**Se um elemento for encontrado:** O find retorna o primeiro elemento que satisfaz a condição.

**Se nenhum elemento for encontrado:** O find retorna undefined. Isso significa que nenhum elemento do array atendeu à condição especificada.


***sort()***

O método permite ordenar os elementos de um array.

```js
    const numeros = [4, 2, 5, 1, 3];
    numeros.sort((a, b) => a - b); // Crescente
    console.log(numeros); // [1, 2, 3, 4, 5]

```

O método `sort()` em JavaScript é usado para ordenar os elementos de um array. Ele recebe como argumento uma função que compara dois elementos do array por vez, representados pelos parâmetros "a" e "b".


Para entender como funciona a ordenação, imagine que a função `sort()` percorre o array, comparando pares de elementos. Para cada par (a e b), a função que você define dentro do `sort()` precisa retornar:


`Um número menor que zero:` Se você quer que o elemento "b" venha antes do elemento "a" na ordenação.


`Um número maior que zero:` Se você quer que o elemento "a" venha antes do elemento "b" na ordenação.


Se a pontuação de "a" for menor que a de "b", a função retorna um número negativo, colocando "b" antes de "a".


Se a pontuação de "a" for maior que a de "b", a função retorna um número positivo, colocando "a" antes de "b".


O método `sort()` modifica o array original. Se você precisa manter o array original intacto, faça uma cópia antes de usar o `sort()`.


Para entender melhor o funcionamento do `sort()`, você pode usar `console.log()` dentro da função de comparação para visualizar os elementos "a" e "b" durante a ordenação.

