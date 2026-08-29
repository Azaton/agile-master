---
title: "Procedimento Repositório"
nav_order: 6
parent: "DevOps"
---

# Procedimento Repositório Git

*De uma forma simples, como criar um repositório, conectar e upar os arquivos?*

### 1 - Criar Chave SSH

Devemos atribuir uma forma automatizada de conectar ao repositório no GitHub. Para isso, se faz necessário criar uma Chave SSH para clonar e upar arquivos no repositório. 

A chave fica armazena por padrão na pasta do usuário do seu Sistema Operacional. No meu caso, no Windows fica em: C:\Users\usuário\.ssh

Então você deve: 

`thime/..` *# Acessar o caminho* 

`$ ls -a ~/.ssh` # Listar todos os arquivos e verificar se existe uma chave pública
`ls: cannot access '/c/Users/thime/.ssh': No such file or directory` # aparece esta mensagem, pois ainda não criamos a chave.

Para criar a chave pública, basta executar o comando $ `ssh-keygen -t ed25519 -C "email@dominio.com.br"` # cria chave e ed25519 é um tipo RSA.

`$ eval "$(ssh-agent -s)"` # Este comando é usado para iniciar o agente SSH no Git Bash, o que permite autenticação segura ao se conectar a servidores remotos usando chaves SSH. É gerado um PIN de autenticação `Agent pid 0000` 

`$ cat id_ed25519.pub` # Este comando serve para mostrar o conteúdo do arquivo. Copie a chave e cole no caminho no: GitHub > Profile > Settings > New SSH and GPG key. Desta forma será possível você conectar no repositório, clonar e atualizar de forma automatizado o repositório.

### 2 - Clonar Repositório

Criar repositório público no GitHub.

Abrir a pasta onde deseja colocar o repositório e no terminal, digite `$ git clone "git@github.com:Azaton/Nome_do_Repositório.git"`.

![image.png]({{ site.baseurl }}/.attachments/image-53953b63-a064-448d-b751-9e39f767d847.png =280x)

Verificar como está a conexão no diretório via comando  `$ cat config` para verificar se tem [core], [remote “origin”] e [branch “main”].

`$ cat config
[core]
repositoryformatversion = 0
filemode = false
bare = false
logallrefupdates = true
symlinks = false
ignorecase = true
[remote "origin"]
url = [git@github.com](mailto:git@github.com):Azaton/Nome_do_Repositório.git
fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
remote = origin
merge = refs/heads/main`

### **3 -  Upar Arquivos no Repositório**

Manipule arquivos, edite-os ou crie novos arquivos na pasta do repositório que foi clonado. Depois execute `$ git status` > será mostrado os arquivos que sofreram modificações.

Executar o comando `$ git add .` > para upar todos os arquivos para o commit.

Executar o comando `$ git commit -m”upando arquivo via bash comandos”` > para commitar as subidas que serão feitas. 

Executar o comando `$ git push` > para enviar ao repositório no GitHub.

### 4 - Criando as branchs

**user@ (main)**
`$ git remote add upstream https://github.com/elidianaandrade/dio-lab-open-source.git`

*# na master, executar o comando: adicionando um novo repositório remoto chamado "upstream" ao seu repositório Git local. No Git, um repositório remoto é uma cópia do repositório Git hospedado em um servidor remoto.*

**user@ (main)**
`$ git remote -v` 

*# O comando "git remote -v" é útil para verificar rapidamente as configurações de repositórios remotos associados a um repositório Git local.*

`origin  [git@github.com](mailto:git@github.com):Azaton/dio-lab-open-source.git (fetch)
origin  [git@github.com](mailto:git@github.com):Azaton/dio-lab-open-source.git (push)
upstream https://github.com/elidianaandrade/dio-lab-open-source.git (fetch)
upstream https://github.com/elidianaandrade/dio-lab-open-source.git (push)`

**user@ (main)**
`$ git checkout -b feat/community/azaton`

*# cria a branch* 
Switched to a new branch 'feat/community/azaton'