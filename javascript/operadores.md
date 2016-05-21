# Operadores em javascript

*Operadores aritméticos:*

```javascript
  var valor1 = 4, valor2 = 2, valor3;

  //adição
  valor3 = valor1 + valor2; //6

  //subtração
  valor3 = valor1 - valor2; //2

  //multiplicação
  valor3 = valor1 * valor2; //8

  //divisão
  valor3 = valor1 / valor2; //0.5

  //módulo (resto)
  valor3 = valor1 % valor2; //0
  valor3 = valor1 % 3; //1
```

*Operadores de atribuição:*

```js
  var valor1 = 4, valor2 = 2;

  valor1 = valor2; //atribuição
  console.log(valor1); // 2

  valor1 += valor2; //soma e atribuição
  console.log(valor1); // 6

  valor1 -= valor2; //subtração e atribuição
  console.log(valor1); // 2

  valor1 *= valor2; //multiplicação e atribuição
  console.log(valor1); // 8

  valor1 /= valor2; //divisão e atribuição
  console.log(valor1); // 0.5

  valor1 %= valor2; //divisão e atribuição
  console.log(valor1); // 0
```

*Operadores de comparação*

```js
  var valor1 = 4, valor2 = 2;

  valor1 == valor2 //false
  valor1 != valor2 //true
  valor1 > valor2 //true
  valor1 < valor2 //false
  valor1 >= valor2 //true
  valor1 <= valor2 //false

  //identico
  1 === 1 //true;
  1 === '1' //false
```

*Operadores de incremento*

```js
  var valor1 = 0;
  valor1++ //1
  valor1-- //0
  --valor1 //-1
  ++valor1 //0
```

*Operadores lógicos*
```js
  var a = true, b = false;
  a && b //false
  a || b //true
  !a //false
```
