# Comandos Git

<img src="https://user-images.githubusercontent.com/77423877/212448635-0d5a1db3-1480-4910-baa8-971115cd06a4.png" width=550>

## Configurações
`git config --global user.name "[nome]"`  
Configura o nome relacionado aos commits  
  
`git config --global user.email "[endereco-de-email]"`  
Configura o email relacionado aos commits  
  
`git config --list`  
Lista as configurações atuais  

## Comandos básicos
`git init`  
Inicializa um repositório git  
  
`git status`  
Verifica o status dos arquivos/diretórios e as modificações realizadas  
  
`git add [arquivo]`  
Adiciona o arquivo à staged area  
  
`git add .` ou `git add -A`  
Adiciona todos os arquivos modificicados à staged area  
  
`git commit -m "Mensagem do commit"`  
Armazena os arquivos que estão na staged area para um novo commit, gravando-os no histórico de versão  
    
`git log`  
Apresenta o histórico de commits  

## Diferenças de arquivos
`git diff`  
Apresenta as linhas modificadas dos arquivos  
  
`git diff --name-only`  
Apresenta os nomes dos arquivos que foram modificados  
  
`git diff [arquivo]`  
Apresenta as linhas modificadas no arquivo especificado no comando  

## Revertendo modificações
`git reset [arquivo]`  
Retorna o arquivo para a staged area  
  
`git reset --soft HEAD~1`  
Retorna ao último commit, mantendo as alterações feitas nos arquivos  
  
`git reset --hard HEAD~1`  
Retona ao último commit, removendo as alterações feitas nos arquivos

`git reset --soft [id do commit]` / `git reset --hard [id do commit]`  
Retorna ao commit do ID especificado, mantendo as alterações (soft) ou removendo as alterações (hard)  

## Branches
`git branch [nome-da-branch]`  
Cria uma nova branch  
  
`git branch`  
Apresenta as branches existentes e destaca a branch atual  
  
`git checkout [nome-da-branch]`  
Muda para a branch informada no comando  
  
`git merge [nome-branch]`  
Integra as mudanças da branch especificada no comando com o histórico da branch atual  
  
`git branch -D [nome-branch]`  
Remove a branch do repositório local  
  
`git push [nome-remote] :[nome-branch]`  
Remove a branch do repositório remoto

## Repositório remoto
`git remote add [nome-remote] [url-remote]`  
Vincula o repositório remoto ao repositório local  
  
`git remote` / `git remote -v`
Apresenta os repositórios remotos  

`git remote rm [nome-remote]`  
Desvincula o repositório remoto do repositório local  
  
`git remote set-url [nome-remote] [url-novo-remote]`  
Altera o repositório remoto vinculado ao repositório local  
  
`git push -u [nome-remote] [nome-branch-local]`  
Envia os arquivos da branch do repositório local para o repositório remoto (utilizado no primeiro push)  
  
`git push`  
Envia os arquivos da branch do repositório local para o repositório remoto (utilizado do segundo push em diante)  
  
`git pull [nome-remote] [nome-branch-local]`  
Envia os arquivos do repositório remoto para a branch do repositório local  
  
`git fetch`  
Busca as alterações feitas no repositório remoto, sem adicioná-las ao repositório local  
  
`git clone [url-remote]`  
Clona um repositório remoto para o repositório local  
