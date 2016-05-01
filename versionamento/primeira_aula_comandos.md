# Comandos básicos

### Atenção: para esta aula, foi utilizado a ferramenta [Git](https://git-scm.com/), e o servidor de hospedagem foi o [Github](https://github.com/).

  - Criando um repositório: em um prompt de comando, digite `git init` para iniciar um novo repositório limpo dentro da pasta que voce acessar, ou digite `git init <diretorio>` para também iniciar um novo repositório mas, neste caso, será indicado o nome da pasta a ser criada. Nos dois casos, dentro da pasta criada, estará localizado o diretório ".git", onde se encontra as configurações da ferramenta.

  - Clonando um diretório: acesse uma pasta no prompt de comando e digite `git clone <url_repo>` indicando a url do repositório a ser clonado, ou digite ``git clone <url_repo> <diretorio>`` para criar uma nova pasta, e dentro dela, ser clonado o repositório em questão.

- É bom entender que o arquivo dentro de um repositório pode existir em diferentes estados. Eles são:

  - Untracked (*não rastreado*): o arquivo acaba de ser criado no repositório e ainda não faz parte do escopo;
  - Staged (*selecionado*): o arquivo começa a fazer parte do escopo, permitido que a ferramenta monitore o estado dele;
  - Unmodified (*não modificado*): estado após ser realizado um commit, o arquivo permanece como inalterado. Permite saber se houve alguma modificação antes mesmo de subir ao servidor;
  - Modified (*modificado*): alerta ao desenvolvedor que o arquivo foi modificado, e que precisa ser adicionado novamente ao escopo antes de realizar o commit;


- .gitignore: permite esconder determinados arquivos do projeto para que a ferramenta não faça upload:

Padrão | Significado
------------ | -------------
``nome_do_arquivo.db`` | Oculta determinado arquivo
``*.html`` | Oculta arquivos desta extenção
``!index.html`` | Apesar de oculto todos os .html na linha acima, aqui é liberado apenas o arquivo descrito.
``/log`` | Ignora diretório específico
``**/tmp`` | Ignora qualquer diretório nomeado. Neste caso, ignora qualquer diretório nomeado como *tmp*

- Para adicionar as mudanças do arquivo ou diretório, execute `git add <nome_do_arquivo ou nome_do_diretório>`, mudando o estado para *selecionado* e deixando pronto para o commit. Para remover as mudanças de um determinado arquivo para realizar o commit, digite `git reset <nome_do_arquivo>`. Para remover o arquivo do escopo da ferramenta, execute `git rm --cached <nome_do_arquivo>`, evitando que a ferramenta continue verificando suas alterações.

- Para salvar as alterações, execute `git commit -m <mensagem_obrigatoria>`. Este comando passa os arquivos selecionados para o estado de não modificado. A mensagem é obrigatória, tornando mais facil o entendimento dos commits. Caso queria adicionar os arquivos e ao mesmo tempo realizar o commit, digite `git commit -am <mensagem_obrigatoria>`. Também existe a possibilidade de reverter o commit anterior com o comando `git commit --amend -m <mensagem_obrigatoria>`, dando possibilidade de alterar o que foi comitado.

- Para verificar o status da situação atual do seu git, execute `git status` ou `git status -s`. O parâmetro `-s` torna a exibição mais simplificada.

- Os *commits* podem ser referenciados por tags, tornando sua busca mais fácil em meio a tantos no servidor. Execute `git tag <tag> [<id_commit>]`. Você pode verificar todas as tags cadastradas usando o comando `git tag` ou buscar determinada tag com o comando `git tag -l <tag>`.

- Os *commits* podem ser referenciados por:
  - **``<sha1>``**: Hash sha-1 referente ao commit, baseado nos primeiros valores do hash. Ex: `hash: aa3c317fa06cf6cfa218b380def17233761d197c`, `sha-1: aa3c317`.
  - **tag**: tag referente ao commit. Ex: `v0.1.2`.
  - **branch**: ramificação de um repositório. Ex: `master`.

- Faça uma análise de determinado commit usando o comando `git show <id_commit>` ou busque o ultimo digitando apenas `git show`. Para abrir determinado arquivo do commit em questão, execute `git show <commit>:<nome_do_arquivo>`.
