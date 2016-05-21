# Introdução a javascript

Javascript teve um início focado em aplicações web client side, onde é possível manipular objetos e valores dentro de uma pagina web. O objetivo dele é realizar tarefas que o próprio HTML não faz, como alterar valores, enviar informações ao servidor, inserir objetos dentro da página, entre outras funções. Apesar que, em seu início, seu uso era limitado, resumido apenas em executar algumas tarefas como foi dito acima, entretanto, o mundo da voltas, e fez com que o javascript se tornasse umas das linguagens de programação mais utilizadas não só na web, mas em outras plataformas. Hoje ele faz parte de dispositivos móveis, plataformas de games, server side, entre outras.

Alguns frameworks que utilizam javascript são: Node.JS (server), Unity3D (games), AppAccelerator (mobile), Ionic (mobile), etc.

**Atenção:** javascript !== java. Muitos podem acreditar que é a mesma coisa mas o resultado da comparação acima é `true`

Existe três formas de adicionar um código javascript a uma página HTML:

- **inline:** o código js está incluído no `<body>` do código HTML;
- **incorporado:** insere uma seção `<script>` dentro do `<head>` da página;
- **externo:** onde o arquivo com o código JS fica localizado fora do arquivo HTML mas podemos chama-lo pela tag `<script src:"<nome_do_arquivo.js>">`;

Quando vamos criar variáveis no código JS, precisamos seguir algumas regras básicas:

- As variáveis são case sensitive, onde as letras maiúsculas se diferem das minúsculas, e vice versa.

  - Ex: `objeto !== Objeto`;

- É recomendado o uso de palavras nas variáveis. Numeros apenas no final do nome.

  - Ex: `a1, variavel, variavel1, variavel2, objeto`;

- Underline e cifrão são permitidos em qualquer posição da variável.

  - Ex: `$objeto, _objeto, nome_professor`;

- Uma ou mais variáveis podem ser declaradas em apenas uma linha.

  - Ex: `var a1 = 0, a2 = 1, objeto = [];`

- Tipos de variáveis disponíveis:

  - Number (aceita qualquer tipo de número, seja inteiro, com ponto flutuante, irracional);
  - String (aceita qualquer tipo de caracter);
  - Boolean (true ou false);
  - Null (nada);
  - Undefined (sem valor);
  - Object (tipo composto, array);

- Os arrays são conjunto de valores separados por vírgulas e seu contador é iniciado pelo zero. Pode ser iniciado apenas por cochetes `var array = [];` ou `var array = new Array();`. Um array é iterável, portanto, utilize alguma forma de iteração para exibir os valores internos:

  ```javascript
  var nomes = ['tiago', 'felipe', 'bruno', 'efraim', 'renato'];
    for (var i = 0; i < nomes.length; i++) {
      console.log(nomes[i]);
    }
    ```

- Um objeto que possua propriedades se assemelha a um objeto JSON:

  ```javascript
      var eu = {
        nome: 'Tiago Amado Durante',
        cidade: 'Altônia/PR',
        anoNascimento: '1993'
      };

      console.log(eu.nome);
      //Tiago Amado Durante
      console.log(eu['nome']);
      //Tiago Amado Durante
  ```

- Os valores de um objeto podem ser alterados desta forma:

  ```javascript
    var eu = {
    nome: 'Tiago Amado Durante',
    cidade: 'Altônia/PR',
    anoNascimento: '1993'
    };

    console.log(eu.nome);
    //Tiago Amado Durante

    eu.nome = 'Tiago Durante';

    console.log(eu.nome);
    //Tiago Durante
  ```


- Caso seja um array de objetos, cada objeto terá seu identificador:

  ```js
    var nomes = [
      {
        nome: 'Tiago Amado Durante',
        cidade: 'Altônia'
      },
      {
        nome: 'Felipe Bock de Faria',
        cidade: 'Marechal Cândido Rondon'
      }
    ];

    console.log(nomes[0].nome);
    //Tiago Amado Durante
    console.log(nomes[1].cidade);
    //Marechal Cândido Rondon
  ```
