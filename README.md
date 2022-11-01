# Anotações sobre git

## Iniciando repositório
 > git init -> Inicializa um repositório 

## Realizando um commit
 > Um commit possui um conjunto de passos a serem seguido: 
  >>1.  git init --> inicia o repositório
  >>2. git status --> mostra o status das alterações, desde as preparadas para realizar o commit como também as que não foram preparadas.
  >>3. git add <caminho-do-arquivo> --> Vale lembrar que, adicionando "." ele adiciona todos os arquivos a staged area.
  >>4. git commit -m "mensagem informando o que foi feito"
  >>5. git push --> Adiciona o commit ao repositório na nuvem.

## Criando novas branches
> Ao criar uma branch, estamos criando ramificações diferente da principal. Assim, o git cria um novo ponteiro que apontará para essa nova ramificação.
> É através do HEAD que o git sabe em qual branch está
> git branch nome-da-branch --> cria uma nova branch
> Ao executar o comando de criação de uma nova branch, ele cria apenas a branch, mas ainda não aponta aponta para ela.

> git log --oneline --decorate --> mostra quais branches estão disponíveis. 

### Alterando entre branches
> O comando *git checkout nome-da-branch* faz com que o HEAD aponte para a branch que foi especificada.
> Vale lembrar que, ao realizar a troca de branch, os arquivos também irão mudar, ou seja, será mostrado os arquivos que foram commitados na branch em que se encontra.

> Com o comando *git checkout -b nome-da-nova-branch* ele cria e ao mesmo tempo muda para a branch criada.
