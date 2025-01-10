**JavaScript** (frequentemente abreviado como **JS**) é uma linguagem de programação leve, interpretada e orientada a objetos com [funções de primeira classe](https://en.wikipedia.org/wiki/First-class_functions), conhecida como a linguagem de scripting para páginas Web, mas também [utilizada em muitos ambientes fora dos navegadores](https://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages).
Ela é uma linguagem de scripting [baseada em protótipos](https://en.wikipedia.org/wiki/Prototype-based_programming), multi-paradigma e dinâmica, suportando os estilos orientado a objetos, imperativo e funcional.

## Tipos Primitivos

- **String**
    
    
    Em JavaScript, Strings são valores compostos de texto e podem conter letras, números, símbolos, pontuação e até emojis!
    
    ```jsx
    'Isto é uma corda. 👏';
    "Esta é a 2ª corda. 💁";
    ```
    
- **Number**
    Números são valores que podem ser usados em operações matemáticas. Você não precisa de nenhuma sintaxe especial para números — basta escrevê-los diretamente no JavaScript.
    
    ```jsx
    12345;
    ```
    
    [Number - Glossário | MDN](https://developer.mozilla.org/pt-BR/docs/Glossary/Number)
    
- **Boolean**
    Em JavaScript, um valor booleano é aquele que pode ser TRUE ou FALSE. Se você precisa saber “sim” ou “não” sobre algo, então você deve usar a função booleana. Parece extremamente simples, mas os booleanos são usados o tempo todo na programação JavaScript e são extremamente úteis. Qualquer coisa que precise estar "ativada" ou "desativada", "sim" ou "não", "verdadeira" ou "falsa", ou que tenha apenas um propósito temporário, geralmente é adequada para booleanos.


    É útil armazenar booleanos em variáveis para acompanhar seus valores e alterá-los ao longo do tempo. Booleanos são usados como funções para obter os valores de variáveis, objetos, condições e expressões. Na verdade, os booleanos são críticos para que as condicionais funcionem.


    Em seu código, quando você precisa saber se uma condição está sendo atendida ou não antes de prosseguir para a próxima etapa, a função booleana se torna sua melhor amiga. Se *tal e tal* for VERDADEIRO, então faça isso. Se for FALSE, então faça outra coisa.


    Considere algo simples como fazer um sanduíche. Na sua cabeça, você realmente estará passando por uma série de booleanos e condicionais:


    Eu tenho pão? Verdadeiro ou falso. Se for TRUE, então posso prosseguir para a próxima etapa, se tenho ou não mostarda, presunto, etc. Se for FALSE, precisarei ir à loja para comprar pão. E assim por diante.


    Você nunca pode assumir nada ao programar - você tem que escrever a lógica explicitamente, e grande parte disso é simplesmente saber se uma condição está sendo atendida ou não. Daí a importância dos booleanos em JavaScript.


- **Null**
    O valor `null`  é um literal em JavaScript que representa um valor nulo ou "vazio" (p/ex: que aponta para um objeto inexistente).
    [null - JavaScript | MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/null)

- **Undefined**
    Um valor  primitivo automaticamente atribuído para variáveis que foram recentemente declaradas ou para argumentos formais para qual não existem argumentos atualmente.
    [Undefined | MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/undefined)
    
- **Symbol**
    Symbols são únicos e imutáveis, introduzido no ES6. Eles servem como identificadores para propriedades de objetos, evitando colisões de nomes e proporcionando uma maneira mais segura de criar propriedades privadas.
    
    [Symbol - Glossário | MDN](https://developer.mozilla.org/pt-BR/docs/Glossary/Symbol)