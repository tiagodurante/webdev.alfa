# HTML Dom

### Document

Quando uma página HTML é carregada no navegador, ela se torna o objeto document. Basicamente, document é um nó do HTML que contem outros nós, sendo acessível pela propriedade ``window.document`` ou pela variável ``document``.

##### Métodos
* __Document.addEventListener(event, handler):__ adiciona um manipulador de evento ao evento;
* __Element.appendChild(element):__ adiciona um elemento filho ao documento;
* __Document.getElementById(id):__ retorna o elemento com o respectivo id;
* __Document.getElementsByClassName(className):__ retorna os elementos com respectivo nome de classe;
* __Document.getElementsByTagName(tagName):__ retorna os elementos que possuem a mesma tag;
* __Document.querySelector(selector):__ Retorna o primero elemento que coincide com o Seletor CSS especificado no documento;
* __Document.querySelectorAll(selector):__ Retorna todos os elementos que coincide com o Seletor CSS especificado no documento.

### Element

Um objeto element representa um elemento no documento HTML, podendo haver elementos filhos. Alguns métodos permitem retornar uma lista de elementos, e cada elemento possui atributos.

##### Métodos
* __Element.addEventListener(event, handler):__ adiciona um manipulador de evento ao evento;
* __Element.appendChild(element):__ adiciona um elemento filho ao elemento;
* __Element.className:__ define ou retorna a classe do elemento;
* __Element.getElementsByClassName(className):__ retorna os elementos com mesmo nome de classe;
* __Element.innerHTML:__ define ou retorna o conteúdo do elemento;
* __Element.getElementsByTagName(tagName):__ retorna uma lista de elementos com a mesma tag;
* __Element.querySelector(selector):__ Retorna o primero elemento que coincide com o Seletor CSS especificado no elemento.
* __Element.querySelectorAll(selector):__ Retorna uma lista contendo todos os elementos que coincide com o Seletor CSS especificado no elemento.
* __Element.style:__ Define ou retorna o valor dos estilos do elemento.

### Style

Os nomes das propriedades de Style são os mesmos usados no CSS, entretanto nomes de propriedades CSS que contém hífen (-) são modificados de acordo com o padrão lowerCamelCase (remove-se o hífen, e a próxima letra é alterada para caixa alta).

```CSS
border /*border*/
background /*background*/
border-top-color /*borderTopColor*/
background-color /*backgroundColor*/
```
