**As funções JavaScript** são blocos de código reutilizáveis que executam uma tarefa específica, recebendo alguma forma de entrada e retornando uma saída.

Aqui está um exemplo de como escrever uma função em JavaScript:

```js
    function nomeDaFucao(parametros) {
    //aqui é escrito a logica para a fução
    }
    //chamando a função para execução
    nomeDaFuncao()
```

```js
    function somaDoisNumeros(x, y) {

            console.log(x + y;)

    }

    somaDoisNumeros(10 ,15)
```

Vamos analisar cada parte individualmente do codigo a cima.

- “Função” é a palavra- **chave** necessária para realmente começar a declarar uma função
- “somaDoisNumeros” é o **nome** da função , que é personalizável. Os nomes das funções podem conter letras, assim como as variáveis.
- (x, y) são **parâmetros** ,as entradas que a função aceitará. Esses parâmetros também são chamados de **argumentos.**
- “Return” é a palavra- **chave** que sai da função e compartilha um valor opcional fora
- O código que a função irá executar deve ser colocado entre chaves **{}**


***Retorno de Valores: Exportando Resultados***

A palavra-chave `return` é utilizada para **especificar o valor que a função retorna** quando invocada. O valor retornado pode ser de qualquer tipo, incluindo objetos, strings, números e booleanos:

```js
    function calcularDesconto(preco, desconto) {
        return preco * desconto;
    }

let valorDesconto = calcularDesconto(100, 0.1);
console.log(valorDesconto); // Exibe 10

```

No exemplo acima, a função `calcularDesconto` retorna o valor do desconto, que é armazenado na variável `valorDesconto`.

***Escopo de Função: Visibilidade e Proteção***

Funções criam um **escopo**, que define a **visibilidade das variáveis**. Variáveis declaradas dentro de uma função só podem ser acessadas dentro dela, enquanto variáveis declaradas fora da função (escopo global) podem ser acessadas em qualquer lugar do código:

```js
    function minhaFuncao() {
        let mensagem = "Olá, mundo!"; // Variável local
        console.log(mensagem); // Acessível dentro da função
    }

    minhaFuncao();
    console.log(mensagem); // Erro: mensagem não definida

```

O escopo de função **protege as variáveis locais**, evitando conflitos com variáveis de mesmo nome em outras partes do código. No entanto, você pode **acessar valores dentro de uma função** utilizando o `return`.

***Boas Práticas: Clareza e Concisão***

- **Nomes descritivos:** Utilize nomes que descrevam claramente a ação da função.
- **Funções concisas:** Limite o número de parâmetros (idealmente, no máximo dois).
- **Uma ação por função:** Cada função deve realizar apenas uma tarefa específica.
- **Evite efeitos colaterais:** Minimize a modificação de variáveis externas à função.