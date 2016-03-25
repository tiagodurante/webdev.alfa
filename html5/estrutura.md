# Estrutura do HTML5

Para começar o assunto sobre HTML5, nada melhor do que apresentar aos mais leigos, um pouco da história desta linguagem. De acordo com a W3C (responsável por desenvolver padrões para a web), define que a web é baseada em 3 pilates:

* Um esquema de nomes para a localização de fontes de informação na web, esse esquema se chama URI;
* Um protocolo de acesso para acessar estas fontes, hoje o mais conhecido é o http;
* Uma linguagem de Hypertexto, para a fácil navegação entre as fontes de informação: o HTML;

Já que vamos abordar sobre o HTML, ele é basicamente uma abreviação de _Hypertext Markup Language_ (Linguagem de Marcação de Hypertexto). Esta é a linguagem responsável pela publicação de qualquer conteúdo na internet.

Desenvolvido originalmente por Tim Berners-Lee, o HTML é um conceito de hipertexto formado por um conjunto de elementos (ou nós) responsáveis por apresentar os conteúdos em uma página. Estes elementos podem ser palavras, imagens, vídeos, etc. Diferente de um texto comum onde um assunto é ligado a outro seguidamente, a conexão entre os elementos é algo imprevisto, mas que permite a comunicaçao de dados, organizando conhecimentos e guardando informações relacionadas.

O HTML tem como propósito ser uma linguagem entendida universalmente. Ela ganhou força quando Marc Andreessen desenvolveu o navegador Mosaic em 1990. A partir disso, desenvolvedores e fabricantes começaram a utilizar o HTML como base para compartilhamento de informações de forma padronizada.

Apesar de que o foco do HTML era padronizar a forma de publicação de conteúdo, entre 1993 e 1995, ela ganhou algumas novas versões (HTML+, HTML2.0, HTML3.0) mas só em 1997, a W3C trabalhou em uma versão 3.2 da linguagem, permitindo que ela fosse tratada como um padrão comum. O grande diferencial do HTML é sua interoperabilidade. Diferente das outras linguagens, esta não dependia de plataforma alguma, podendo ser desenvolvida e apresentada em diversos dispositivos.

![HTML5 3.2 W3C](./images/html5-img1.png)

Além da W3C que estava focada no desenvolvimento de uma segunda versão do XHTML, um grupo chamado _Web Hypertext Application Technology Working Group_ ou WHATWG estava trabalhando em uma versão do HTML em que trazia mais flexbilidade para a produção de websites e sistemas baseados na web. Fundada pelos desenvolvedores de empresas como Mozilla, Apple e Opera em 2004 que perceberam falhas no caminho em que a web estava tomando junto ao XHTML, por isso, estas organizações se juntaram e se comprometeram a desenvolver o que hoje conhecemos por HTML5.

Por volta de 2006, o trabalho deste grupo passou a ser conhecido mundialmente, inclusive pela W3C. Em outubro de 2006, Tim Berners-Lee anunciou que trabalharia juntamente ao WHATWG promovendo o desenvolvimento do HTML5 em detrimento ao XHTML2, entretanto, seria um trabalho paralelo. O XHTML2 foi mantido de acordo com as mudanças do HTML, mas, em 2009, o grupo responsável pelo XHTML2 parou suas atividades.

Nisso, o HTML4 apareceu, e os desenvolvedores dele (a W3C) informou que algumas boas praticas deveriam ser seguidas ao produzir códigos client-side. Deste esta época, assuntos como a separação da estrutura de código com a formatação e princícipos de acessibilidades foram trazidos para discução. Apesar de grandes mudanças, o HTML4 ainda não facilitava a manipulação de elementos via CSS e JS. Caso quisesse algo como isso, um grande script deveria ser escrito, com bugs, e que muitas vezes não funcionavam em todos os navegadores.

Por fim, aparece o HTML5!

![O novo (e forte) HTML5](./images/html5-img2.png)

O grande diferencial desta versão é que foi definido algumas APIs base para a arquitetura web, conhecidas como _DOM Level 0_. Um dos principais objetivos foi facilitar a manupulação de elementos de forma mais transparente e menos intrusiva para o usuário final.

Diferente das versões anteriores, o HTML5 fornece ferramentas para CSS e JS trabalharem da melhor forma possível. Responsável pelas novas APIs, a manipulação das caracteristicas destes elementos foi facilitada, de forma que o website ou aplicação se torne mais leve e funcional.

Nesta versão do HTML, foram criadas novas tags e outras foram modificadas, trazendo um padrão universal para a criação de seções comuns e específicas como rodapé, cabeçalho, menus, etc. Desta forma, fica mais facil localizar determinadas seções de forma automática. Atributos e elementos destas seções também foram modificados e agora podem ser reutilizados de forma mais eficaz.

Hoje, o HTML5 permite a escrita de um código mais organizado. Muito mais semântica e menos código. Mais interatividade e menos plugins, resultando em uma maior performance.

Bem vindo a web do futuro, onde o código é realmente interoperável, facilitando a reutilização da informação de diversas formas e pronta para a exibição em qualquer dispositivo.

# Novidades do HTML5

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

* *template* : Container para conteúdo no lado cliente instanciado em tempo de execução usando JavaScript;

### Seções

* section : Define a seção do Documento;
* nav : Define uma seção que contém apenas links de navegação;
* article : Define que pode existir uma forma independente do resto do conteúdo. Esta tag poderia ser um post no fórum, um artigo de revista ou jornal, uma entrada de log na web, um comentário, ou qualquer outro item independente do conteúdo;
* aside : Define  um contúdo reservado do resto da página. Caso seja removida, o conteúdo restante ainda faz sentido;
* header : Define o cabeçalho de uma página ou seção;
* footer : Define o rodapé de uma página ou seção;
* main : Define o conteúdo principal ou importante do documento. Existe apenas um elemento <main> e uma página.

### Agrupando conteúdos

* figcaption : Representa o conteúdo de uma figura
* figure : Tabalha junto com o *figcaption*, o *figure* permite marcar diagramas, ilustrações, fotos e até mesmo fragmentos de código, etc;

### Semântica textual

* data : Associa o seu conteúdo a um equivalente legível por máquina.(Este elemento esta apenas na versão padrão HTML do WHATWG, e não documentado na versão HTML5 da W3C);
* time : Representa um valor de data e hora, eventualmente com um equivalente legível por máquina;
* mark : Representa um texto de referência;
* ruby : Representa um conteúdo marcado com anotações em ruby;
* rt : Representa uma anotação em ruby;
* rp : Representa o parentêses em volta da anotação em ruby, usado para apresenta a anotação como meio alternativo para os browsers que não suportam a forma normal;
* wbr : Representa uma quebra de linha;

### Conteúdo embutido

* embed : Representa a integração com algo externo, uma aplicação ou conteúdo interativo;


> Referência
> http://www.w3c.br/cursos/html5/conteudo/capitulo1.html
