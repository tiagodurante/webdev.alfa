# Formulários em HTML5

Os formulários em HTML sofreram diversas alterações e, inclusive, ganhou novos componentes, ajudando o dia a dia do programador, principalmente aquele que procura integrar sua página web ao ambiente mobile.

### Tipos de entrada para inputs

Estas formas de entradas são de grande importância para o programador. A partir deles, é possível determinar qual o tipo de dado que será trabalhado no campo. Na maioria dos casos, em versões mobile, de acordo com o tipo de entrada, o teclado do próprio dispositivo é alterado, reduzindo a inserção incorreta de valores.

Segue a lista dos novos campos:

* **number** : entrada numéria;
* **tel** : entrada de numeros telefônicos;
* **search** : utilizado para realizar buscas, permitindo que o campo fique estilizado de acordo com um campo de busca;
* **email** : limita a entrada apenas de e-mails, seja apenas um ou vários, separados por vírgulas;
* **url** : insere uma url;
* **date** : entrada de datas, permitindo o uso de um datepicker nativo;
* **datetime** : permite entrada de data e hora;
* **month** : entrada de mês;
* **week** : entrade de semana;
* **time** : entrade de hora e minuto;
* **range** : input deslizante com controle;
* **color** : permite escolher uma cor;

### Atributos de entrada de dados

Estes atributos permitem que o formulário se torne mais transparente aos olhos do usuário, ou seja, permite que o seu uso seja mais fácil durante seu preenchimento.

* **autofocus** : foca o input no momento em que a página é carregada;
```html
<input type="email"
        name="email"
        id="email"
        autofocus>
```

* **autocomplete** : caso ele tenha sido preenchido anteriormente, permite com que o campo exiba valores ja usados naquele campo;
```html
<input type="email"
        name="email"
        id="email"
        autocomplete>
```

* **form** : permite que elementos de entrada possam ser utilizados em diversos lugares da página;
```html
<form id="form1" method="post"></form>
```

* **placeholder** : exibe um tipo de dica para o usuário. Por default, ele aparece com uma cor cinza clara, dentro do input. O desenvolvedor pode utilizar este atributo para indicar a forma de dado que deve ser inserida ao usuário;
```html
<input type="number"
        name="data"
        id="data"
        placeholder="Digite sua idade">
```

* **required** : valida se o input foi corretamente preenchido, de acordo com os artributos que o desenvolvedor estabeleceu;
```html
<input type="number"
        name="data"
        id="data"
        placeholder="Digite sua idade"
        required>
```

* **pattern** : permite utilizar expressões regulares para validar os campos, sem a necessidade de JavaScript;
```html
<input type="text"
        name="cpf" id="cpf"
        placeholder="Digite seu CPF"
        required pattern="\d{3}\.\d{3}\.\d{3}-\d{2}\"
        title="Digite o CPF no formato 000.000.000-00">
```
