# Repositórios remotos

## O que é um repositório Remoto?

  É chamado de repositório remoto aquele cujo controle de versão esta na internet ou em outras redes. Como exemplo temos o GitHub, site no qual se encontram os repositórios deste TP. Com acesso a vários repositórios remotos, os participantes de um mesmo projeto podem ter um controle de versão pessoal, além do compartilhado com seus colegas de equipe, o que fortalece a independência entre eles no projeto.


## Adicionando um novo remoto

 Para adicionar um novo repositório remoto, basta usar o comando
"git remote add nomeCurto url"

 *exemplo*:
  git remote add novorign h ttps://github.com/Fulano/projeto-.git

## Listando remotos
 Para listar seus repositórios remotos, basta digitar os comandos "git remote" ou "git remote -v". O primeiro comando mostra apenas os nomes dos remotos, ao passo que o segundo mostra não só os nomes como também o URL do repositório remoto.

## Renomeando e  Removendo remotos
Para renomear um repositório remoto, basta usar o comando
"git remote rename nomeantigo nomenovo"

*exemplo*:
 git remote rename novorign neworigin

 Para remover um repositório remoto, basta usar o comando
 "git remote rm nomeDoRemoto"
*exemplo*:
 git remote rm neworigin

## Usando push em diferentes remotos
Para usar o push em diferentes remotos, basta digitar
"git push nomeDoRemoto"
*exemplo*
git push neworigin
