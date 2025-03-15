# Comandos mais usados no dia a dia para Git/GitHub

## --Criando e clonando repositórios:
### **git init**
> Para criar um novo repositório, você vai usar o comando git init. git init é um comando único que você usa durante a configuração inicial de um novo repositório. A execução desse comando cria um novo subdiretório .git no > diretório de trabalho atual.
### **git clone < URL >**
> Se um projeto já foi configurado em um repositório central, o comando clonar é a forma mais comum para os usuários obterem um clone de desenvolvimento local. Como o git init, a clonagem é geralmente uma operação única.

## --Salvando alterações no repertório local:
### **git add**
> O comando git add adiciona alterações a um arquivo.
### **git commit -m"descrição"**
> O comando git commit captura um instantâneo das mudanças preparadas do projeto no momento. Os instantâneos com commit podem ser considerados versões "seguras" de um projeto, o Git nunca os altera, a menos que você peça a > ele.

## --Desfazendo alterações no repertório local:
### -**git restore**
> O comando git restore restaura arquivos para o estado de um commit anterior, sem alterar o histórico de commits.
### Estrutura principal: git restore < nome do arquivo > 

### -**git reset**
> O comando git reset desfaz alterações no repositório do Git, movendo o indicador de referência HEAD para um commit específico. Ele também pode modificar o Índice de staging e o Diretório de trabalho. 
### Estrutura principal: git reset --< Tipo > < hash do repositório >
### Tipos:
## Soft ##
> Não toca no arquivo de índice ou na árvore de trabalho (mas redefine a cabeça, ou HEAD, assim como todos os modos). Isso deixa todos os seus arquivos alterados como "Mudanças a serem comitadas", como o status do git colocaria.
## Mixed ##
> Redefine o índice, mas não a árvore de trabalho (ou seja, os arquivos alterados são preservados, mas não marcados para confirmação) e relata o que não foi atualizado. Esta é a ação padrão. Se -N for especificado, os caminhos removidos são marcados como intenção de adicionar.
## Hard ##
> Redefine o índice e a árvore de trabalho. Quaisquer alterações nos arquivos rastreados na árvore de trabalho são descartadas.

## --Trabalhando com branch
> Basicamente, a main fica "apontada" para o último commit realizado nela, ao criar outra branch pode-se modificar a mesma da maneira que desejar sem nem mesmo tocar no branch main( principal ) e para trazer as alterações para a main so meclar a branch com as alterações com a main.

### git checkout < nome da branch que desejo voltar > ###
### git checkout -b  < nome da nova branch > ###
### git branch -v ###
> Mostra quantas branch's tem e em quais commits estão.
### git merge < nome da branch que deseja mesclar > ###

## --Outros comandos importantes
### git congif --global user.name"nome" ###
### git congif --global user.email"email" ###
### git status ###
### mkdir < nome repositório > ###
> cria pastas( repositórios )
### git log ###
> Mostra o hitorico dos commits dados pelo usuário.
### git commit --amend -m"aqui você coloca a nova descricao do commit"###

