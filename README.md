# Curso de GIT/Github para iniciantes

### Alguns comandos simples

* [`git log`](https://git-scm.com/docs/git-log/pt_BR): Mostra informações gerais do repositório, como branches, autores, datas, emails, etc. Ele pode ser combinado com algumas "flags" para sinalizar que você busca por algumas informações específica, como `git log --author="nome"`, onde estará exibindo apenas as informações que sejam referente a um autor específico e também o `git log --graph` que mostra de forma grafica o estado das branches.
* [`git shortlog`](https://git-scm.com/docs/git-shortlog/pt_BR): O mesmo que o `git log`, porém de forma mais suscinta, eles apresenta um resumo das informações com o nome do autor, quantidade de commits e os arquivos rastreados em nome deste autor. É interessante ressaltar uma forma de exibição ainda mais simplificada, `git shortlog -sn`, onde mostra apenas a quantidade de commits e o nome do autor.
* [`git show`](https://git-scm.com/docs/git-show/pt_BR): Ele mostra as diferenças adicionadas/retiradas do arquivo que está sendo monitorado.
* [`git diff`](https://git-scm.com/docs/git-diff/pt_BR): Exibe as alterações feitas em um arquivo/item antes de ser enviado ao repositório.
* [`git checkout nome-do-arquivo`](https://git-scm.com/docs/git-checkout): Caso seu arquivo tenha sido editado, porém antes de ser adicionado ou comitado, é possível reverter através do checkout, porém o comando checkout não ser apenas para isso.
* [`git reset HEAD nome-do-arquivo`](https://git-scm.com/docs/git-reset): Você restaura um arquivo que vc já havia adicionado/commitado mas antes de enviar para o repositório. Existem 3 variações de flags pricipais, a `--soft` (Não altera o index ou o working-tree, mantém tudo como estava, apenas devolvendo pra um estado antes de adicionar ou commitar), `--mixed` (Reseta o index mas mantém o working tree) e `--hard` (reseta o index e o working tree)
* 