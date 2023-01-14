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
  
`git diff`  
Apresenta as linhas modificadas dos arquivos  
  
`git log`  
Apresenta o histórico de commits  
  
`git branch`  
Apresenta a branch atual  
  
## Revertendo modificações
`git reset [arquivo]`  
Retorna o arquivo para a staged area  
  
`git reset --soft HEAD~1`  
Retorna ao último commit, mantendo as alterações feitas nos arquivos  
  
`git reset --hard HEAD~1`  
Retona ao último commit, removendo as alterações feitas nos arquivos

`git reset --soft [id do commit]` / `git reset --hard [id do commit]`  
Retorna ao commit do ID especificado, mantendo as alterações (soft) ou removendo as alterações (hard)  
