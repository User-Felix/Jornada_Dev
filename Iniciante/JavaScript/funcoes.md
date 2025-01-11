**As funções JavaScript** são blocos de código reutilizáveis que executam uma tarefa específica, recebendo alguma forma de entrada e retornando uma saída.

Para definir uma função, você deve usar a palavra-chave **function** , seguida de um **name** , seguido de parênteses **( )**.  Então você tem que escrever a lógica da função entre colchetes **{}**

Aqui está um exemplo de como escrever uma função em JavaScript:

```jsx
    function nomeDaFucao(parametros) {
    //aqui é escrito a logica para a fução
    }
    //chamando a função
    nomeDaFuncao()
```

```jsx
    function somaDoisNumeros(x, y) {

            console.log(x + y;)

    }

    somaDoisNumeros(10 ,15);
```

Há muita coisa acontecendo no exemplo acima, então vamos analisar cada parte individualmente.

- “Função” é a palavra- **chave** necessária para realmente começar a declarar uma função
- “addTwoNumbers” é o **nome** da função , que é personalizável. Os nomes das funções podem conter letras, números e certos caracteres especiais, assim como as variáveis.
- (x, y) são **parâmetros** , que são nomes de variáveis para as entradas que a função aceitará. Esses parâmetros também são chamados de **argumentos.**
- “Return” é a palavra- **chave** que sai da função e compartilha um valor opcional fora
- O código que a função irá executar deve ser colocado entre chaves **{}**