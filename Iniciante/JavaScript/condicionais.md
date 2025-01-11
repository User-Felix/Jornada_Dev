As instruções condicionais controlam o comportamento em JavaScript e determinam se partes de código podem ou não ser executadas.

Existem vários tipos diferentes de condicionais em JavaScript, incluindo:

- Instruções **“If”**: onde se uma condição for verdadeira é usada para especificar a execução de um bloco de código.

```js
let numero = 10;

if (numero > 2) {
		console.log("É maior que 2")
}
```

- Instruções **“Else”**: onde se a mesma condição for falsa especifica a execução de um bloco de código.

```js
let numero = 10;

if (numero > 2) {
		console.log("É maior que 2")
}else {
	console.log("Não é maior que 2")
}
```

- Instruções **“Else if**”: especifica um novo teste se a primeira condição for falsa(Veremos isso mais a frente)

```js
    let numero = 10;

    if (numero > 11) {
        console.log("É maior que ", numero)
    }else if(numero > 7) {
        console.log("É maior que 7")
    }
```

A instrução switch é uma alternativa ao uso de múltiplos **if...else if**. Ela avalia uma expressão uma vez, comparando o valor da expressão com várias cláusulas **case**. 


```js

    let cor = "vermelho";

    switch (cor) {
        case "azul":
            console.log("A cor é azul");
            break;
        case "vermelho":
            console.log("A cor é vermelho");
            break;
        case "verde":
            console.log("A cor é verde");
            break;
        default:
            console.log("Cor não reconhecida");
            break;
    }


```

O switch verifica cada **case** em ordem.
Quando encontra o **case** correspondente (neste caso, **"vermelho"**), executa o código dentro desse bloco.
O **break** impede que os outros casos sejam verificados após o **case** correspondente ser encontrado.
Se nenhum **case** for correspondente, o código dentro de **default** será executado.
