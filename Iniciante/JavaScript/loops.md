JavaScript tem as estruturas de repetição com os laços `while` e `do-while`. O primeiro é bom para repetições básicas; o segundo é para os casos em que você queira que o corpo da repetição seja executado pelo menos uma vez antes de continuar:

```js
let n = 0;
let x = 0;

while (n < 3) {
  n++;
  x += n;
}
//cuidado com loop infinitos
while (true) {
  // um loop infinito!
}

let resultado = '';
let i = 0;

do {
   i += 1;
   resultado += i + ' ';
} while (i < 5);
console.log(resultado)
```

### W**hile**

A **declaração while(enquanto)** cria um laço que executa uma rotina especifica enquanto a condição de teste for avaliada como verdadeira. A condição é avaliada antes da execução da rotina.

```js
while (condição) {
  rotina
}
```

### `condição`

Uma expressão avaliada antes de cada passagem através do laço. Se essa condição for avaliada como verdadeira, a rotina é executada. Quando a condição for avaliada como falsa, a execução continua na declaração depois do laço `while`.

### rotina

Uma declaração que é executada enquanto a condição é avaliada como verdadeira. Para executar múltiplas declarações dentro de um laço, use uma declaração em [bloco](https://developer.mozilla.org/en-US/docs/Web) (`{ ... }`) para agrupar essas declarações.

### D**o...while**

A declaração **`do...while`**(fazer enquanto) cria um laço que executa uma declaração até que o teste da condição for falsa (false). A condição é avaliada depois que o bloco de código é executado, resultando que uma declaração seja executada pelo menos uma vez.

```js
    do
    rotina
    while (condição);
```

### F**or**

A instrução `for` cria um loop que consiste em três expressões opcionais, dentro de parênteses e separadas por ponto e vírgula, seguidas por uma declaração ou uma sequência de declarações executadas em sequência.
```js
    
    for (let i = 0; i < 9; i++) {
        console.log(i);
        // mais declarações
    }
```

**`Inicialização:`** Geralmente usada para declarar e inicializar uma variável de controle, como **let i = 0**. 
Executada apenas uma vez no início do loop.
**`Condição:`** Uma expressão booleana que é avaliada antes de cada iteração. O loop continua enquanto essa condição **i < 9** for verdadeira .
**`Expressão final:`** Executada no final de cada iteração. Geralmente usada para atualizar a variável de controle, como **i++**.