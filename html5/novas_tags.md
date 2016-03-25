# Novas tags do HTML5

Está e a estrutura básica do html
´´´HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Estrutura do HTML</title>
  </head>
  <body >
    Hello World
  </body>
</html>
´´´

# Novos elementos

### Scripting

* **template** : Container para conteúdo no lado cliente instanciado em tempo de execução usando JavaScript;

### Seções

* **section** : Define a seção do Documento;
* **nav** : Define uma seção que contém apenas links de navegação;
* **article** : Define que pode existir uma forma independente do resto do conteúdo. Esta tag poderia ser um post no fórum, um artigo de revista ou jornal, uma entrada de log na web, um comentário, ou qualquer outro item independente do conteúdo;
* **aside** : Define  um contúdo reservado do resto da página. Caso seja removida, o conteúdo restante ainda faz sentido;
* **header** : Define o cabeçalho de uma página ou seção;
* **footer** : Define o rodapé de uma página ou seção;
* **main** : Define o conteúdo principal ou importante do documento. Existe apenas um elemento *main* e uma página.

### Agrupando conteúdos

* **figcaption** : Representa o conteúdo de uma figura
* **figure** : Tabalha junto com o *figcaption*, o *figure* permite marcar diagramas, ilustrações, fotos e até mesmo fragmentos de código, etc;

### Semântica textual

* **data** : Associa o seu conteúdo a um equivalente legível por máquina.(Este elemento esta apenas na versão padrão HTML do WHATWG, e não documentado na versão HTML5 da W3C);
* **time** : Representa um valor de data e hora, eventualmente com um equivalente legível por máquina;
* **mark** : Representa um texto de referência;
* **ruby** : Representa um conteúdo marcado com anotações em ruby;
* **rt** : Representa uma anotação em ruby;
* **rp** : Representa o parentêses em volta da anotação em ruby, usado para apresenta a anotação como meio alternativo para os browsers que não suportam a forma normal;
* **wbr** : Representa uma quebra de linha;

### Conteúdo embutido

* **embed** : Representa a integração com algo externo, uma aplicação ou conteúdo interativo;
* **video** : Representa um video e pode ser associado a arquivos de audio e legendas, com a possibilidade de interface para iniciar o video;
* **audio** : Representa um audio ou um stream de audio;
* **source** : Permite especificar uma alternativa a um elemento de media como _video_ ou _audio_;
* **track** : Permite apresentar o texto da faixa de um elemento de media;
* **canvas** : Permite renderizar graficos em HTML5;
* **svg** : Define uma imagem vetorial compactada;
* **math** : Representa uma fórmula matemática;

### Formulários

* **datalist** : Representa um conjunto de opções pré definidas e outros controles.
* **keygen** : permite controler um gerador de chaves;
* **output** : Permite apresentar o resultado de um calculo;
* **progress** : Permite apresentar o andamento de uma tarefa;
* **meter** : Permite mensurar um valor dentro de um intervalo;

### Elementos Interativos

* **details** : Representa um *widget* que o usuário pode utilizar para obter informações adicionais ou controles;
* **summary** : Representa um sumario ou legenda da tag *details*;
* **command** : Representa um comando que o usuário pode executar;
* **menu** : Representa uma lista de comandos;

> Referência
> [Lista de elementos do HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5/HTML5_element_list)
