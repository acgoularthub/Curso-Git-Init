# Curso de GIT/Github para iniciantes

### Alguns comandos simples

* [`git log`](https://git-scm.com/docs/git-log/pt_BR): Mostra informações gerais do repositório, como branches, autores, datas, emails, etc. Ele pode ser combinado com algumas "flags" para sinalizar que você busca por algumas informações específica, como `git log --author="nome"`, onde estará exibindo apenas as informações que sejam referente a um autor específico e também o `git log --graph` que mostra de forma grafica o estado das branches.
* [`git shortlog`](https://git-scm.com/docs/git-shortlog/pt_BR): O mesmo que o `git log`, porém de forma mais suscinta, eles apresenta um resumo das informações com o nome do autor, quantidade de commits e os arquivos rastreados em nome deste autor. É interessante ressaltar uma forma de exibição ainda mais simplificada, `git shortlog -sn`, onde mostra apenas a quantidade de commits e o nome do autor.
* [`git show`](https://git-scm.com/docs/git-show/pt_BR): Ele mostra as diferenças adicionadas/retiradas do arquivo que está sendo monitorado.
* [`git diff`](https://git-scm.com/docs/git-diff/pt_BR): Exibe as alterações feitas em um arquivo/item antes de ser enviado ao repositório.
* [`git checkout nome-do-arquivo`](https://git-scm.com/docs/git-checkout): Caso seu arquivo tenha sido editado, porém antes de ser adicionado ou comitado, é possível reverter através do checkout, porém o comando checkout não ser apenas para isso.
* [`git reset HEAD nome-do-arquivo`](https://git-scm.com/docs/git-reset): Você restaura um arquivo que vc já havia adicionado/commitado mas antes de enviar para o repositório. Existem 3 variações de flags pricipais, a `--soft` (Não altera o index ou o working-tree, mantém tudo como estava, apenas devolvendo pra um estado antes de adicionar ou commitar), `--mixed` (Reseta o index mas mantém o working tree) e `--hard` (reseta o index e o working tree)
PS. O `git reset` deve ser utilizado comm parcimônia, as alterações feitas nele podem influenciar em toda a pipeline caso seja um repositório que esteja sendo acessado por várias pessoas e as alterações interfiram em arquivos que já fossem enviados para o repositório remoto.
*  [`git checkout -b nome-da-branch`](https://git-scm.com/docs/git-checkout): Cria uma branch nova, podendo ser utilizado como um "checkpoint" para voltar ao estado anterior.
*  [`git checkout nome-da-branch`](https://git-scm.com/docs/git-checkout): Seleciona uma branch existente, podendo ser utilizado para voltar ao estado anterior.
*  [`git branch -d nome-da-branch`](https://git-scm.com/docs/git-branch): Deleta uma branch existente.
*  [`git stash`](https://git-scm.com/docs/git-stash): Salva o estado atual do repositório, podendo ser utilizado para voltar ao estado anterior.
*  [`git stash apply`](https://git-scm.com/docs/git-stash): Aplica o stash, caso tenha sido salvo.
*  `git config --global alias.stash "stash -u"`: Alias para o comando `git stash`.
*  [`git stash list`](https://git-scm.com/docs/git-stash): Lista os stashes.
*  [`git stash drop`](https://git-scm.com/docs/git-stash): Deleta um stash.
* [`git tag`](https://git-scm.com/docs/git-tag/pt_BR): Cria um tag no repositório. `git tag -a nome-do-tag` cria um tag com o nome `nome-do-tag` e `git tag -a nome-do-tag -m "mensagem"` cria um tag com o nome `nome-do-tag` e a mensagem `mensagem`.
* `git push origin main --tags`: Envia o repositório para o branch `main` do repositório remoto `origin` e também envia as tags.