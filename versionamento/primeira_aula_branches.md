# Branches

### Atenção: para esta aula, foi utilizado a ferramenta [Git](https://git-scm.com/), e o servidor de hospedagem foi o [Github](https://github.com/).

Ramificações podem ser caracterizados por divisões do projeto guardado. Uma vez criado um novo branch, as demais alterações realizadas no código não afetaram o branch principal. No git, o branch principal é chamado de master. Isto permite que os desenvolvedores tenham a liberdade de trabalhar em novas funcionalidades sem afetar o código estável.

Uma vez concluido o código de determinado branch, o usuário pode unir o branch secundário com o principal, realizando as devidas alterações.

Para criarmos uma ramificação, digite `git branch <nome_do_novo_branch> [<nome_branch_base>]`. O branch base pode ser qualquer ramificação criada. Caso digite apenas `git checkout -b <nome_do_novo_branch>`, você sairá do branch atual e irá entrar no novo branch. "Ah, mas qual é a base do novo brach neste caso?? :confused:". A base deste novo branch será o branch anterior, mesmo sem referencia-lo no comando. *Eu tive esta duvida também :joy:*

Caso queria excluir algum branch, existe duas formas: `git branch -d <nome_do_branch>` para os branchs que não tenham sido mesclados(*realizado o comando `merge`. Vamos ver isto no próximo parágrafo :smiley:*), e o comando `git branch -D <nome_do_branch>` caso já tenha sido mesclado.

Para mesclarmos um branch a outro, devemos utilizar o comando `git merge <nome_do_branch>`, permitindo que o branch `nome_do_branch` seja mesclado ao branch atual. Normalmente, esta opção deixa ativa por padrão o fast-foward, permitindo que o branch informado avance adiante até o branch atual, sem realizar um commit. Utilizando o comando `git merge <nome_do_branch --no-ff>`, um commit automático e cria um novo branch master com base no branch atual. Esta opção possibilita uma melhor visualização no histórico.
