---------------------------Commands to HELP---------------------------

$ git help (command to help us) <br/>

$ git help init (the description of the command)



---------------------------Commands to INIT and COMMIT---------------------------

$ git init ("" to create in the currently directory or c:\path\..." to create a repository in the specific directory)

$ git add ("." to add everything or "specific_name" to add a specific content)

$ git commit (Insert a commentary and press ESC and write ":wq" to save and exit)
$ git commit -m "Your commentary"

$ git push


$ git commit --amend (vai alterar o último commit)



---------------------------Commands to CHECK some information---------------------------

$ git status (To check the repository status)

$ git log (To check the commits)



---------------------------Commands to check DIFFERENCE---------------------------

$ git diff (to check if there is difference between commits and branches)

$ git diff HEAD~"number" (check difference between a specific commit or branch)



---------------------------Commands to GET a project---------------------------

$ git clone <URL>

$ git pull


---------------------------Commands (Checkout)---------------------------

$ git checkout <commit> <file> (navegação no histórico do repositório)

(bom para ver bugs, dar checkout em um commit antigo e compilar o código)

$ git checkout -- <path_or_file> (To undo changes)
               -- .

$ git checkout HEAD -- <path_file> (que já estão no STAGE)


---------------------------Commands to REVERT/RESET changes ---------------------------

$ git revert <commit> (útil para desfazer um commit antigo, cria um novo commit que desfaz as alterações do commit especificado)

(faz exatamente o contrário daquele commit)

$ git reset <commit> (resetar o repositório para um determinado commit)

$ git reset -- hard --soft <commit> (resetar  e remover todas as alterações)

(útil para desfazer últimos commits)


---------------------------Commands---------------------------

$ git branch (checar qual branch estamos)

$ git status

$ git branch <nova_branch> (para criar uma nova branch)

$ git checkout -b <nova_branch> (cria e muda para a nova branch)

$ git branch -d <branch> (para excluir uma branch)

$git checkout <branch> (mudar para uma branch)


---------------------------Commands---------------------------

$ git merge <branch> (aplicar os commits de uma branch na branch atual)

(os commits da branch especificada serão aplicadas antes da branch atual)

$ git rebase <branch> (usá-lo quando há chance de poucos ou nenhum conflito)

$ git rebase --continue

$ git fetch

(fetch + rebase + continue)

(pull = fetch + merge)

(fetch e rebase é melhor para manter o histórico do desenvolvimento)


---------------------------Commands---------------------------

$ git tag <nome da tag>

$ git push <remote> <tag>

$ git push origin v1.0 (para criar uma nova tag no github)

(realiza o controle de versão, outra opção é fazer com branch, é melhor em casos de bug fix)

(tag = release)

(Tag útil para definir versões estáveis do projeto)

(Semelhante a Branch, porém não recebe mais commits)

(Guarda um estado do repositório)

---------------------------Commands---------------------------

$ git fetch origin pull/<ID>/head:<BRANCH>

(ID da pull request)

(aceitar o merge do pull request dentro do github)

---------------------------Commands---------------------------

$ git stash <list_or_pop>

(para guardar as alterações do Working Directory)

(por exemplo quando você deseja trocar de branch para fazer algum teste, mas não quer realizar um commit)


$ git cherry-pick <commit>

(aplica as alterações de um commit na branch atual)

(cria um novo commit)

(Útil para recupera histórico)


---------------------------Commands---------------------------

$ git blame

(Mostra as alterações feitas em um arquivo por linha)

(Mostra o autor e o commit que foi feito aquela linha)

(Útil para verificar quando as alterações foram feitas, por que e por quem)


---------------------------Commands---------------------------

$ git bisect

(Permite fazer uma busca binário nos commits para encontrar uma alteração)

(Útil para alterações que modificaram o comportamento e não podem ser identificadas por código facilmente)

(Quando a alteração pode ser bastante antiga)


-----------------------------------------------------

www.git-game.com

gitkraken


