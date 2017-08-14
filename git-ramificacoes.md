# Ramificações no Git

## O que são os _branches_

Um projeto desenvolvido através do Git pode ser comparado ao galho de uma árvore. No galho, existe uma estrutura central com diversas ramificações, que se tratam de galhos menores. Comparando com o Git, a estrutura central do galho trata-se do andamento principal do projeto, ao passo que suas ramificações são modificações que se diferenciam do galho central. Esses "galhos" são chamados de "branches", ou seja, são caminhos alternativos que surgem ao longo do controle de versão.

Com a existência de vários branches em um mesmo projeto, vários deles podem ser trabalhados pelos desenvolvedores envolvidos. Isso ocorre com auxílio do ponteiro denominado "Head", que indica qual é o branch no qual o usuário do git esta trabalhando no momento. O branch para o qual o "Head" aponta é aquele que irá seguir os comandos e commitar as modificações feitas pelo desenvolvedor.

## Como criar um branch

Em termos técnicos, o branch trata-se de um ponteiro localizado em certa parte do projeto git. Através do comando `git branch`, cria-se um ponteiro no commit mais recente do projeto no git.
```
git branch nomeBranch
```
Com a criação do novo branch, para que o ponteiro "Head" aponte para ele é necessário usar o comando `git checkout`.
```
git checkout nomeBranch
```
Agora, as modificações feitas no projeto estarão no novo branch.

Para criar um branch e apontar o "Head" para o mesmo em um só comando, basta usar o `git checkout -b`.
```
git checkout -b nomeBranch
```
## Como mesclar dois branches

O processo de união de dois branches é chamado de "merge". Com o fim das modificações nos branches e com a necessidade da união deles, basta usar o comando `git merge`, que une o branch especificado pelo comando ao branch apontado pelo "Head".
```
git checkout master
// aponta o Head para o branch master
git merge nomeBranch
// faz a união do master com o nomeBranch
```

É interessante ressaltar que, em dois branches diferentes, quando há modificações em linhas iguais, haverá um conflito no merge. Nesse caso, haverá uma pausa no processo de unificação que só termina com a resolução do conflito.

As modificações conflituosas podem ser identificadas e encontradas pelo git através do `git status`. O arquivo conflituoso estará acompanhado da mensagem `unmerged:`
```
unmerged: arquivo.md
```  
Além disso, dentro do arquivo conflituoso, no exato local de conflito, haverá uma indicação evidenciando-as.
```
<<<<<<< HEAD:arquivo.md
Aqui haverá a modificação no branch apontado pelo Head.
=======
Aqui haverá a modificação no branch unificado pelo git merge.
>>>>>>> nomeBranch:arquivo.md
```
Para resolver o conflito, basta fazer as modificações no arquivo apagando a parte que não se deseja manter e executando o `git add`, `git commit`, etc para o dado arquivo.

## Como excluir um branch

Para apagar o branch, basta usar o comando `git branch -d`

```
git branch -d nomeBranch
```
