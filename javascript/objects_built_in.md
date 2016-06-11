# Objetos built-in em javascript

Caracteriza os tipos de valores disponíveis para se atribuir a uma variável. Lembrando que, os métodos listados de cada tipo não são todos, são apenas alguns para exemplos.

### String
Permite trabalhar com um conjunto de caracteres, podendo também manipular seu valor a partir de métodos já estabelecidos. De forma primitiva, tipo que é utilizando é string e a própria linguagem faz a conversão entre string e objeto.

```js
var string = new String('Tiago Amado Durante');
var string2 = 'Tiago Amado Durante';

// propriedades de string
console.log(string.length) // retorna o numero de caracteres
// => 19
```

##### Métodos para String
* __String.indexOf(searchValue[, fromIndex]):__ permite realizar a busca de algum caracter na string em questão usando searchValue, podendo também de forma opcional, informar o index que de onde se deve partir;
* __String.replace(pattern, replacement):__ substituir algum caracter ou conjunto informados pelo pattern e com o replacement, informar o que deve ser colocado naquele local;
* __String.split(separator):__ divide a string em um array, informando a forma em que deve ser separado;
* __String.substr(start[, length]):__ informa o conjunto de string a partir de um caracter;
* __String.substring(indexA, indexB):__ informa o conjunto de caracteres determinados entre o index inicial e final;
* __String.toLowerCase():__ retorna toda a string em caixa baixa;
* __String.toUpperCase():__ retorna toda a string em caixa alta;

```js
var s = new String("Republica do Brasil");
console.log(s.indexOf("a")); // 8
console.log(s.replace("Brasil", "Congo")); // Republica do Congo
console.log(s.split(" ")); // ["Republica", "do", "Brasil"]
console.log(s.substr(10)); // do Brasil
console.log(s.substring(10, 12)); // do
console.log(s.toLowerCase()); // republica do brasil
console.log(s.toUpperCase()); // REPUBLICA DO BRASIL
```

### Number

Este tipo permite trabalhar com valores numéricos, envolvendo o tipo primitivo number, permitindo sua manipulação a partir de métodos estabelecidos. Da mesma forma que em String, o Number funciona da mesma forma, onde o javascript realiza a conversão de primitivo para objeto automaticamente.

```js
// seja iniciando o valor a partir de um método ou apenas setando seu valor de forma manual, uma variável number será criada
var numero = new Number(1);
var numero = new Number(1.10);
var numero = 1;
var numero = 1.10;
```

##### Métodos para Number
* __Number.toFixed(digits):__ retorna uma string com os decimais do valor informado;
* __Number.toLocaleString():__ retorna uma string com o valor local do valor informado;

```js
var n = new Number(3.14);
console.log(n.toFixed()); // 3
// pt_BR = 3,14
// en = 3.14
console.log(n.toLocaleString());
```

### Array

Permite guardar diversos valores de tipos diferentes em uma mesma variável.

```js
var a = new Array(1, 'tiago', 2, 3);

a.length // propriedade exibe o numero de itens dentro do array;
// => 4
```

##### Métodos para Array
* __Array.join(glue):__ junta os elementos em uma string;
* __Array.pop():__ remove o ultimo elemento do array e retorna;
* __Array.push(...values):__ permite incluir no array vários itens e retorna o length do array completo;
* __Array.shift():__ remove o primeiro item do array e retorna;
* __Array.unshift(...values):__ informa um ou mais valores no inicio do array e retorna o comprimento do array por completo;

```js
var a = new Array(9,8,7,6);
console.log(a.join("-")); // 9-8-7-6
console.log(a.pop()); // [9,8,7] => 6
console.log(a.push(5, 4)); // [9,8,7,6,5,4] => 6
console.log(a.shift()); // [8,7,6] => 9
console.log(a.unshift(10)); // [10,9,8,7,6] => 5
```

### Math

O objeto Math oferece diversos metodos e propriedade que auxiliam em processos matemáticos.

```js
  var aux = Math.PI; // retorna o valor aproximado de PI
  // => 3,1415...
```

##### Métodos para Math
* __Math.abs(number):__ valor absoluto de um numero;
* __Math.ceil(number):__ arredonda frações pra cima;
* __Math.floor(number):__ arredonda frações para baixo;
* __Math.max(...numbers):__ retorna o maior valor entre os numbers;
* __Math.min(...numbers):__ retorna o menor valor entre os numbers;
* __Math.pow(base, exponent):__ retorna o calculo de base elevado ao exponent;
* __Math.random():__ retorna um valor entre 0 e 1. (0 >= valor < 1);
* __Math.round(number):__ retorna o valor mais próximo de number;

```js
console.log(Math.PI); // 3.14...
console.log(Math.abs(10)); // 10
console.log(Math.abs(-10)); // 10
console.log(Math.ceil(3.14)); // 4
console.log(Math.ceil(-3.14)); // -3
console.log(Math.floor(3.14)); // 3
console.log(Math.floor(-3.14)); // -4
console.log(Math.max(1,5,7)); // 7
console.log(Math.min(1,5,7)); // 1
console.log(Math.pow(2, 3)); // 8
console.log(Math.pow(2, -1)); // 0.5
console.log(Math.random(2, -1));
console.log(Math.round(1.4)); // 1
console.log(Math.round(1.5)); // 2
```

### Date

O objeto Date permite obter e manipular valores temporais.

```js
// Data/Hora atual
var d = new Date( );
// timestamp_miliseconds
// Sun May 08 2016 17:22:01 GMT-0300 (BRT)
var d = new Date(1462738921000);
var d = new Date(’2014-08-09’);
// year,month,date[,hour,minute,second,millisecond ]
// Wed Jan 15 2014 00:00:00 GMT-0200 (BRST)
var d = new Date(2014,00,15);
```

##### Métodos para Date
* __Date.getDate():__ retorna o dia do mês;
* __Date.getDay():__ retorna o dia na semana, sendo que o domingo é interpretado pelo valor 0;
* __Date.getFullYear():__ retorna o ano;
* __Date.getHours():__ retorna a hora;
* __Date.getMinutes():__ retorna os minutos;
* __Date.getMonth():__ retorna os mêses, iniciando com janeiro com o valor 0;
* __Date.getSeconds():__ retorna os segundos;
* __Date.getTime():__ retorna o timestamp_miliseconds;

```js
// year, month, date, hour, minute, second
var d = new Date(2016, 04, 14, 13, 14, 15);
console.log(d.getDate()); // 5
console.log(d.getDay()); // 6
console.log(d.getFullYear()); // 2016
console.log(d.getHours()); // 13
console.log(d.getMinutes()); // 14
console.log(d.getMonth()); // 4
console.log(d.getSeconds()); // 15
console.log(d.getTime()); // 1463242455000
```
