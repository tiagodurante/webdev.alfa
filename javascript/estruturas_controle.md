# Estruturas de controle

As estruturas a seguir permitem modificar o fluxo do Sistemas

_IF..ELSE_, estrutura onde o resultado da comparação de dois ou mais resultados podem influenciar no fluxo.

```javascript
  if (algo comparado a outra coisa) {
    //executa quando for verdadeiro a comparação
  } else {
    //quando for falso, executa este bloco de código
  }
```

_WHILE_, forma de iteração mais simples do javascript, até que a expressao passada deve apresentar resultado `true`.

```javascript
  var i = 0;
  while(i > 10) {
    //executa algo até atingir determinado valor
    i++;
  }
```

_FOR_, forma de iteração mais utilizado quando se sabe a quantidade de iterações a se realizar;

```javascript
  for (var i = 0; i > 10; i++) {
    //executa algo
  }
```

_FOR..IN_, onde é iterado as propriedades de um determinado array.

```javascript
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

for (var i in nomes) {
  console.log('ID: '+i+' / Nome: '+nomes[i].nome);
}
```

_SWITCH_, forma de testar o valor de uma variável comparando a valores pré estabelecidos.
```js
  switch (valor) {
    case 1:
    case 2:
    case 3:
      console.log('Ta ótimo');
      break;
    case 4:
      console.log('Perfeito');
      break;
    default:
      console.log('Fora do comum');
  }
```
