# Comandos Git

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

## Diferença entre arquivos
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
