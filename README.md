git –version
//setando info do user
git config –global user.name “Juliano Appezzato”
git config –global user.email “juliano.appe@gmail.com”
git config –global core.editor vscode   //define o editor que vc usa

//exibindo os dados
git config user.name
git config user.email
git config –list   //lista todos os dados do usuario

git init //cria repo vazio numa pasta oculta
git status // verifica arquivos modificados.
git add –A //adciona no repo todos os arquivos modificados
git add NOME DO ARQUIVO //add somente ele
git commit –m “Descrição...”
git commit –am “Descrição...”  //isso já faz adiciona os arquivos e já faz o commit
git log // exibe todos os commits
git diff //ele exibe todas as modificações no próprio código em detalhes
git diff –name-only //mostra somente os nomes dos arquivos modificados
git diff style.css //mostra só alterações em um arquivo

//REVERTENDO COMMITS
git reset -- soft //volta a alteração anterior porem já preparadas com add
git reset --mixed //ele volta porem sem estar preparado com add
git reset -- hard //ignora tudo removendo todas  as alterações feitas no código, ele apaga o commit do log

//BRANCHS
git branch //exibe as branch, a com * é a atual
git branch NOME DA BRANCH //cria uma branch
git checkout NOME DA BRANCH //altera a branch para essa
git checkout HEAD --  style.css //ele volta as alterações nesse arquivo, HEAD é ref da branch atual

ssh-keygen -t rsa –b 4096 -C “Email@com.com”

git remote add origin https://github.com/JulianoANR/ProjetoIntegrado.git
git branch -M main
git push -u origin main //envia do repo local para o remoto, mais é a branch que vc vai enviar

git remote //mostra  os repo adicionados
git remote –v //exibe os comandos disponiveis
