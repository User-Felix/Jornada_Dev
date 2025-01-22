```js
//JSON - JavaScript Object Notation
// chave e valor com o objetivo de transferir dados
let invoice = {
	name: "felipe",
    age: 28,
    products: {
    	0: ["mouse 2xwm", 29.90],
        1: ["Teclado mecânico", 129.99],
        2: ["Monitor", "899.99"],
        3: ["TV 100 polegadas", "10000.90"]
    },
    taxes: "98.90"
}

generateInvoice(invoice)

function generateInvoice(invoice){
	console.log(`O comprador é ${invoice.name}`)
    console.log(`A idade é ${invoice.age}`)
    console.log("------------")
    
    for(let index in invoice.products){
    	let [productName, productPrice] = invoice.products[index]
        console.log(`- ${productName}: R$ ${productPrice}`)
    }
    
    
}
```

**O Que É Esse Tal de JSON?**

Sabe quando você tem uma mochila mágica onde guarda todos suas armas e poções? JSON é um jeito de guardar informações especiais em um formato que o computador entende, tipo uma mochila mágica para dados!

**Criando Dados em JSON**

Pensa assim: você quer guardar informações sobre seus bichinhos de estimação, como nome, cor e tipo. 
Com JSON, é fácil!

```js
let bichinhos = [
  { "nome": "Mimi", "cor": "preto", "tipo": "gato" },
  { "nome": "Flufi", "cor": "marrom", "tipo": "coelho" }
];

```

**Conversando com Dados Mágicos em JSON**

Agora, imagine que você quer saber a cor do bichinho chamado "Mimi". Com JSON, é como conversar com seus brinquedos!

```js
let bichinhoEscolhido = bichinhos[0];
console.log("O " + bichinhoEscolhido.nome + " é " + bichinhoEscolhido.cor + "!");

```

Aqui, a gente escolheu o bichinho na posição 0 da lista (que é o "Bolinha") e perguntou a cor dele. Ele nos respondeu "amarelo"!

**Mandar e Receber Dados em JSON**

JSON também é ótimo para mandar e receber informações. Imagine que você quer compartilhar a lista de bichinhos mágicos com um amigo. Você pode fazer assim:

```js
let listaParaAmigo = JSON.stringify(bichinhos);
console.log(listaParaAmigo);

```
Trabalhando...