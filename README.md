
# :bulb: Git

Códigos essenciais para utilizar no terminal

### Inicializar repositório

    $ git init

### Conectar repositório local no GitHub

    $ git remote add origin <link do repositório do GitHub>

### Configurando usuário

    $ git config –global user.name “Seu nome”
    
    $ git config –global user.email “Seu email”

### Ver o status, se há alguma modificação, como está meu repositório no momento, em qual branch estou

    $ git status

### Adicionar as alterações

    $ git add . || git add --all || git add seu_arquivo

### Escrever o que foi modificado

    $ git commit -m "fazer o comentário"

### Atualizar repositório

    $ git pull

### Mandar para o repositório

    $ git push

## Branch

 - ### Criando uma branch

    $ git checkout -b <nome da branch>

 - ### Acessando uma branch

    $ git checkout <nome da branch>

 - ### Deletar branch

    <p>obs.: tem que estar fora da branch que quer deletar</p>

    $ git branch -D <nome da branch>

### Comparar dois arquivos  ou duas _branches_  antes de passarem por um commit ou um push.
  

 - comparando o repositório ativo com o repositório local:  

    $ git diff HEAD <nome_do_arquivo
 - comparando duas ramificações:  

    $ git diff <_branch_ de origem> <_branch_  de destino>

### Detalhes específicos sobre um commit

    $ git show <hash_do_commit>

### Desfaz todas as modificações do commit

    $ git revert <hash_do_commit>

### Armazenar temporariamente seus arquivos modificados em uma área

    $ git stash


### Integra as mudanças de duas _branches_ diferentes em um único _branch_. 
<p> Obs: Ele precisa ser iniciado a partir de um _branch_ já selecionado, que será mesclado com outro, com o nome passado por parâmetro. </p>
  
    $ git merge <nome_do_branch>

### Integra duas _branches_ em um _branch_ único. Porém, esse comando refaz o histórico de commits, tornando-o linear

    $ git rebase <base>
    $ git pull –rebase
    
### Comando help para trazer ajuda diretamente no terminal

    $ git help
