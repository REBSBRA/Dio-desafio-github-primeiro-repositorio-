## Desafio de Projeto sobre Git/GitHub da DIO
Repositório para o Desafio do Projeto

## Links Relacionados

[Dowload do Git](https://git-scm.com/downloads)

[Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/)

[Adicionar imagem no GitHub](https://www.youtube.com/watch?v=oMFiGEZ6UlQ)

📌Criando um novo projeto

1. Crie uma nova pasta no seu PC 
2. Abra o VSCode na pasta criada
3. Crie novo arquivo `README.md`
5. Dê nome ao seu arquivo e salve

Usando o Git

- Abra o `git bash` que foi instalado
- `git init`para que o repositório seja inicializado
- `git add README.md`coloca o arquivo na área de staging  (área intermediária)
- `git commit -m "nome do arquivo"` para que o commit vá para o repositório
- `git brach -M "main"` esse comando altera o nome da brach principal master > main  

📌Criando um repositório no GitHub

- Após criar sua conta na plataforma, você criará um `novo repositório`

Preencha com as informações do seu projeto; adicione um nome ao repositório; coloque uma breve descrição e por fim, crie o repositório
<img src = "https://user-images.githubusercontent.com/103836478/164515714-4bccdd1b-5c35-477d-be81-8a41a9570884.png">

<img src = "https://user-images.githubusercontent.com/103836478/164520549-4e9b422b-ecc7-487f-977a-f463eab163ef.png">

- Vá até seu repositório > code > copia o link HTTPS

- Para passar o commit do seu repositório local, ou seja, da sua máquina para um repositório remoto (plataforma GitHub), usamos o `git remote add origin <link do repositório>`
- `origin`  é utilizado para referenciar o nosso repositório

Agora temos o repositório local conectado ao repositório do GitHub, contudo o `commit`  que damos na nossa máquina não sobe automaticamente para a plataforma. Precisamos dá um empurrão.

- `git push -u origin main`

Pronto, ao recarregar a página, veremos o nosso arquivo na plataforma do GitHub 

💡 Adicionando e alterando arquivos

- Adicione uma frase no arquivo criado 
- Para criar um novo arquivo `README.md`, escreva por exemplo, `esse é o arquivo onde irei desenvolver o projeto x`
- Agora vamos adicionar essas informações no nosso GitHub através do comando `git add .(O `.`  é responsável por adicionar todos os arquivos) e o comando `git commit -m "Primeira alteração"` 

Obs: para alterarmos algo no nosso repositório do GitHub, precisamos dar o comando `push`, ou seja `git push origin main`

💡 Branch

Como criamos uma Branch?????

- Vamos adicionar um novo arquivo para desenvolver o `botão` de interesse
- `git checkout -b "novo-botão"`  e assim criamos a brach para ele 
  - (Além de criar uma branch, esse comando permite entrar nela através do checkout)
- Crie o arquivo `botão.md` "crio o botão"
- Coloque a alteração em stagging com o `git add .` 
- Commita com o `git commit -m "novo botão"`
- Para enviar o arquivo da sua máquina para o GuitHub, o comando executado será `git push origin main.` O `main` é referente a brach principal. EX: `git push origin botão`

💡 Merge

- Agora vamos até nossa Branch principal. Utilize o comando `git checkout main` lá faremos o merge com a branch, ou seja o `botão` que criamos, através do `git merge botao`
  - Pronto, agora as alterações que estavam na branch `botão` está junto da `main`
  - Agora vamos utilizar o comando `git push origin main` para empurrar tudo para o GitHub

💡 Clone

Como se pode baixar um código????

- Sempre que você entrar em um repositório, sendo o seu ou de outra pessoa, terá uma opção chamada `Code`. Ao clicar nele, irá abrir essa opção:

<img scr = "https://user-images.githubusercontent.com/103836478/164520549-4e9b422b-ecc7-487f-977a-f463eab163ef.png">

- Copie o link `HTTPS` e leve para o seu terminal
- Use o comando `git clone e o link https` do repositório que você quer clonar, para puxar o projeto para a sua máquina
- Prontinho, o projeto será clonado

💡 Pull

- Esse comando `Pull` nos ajuda a puxar as alterações feitas no repositório GitHub para o seu repositório local. Ou seja, se você fizer uma alteração no seu repositório do GitHub, utilizando o comando `git pull` conseguirá passar tudo para a sua máquina. 

📌 Comandos extras

⭐ Criando um repositótio no terminal

1. Faça uma pasta na sua máquina para salvar o seu repositório 
2. `git bash`
3. `ls`
4. `cd e nome da pasta que você criou /`
5. `mkdir e o nome da sua pasta`
6. `cd e o nome da pasta`
7. `git init`
8. `ls -a`
9. Pronto, seu repositório foi criado

Legenda

- O comando `ls` lista 
- `Ctrl l` limpa a página no git bash
- `mkdir` cria uma pasta dentro de outra
- `cd e o nome da pasta`entra na pasta
- `git init` para iniciar o git na pasta
- `ls -a` mostra os arquivos que estão ocultos

⭐ Criando o primeiro arquivo dentro de outra pasta

Se for a primeira vez que está criando algum conteúdo no Git, ele vai te pedir algumas informações, para isso siga esses passos:

1. `git bash`
2. `git config --global user.email "email"`
3. `git config -- global user.name "seu username"`
4. Pronto, sua configuração inicial foi realizada

⭐ Movendo uma pasta para a outra

1. `ls`
2. `git status`
3. `mkdir e o nome da pasta`
4. `mv "nome da pasta 1" .md ./ nome da pasta 2/` ex: (mv "torta de frago".md ./ comidas/)
5. `Ctrl l`
6. `echo > Readme.md`
7. Prontinho

Obs: O git vai passar a seguinte mensagem "sua pasta foi deletada", porém, a pasta foi apenas removida para dentro de outra pasta. O sistema não entende, por isso passa a mensagem como se a mesma tivesse sido deletada. 

⭐ Criando uma pasta README

1. `echo > Readme.md`
2. `ls`
3. `git status`
4. `git add*`
5. `git commit -m "adiciona index"`
6. Pasta criada

⭐ Para adicionar um repositório

1. Vá até o GitHub e crie um repositório
2. Copie o `https` do repositório 
3. Abra o `git hash` na pasta de seu interesse
4. `git remote add origin e cola o link https`
5. `git remote -v`
6. `git push origin master`
7. `username e password`
8. Prontinho

⭐ Git Clone

1. Crie um repositório no GitHub
2. Copie o `https`do seu repositório
3. Crie uma pasta na sua máquina para clonar o seu repositório
4. Entre no `Git Bash`
5. `git clone e cola o https do repositório`
6. `git status`
7. Prontinho 

📌Principais comandos do Git

- `git config --list` = Lista as configurações do git; estando dentro do repositório, lista mais itens
- `git config --global user .name "Meu nome"` = Define o nome do usuário para o git
- `git config --global user .email "email@gmail.com"` = Define o e-mail do usuário para o git (precisa ser o email cadastrado no GitHub)
- `git config --global core.editor vim` = Define o editor de texto padrão para abrir automaticamente os arquivos do git
- `git init` = Inicializa um repositório
- `git status` =  Vê o estado atual do projeto
- `git add arquivo.txt` = Adiciona o arquivo arquivo.txtao projeto
- `git commit -m "Minhas mudanças efetuadas"` = Armazena as mudanças efetuadas e descreve o que foi alterado
- `git log` = Mostra todas as mudanças que foram efetuadas (commit, autor,data)
- `git push -u origin master` = Envia todos os arquivos modificados e commitados para o repositório do github
  - `-u` = Faz com que o git armazene os comandos e na próxima vez basta utilizar o git push
  - `origin` = Diz que o respositório no github possui o mesmo nome do projeto/diretório que você está enviando
  - `master` = É o nome da branch (indicador) 
- `git pull origin master` = Verifica as mudanças efetuadas por outro colaborador do projeto
- `git diff HEAD` = Verifica as partes dos arquivos alterados no último commit
- `git reset arquivo.txt` = Remove um arquivo do projeto
- `git checkout - arquivo.txt` = Defaz a última alteração feita no arquivo
- `git rm "*.txt"` = Remove 1 ou mais arquivos utilizando "curinga"
- `git clone https://github.com/user/project.git` = Copia o repositório para sua máquina
- `info git` = obtém a documentação do git
- `man git` = obtém o manual do git 

🎯 Opções de comandos com o add

- `git-add` = É o mesmo comando do git add (o comando git-addnão irá adicionar arquivos ignorados por padrão a menos que seja utilizado o parâmetro-f)
- `git add -a` = Adiciona todos os arquivos que foram modificados
- `git add * .txt` = Adiciona todos os arquivos .txt que foram modificados
- `man git-add` = manual competo sobre git-add

 

