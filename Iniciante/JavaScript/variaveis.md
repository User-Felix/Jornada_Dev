**Variáveis** são valores nomeados e podem armazenar qualquer tipo de valor JavaScript.

[**`var`**](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/var)

Declara uma variável, opcionalmente, inicializando-a com um valor.

```js
var nome = "Nero";
```

[`let`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/let)

Declara uma variável local de escopo do bloco, opcionalmente, inicializando-a com um valor.

```js
let nome = "Nero";
```

[`const`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/const)

Declara uma constante de escopo de bloco, apenas de leitura.

```js
const nome = "Nero";
```

Qual a diferença de const, ler e var?

Variáveis `var` podem ser atualizadas e declaradas novamente dentro de seu escopo. (Cuidado ao utilizar var, se possível substitua sempre por let)

As variáveis `let` podem ser atualizadas, mas não podem ser declaradas novamente.
 
As variáveis de `const` não podem ser atualizadas nem declaradas novamente.
[Diferença entre let e var](https://www.alura.com.br/artigos/entenda-diferenca-entre-var-let-e-const-no-javascript)
