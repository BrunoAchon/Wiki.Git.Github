--------------------------------------------------------------------------------------------------------------------------------------
Create                                    = a criação do projeto é feita pelo site do github
--------------------------------------------------------------------------------------------------------------------------------------
git init                                  = Cria um Repositorio
git add readme.md                         = cria uma arquivo qualquer para que o projeto nao esteja vazio
git commit -m "first"                     = faz um primeiro commit no projeto para enviar arquivos
git branch -M main                        = cria a primeir branch do projeto (main / master)
git remote add origin "url"               = vincula a origen do projeto ao git
git push -u origin main                   = envia os arquivos para a branch principal
--------------------------------------------------------------------------------------------------------------------------------------
git clone "url"                           = clona um projeto existente do git, criando uma estrutura igual ao repositorio
git clone "url" .                         = clona um projeto existente do git, dentro do diretorio atual aberto
--------------------------------------------------------------------------------------------------------------------------------------
git status                                = verifica a integridade do projeto e aponta os arquivos alterados
--------------------------------------------------------------------------------------------------------------------------------------
git add .                                 = adciona todos os arquivos ao commit comando necessário para sempre incluir arquivos novos
git add "origem/arquivo"                  = adciona 1 arquivo ao commit
git rm "origem/arquivo"                   = remover 1 arquivo do projeto
git mv "origem/arquivo" "destino/arquivo" = mover arquivo de um lugar para outro (pode-se alterar o nome do arquivo tbm)
--------------------------------------------------------------------------------------------------------------------------------------
git commit -a -m"Mensagem"                = comita as alterações selecionadas
git reset                                 = cancela todas as alterações e todos os commits feitos
git reset --hard "origin/main"            = força com que todos os commits sejam cancelados (perde tudo que nao foi push)
git checkout "origem/arquivo"             = remove todas as alterações - não envia nada para o commit do arquivo indicado
git show                                  = exibe informações do arquivo
--------------------------------------------------------------------------------------------------------------------------------------
git pull                                  = Puxa todas as atualizações do projeto
git push                                  = envia todas as atualizações dentro do commit
--------------------------------------------------------------------------------------------------------------------------------------
git branch                                = visualiza branchs existentes
git branch <nome>                         = cria um branch novo
git branch -d <nome>                      = deleta um branch existente (nao deletar -- somente o adm faz isso)
git checkout -b <nome>                    = cria e muda para a branch a ser utilizada
git checkout <nome>                       = muda para a branch a ser utilizada
--------------------------------------------------------------------------------------------------------------------------------------
comentários importantes sobre branch      = sempre criar uma nova branch apartir da main / master para assim possuir sempre
                                            o codigo correto, e dessa forma criar seus testes ou ramificações combase no
                                            que esta sendo usado, sempre comitar os codigos antes de mudar de branchs
                                          > sempre partir da main / master atualizada (utilizar o pull para atualizar)
                                            e apartir dai criar uma branch usando o git branch -d <nome>.
                                          > nunca dar um push para a main / master, somente o adm faz isso, porem pode-se 
                                            dar o pull dela livremente (obrigatorio), os unicos pushs que serão enviados
                                            serão justamente as branchs criadas.
--------------------------------------------------------------------------------------------------------------------------------------
git merge "nome_da_branch"                = une uma branch a outra geranmente unindo 2 trabalhos ou sua branch ao main
--------------------------------------------------------------------------------------------------------------------------------------
git stash                                 = usado para resetar o codigo mas salvar os comandos em uma area de transferencia
git stash list                            = exibe todas as stashs salvas
git stash apply <indice>                  = muda para a stash salva
git stash show -p                         = mostra exatamente quais sao as alteraçõe existentes em casa stash
git stash clear                           = exclui todas as stashs
git stash drop <indice>                   = exclui somente 1 da stash informada
--------------------------------------------------------------------------------------------------------------------------------------
git tag -a <nome> -m <msg>                = cria um checkpoint de um branch
git show <nome>                           = visualiza todas as alterações dentro da tag
git checkout <nome>                       = troca de tag tambem
--------------------------------------------------------------------------------------------------------------------------------------
git push origin <nome>                    = envia uma tag para que outros devs consigam ver e acompanhar seu desenvolvimento
git push origin --tags                    = envia todas as tags
--------------------------------------------------------------------------------------------------------------------------------------
git fetch -a                              = verifica todas as branchs (de outros devs)
git branch                                = visualiza branchs existentes
git checkout <nome>                       = muda para a branch a ser utilizada
--------------------------------------------------------------------------------------------------------------------------------------
git remote                                = serve para mudar o repositorio trakeado, (exemplo: trocar entre o bitbucket e o github)
git remote -v                             = verificar o repositorio trakeado
git remote rm origin                      = remove o provedor de repositorio do origin 
git remote add origin <url>               = incluir novo repositorio 
--------------------------------------------------------------------------------------------------------------------------------------
git diff <arquivo> <arquivo>              = verificar diferenças entre duas branchs
--------------------------------------------------------------------------------------------------------------------------------------
git submodule add <repo>
--------------------------------------------------------------------------------------------------------------------------------------
.gitignore                                = arquivo usado para evitar o envio de outros arquivos
--------------------------------------------------------------------------------------------------------------------------------------