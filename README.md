# projeto-curso-git

NO APRENDIZADO ATÉ AQUI EM GIT E GITHUB SOBRE BRANCH:

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$  git branch
* master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$  git checkout master --> Este comando sai da Branch atual para ir a Branch master...
Already on 'master'
Your branch is up to date with 'origin/master'. --> Como só existe esta - ele diz que já é a principal

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch --> Este Comando mostra a Branch Principal no Momento...
* master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch contato --> Este comando está criando uma nova Branch "contato"...
g
WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch fornecedor --> Este comando está criando uma nova Branch "fornecedor"...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch --> Este Comando mostra a Branch Principal no Momento...
  contato
  fornecedor
* master

*** ABAIXO, TEMOS OUTROS EXEMPLOS DE COMANDOS VÁLIDOS ***

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch -b fornecedor
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged | --no-merged]
   or: git branch [<options>] [-l] [-f] <branch-name> [<start-point>]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track           set up tracking mode (see git-pull(1))
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display SHA-1s

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --format <format>     format to use for the output

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git checkout -b institucional --> Este comando criar uma nova Branch e já a coloca como sendo a Principal...
Switched to a new branch 'institucional' --> Resposta de Sucesso da criação da Branch...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (institucional)
$ git branch --> Este Comando mostra a Branch Principal no Momento... No caso: "institucional"
  contato
  fornecedor
* institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (institucional)
$ git branch master --> Se colocarmos este comando para voltar para a Branch master ele vai dizer que já existe...
fatal: A branch named 'master' already exists.
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (institucional)
$ git checkout institucional --> Usamos o "git checkout" e o nome da branch que queremos que seja a principal...
--> Se colocarmos este comando acima para sair da Branch Principal ele vai dizer que já está na Branch institucional
Already on 'institucional'

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (institucional)
$ git branch --> Confirmamos qual é a Branch Principal, No caso: "institucional"...
  contato
  fornecedor
* institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (institucional)
$ git checkout contato --> Alteramos a Branch Principal, No caso: "institucional" para a Branch: "contato"...
Switched to branch 'contato'

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git branch --> Verificamos se a Branch Principal foi alterada, No caso, agora é: "contato"...
* contato
  fornecedor
  institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git checkout master --> Se quisermos voltar para a Branch master com este comando também dá erro...
Switched to branch 'master'
Your branch is up to date with 'origin/master'. --> Informa que ela é a Branch: "origin/master" e Altera a Branch...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch
  contato
  fornecedor
  institucional
* master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git status --> A consulta de "git status" informa que não há nenhum inserção commitada...
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git checkout contato --> Alteramos a Branch: "master" para a Branch: "contato"
Switched to branch 'contato'

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git branch --> Agora estamos confirmando em qual Branch estamos... No caso: "contato"
* contato
  fornecedor
  institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git checkout master --> Alteramos a Branch: "contato" para a Branch: "master"
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch --> Agora estamos confirmando em qual Branch estamos... No caso: "master"
  contato
  fornecedor
  institucional
* master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git branch contato --> Tentando criar uma Branch já existente...
fatal: A branch named 'contato' already exists. --> Resposta, de que a Branch "contato" já existe...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (master)
$ git checkout contato --> Voltaremos para a Branch "contatos"
Switched to branch 'contato' --> Resposta de que foi (Switched) Comutado ou Alterado com Sucesso...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git branch --> Consultamos, a alteração antes de fazer qualquer outra Ação...
* contato
  fornecedor
  institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ touch contato.html --> Agora, estamos criando um arquivo dentro da Branch (Ramo) "contato"...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git status --> Consultando o Status atual...
On branch contato
Untracked files:
  (use "git add <file>..." to include in what will be committed) --> Dica para incluir no Rastreamento do GIT
        contato.html --> VAI ESTAR NA COR VERMELHA...

nothing added to commit but untracked files present (use "git add" to track)
--> Avisando que os arquivos foram inseridos no Diretório local, mas não estão sendo rastreados...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git branch --> Consultando o status atual...
* contato
  fornecedor
  institucional
  master

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git add contato.html --> Adicionando o arquivo contato.html para ser rastreado no Git... Tracked

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git status --> Consultando o status atual...
On branch contato
Changes to be committed:
  (use "git restore --staged <file>..." to unstage) --> Fornecendo a opção de restaurar ou deletar o que foi feito...
        new file:   contato.html

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git commit -m 'Criando arquivo contato.html na Branch(Ramo) de Contato'

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git commit -m 'Criando arquivo contato.html na Branch(Ramo) de Contato'
[contato f81c8f4] Criando arquivo contato.html na Branch(Ramo) de Contato
 
	1 file changed, --> 1 arquivo alterado
	0 insertions(+), 
	0 deletions(-)
	create mode 100644 contato.html

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git status --> Consultando o status atual...
On branch contato
nothing to commit, working tree clean --> informa que não há mais alterações a serem realizadas...

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git log --> Este comando verifica o log de alterações de todos os envolvidos e rastreamento...
commit f81c8f44bfa03bada43944aba03c2cb9a481b908 (HEAD -> contato)
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Tue Apr 7 17:08:37 2020 -0300

	*** ABAIXO TEMOS A SEQUENCIA DE ALTERAÇÕES E RASTREIO - DE BAIXO PARA CIMA ***

    Criando arquivo contato.html na Branch(Ramo) de Contato --> Última Alteração...

commit 2a4bb09547e4e060104657cf74fbab5fce170da9 (origin/master, master, institucional, fornecedor)
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Tue Apr 7 15:20:04 2020 -0300

    Inserindo novas Tags "H3" e Estilizando palavras chaves com "CSS" na Tag "span"

commit c054f33a52441625850bef8db987a06b80a90185
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Tue Apr 7 15:04:03 2020 -0300

    Estilizando as tags P

commit b02f7b62e616b41487f6382c0611c9de82603153
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Tue Apr 7 13:04:31 2020 -0300

    Treinando as Alterações nas tag P adicionando no git e commitandono GitHub...

commit 44bd6f537bf6e4f9c16035187cbd50f61b109c60
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Tue Apr 7 12:56:06 2020 -0300

    Adicionamos estrutura inicial no index.html e criamos o arquivo com estrutura no CSS/style.css

commit 42b94ce570b109950c656330ea0f4e0d3a2d48eb
Author: hamamellis <wagnerhamamellis@gmail.com>
Date:   Mon Apr 6 18:56:21 2020 -0300

    Meu Primeiro commit criando um arquivo.html --> Primeira alteração
(END)

WAGNER@WagnerBarros MINGW64 /e/Projetos VSCode/Curso-Git/projeto-curso-git (contato)
$ git push origin contato --> AQUI INSERIMOS A BRANCH CONTATO CRIADA NO REPOSITÓRIO REMOTO DO GITHUB...

