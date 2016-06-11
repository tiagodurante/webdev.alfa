# Funções

O objetivo de uma função é reduzir a repetição de um mesmo bloco de código em diversas partes do sistema. Desta forma, o serviço do programador é reduzido, permitindo com que ele execute a mesma função sem reescreve-la novamente, e, torna o código mais limpo, tornando-o objetivo e claro. Com as funcões, podemos realizar o processamento de determinados dados afim obter um resultado.

Uma função em javascript possui esta estrutura:

```javascript
  //Lembrando que, o nome da função segue os mesmos princípios das variáveis
  function nome_da_funcao(param1, param2, ..., paramN) {

  }
```

Podemos executar uma função desta forma:

```javascript
  function exibeTexto(txt){ //por parâmetro, passamos o texto a ser exibido
    console.log(txt); //console.log() permite exibir informações no console do navegador
  }

  exibeTexto('Tiago');
  exibeTexto('Durante');
```

Caso seja necessário retornar algum valor onde a função foi chamada, faremos assim:

```javascript
  function soma(var1, var2){
    return var1 + var2; //a palavra "return" se encarrega de retornar o valor
 }

  console.log(soma(1, 2)); // =>3
```

As funções em javascript diferenciar as váriaveis por meio de escopos diferentes. Seguindo a lógica de outras linguagens, podemos contar com 2 escopos:

**Global**: tornando visível ao sistema por completo, dentro ou fora das funções;
**Local**: onde as variáveis são apenas visíveis dentro das funções;

```js
var a;
function iniciar() {
console.log(a); // undefined
console.log(b); // undefined
a = 10;
var b = 50;
console.log(a); // 10
console.log(b); // 50
}
console.log(a); // undefined
console.log(b); // erro
iniciar();
console.log(a); // 10
console.log(b); // erro
```
