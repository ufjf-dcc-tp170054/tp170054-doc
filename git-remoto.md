# Repositórios remotos

## O que é um repositório Remoto?

É chamado de repositório remoto uma cópia de trabalho que está na internet, na rede ou mesmo em outra pasta. Como exemplo temos os próprios repositórios no GitHub, que inclusive adiciona uma camada extra de controle de acesso ao git.

Com acesso a vários repositórios remotos, as cópias de trabalho podem trocar revisões entre elas. Isso permite aos participantes de um mesmo projeto deixarem seus fluxos de trabalho independentes uns dos outros. Pois cada um pode realizar suas modificações em  suas próprias cópias de trabalho e compartilhar as revisões com colegas de equipe. Isso fortalece a independência entre eles para o avanço do projeto.

## Adicionando um novo remoto

Um repositório pode ter uma grande lista de remotos e cada remoto é referenciado por um nome local único. Para adicionar e remover repositórios remotos, basta usar o comando `git remote`.

Para adicionar um novo remoto, deve-se fornecer um nome e a URL do repositório:

```
git remote add nomeCurto url
```

Por exemplo,para adicionar um remoto hospedado a uma cópia de trabalho local, utilize o comando:

```
git remote add origin https://github.com/Fulano/projeto-exemplo.git
```

## Listando remotos
Para listar todos os repositórios remotos na cópia de trabalho local, basta usar `git remote`. Isso mostrará os nomes dos remotos atualmente configurados.

Se for utilizado `git remote -v`, será exibido também as URLs ds remotos, tanto para operações de envio (_push_) e recebimento (_pull_) associadas à URL dos repositórios remotos.

## Renomeando
O identificador local de um repositório remoto pode ser alterado pelo comando `git remote rename`. Por exemplo:

```
git remote rename nomeantigo nomenovo
```

## Removendo remotos
Para remover uma referência a um repositório remoto, basta usar o comando `git remote rm nomeDoRemoto`. É importante destacar que isso apenas remove a referência do remoto da cópia de trabalho local. Isso não exclui a cópia de trabalho remota.

## Usando diferentes remotos
É possível tanto obter quanto enviar revisões para cópias de trabalho remotas ao especificar o seu identificador para `git push` e `git pull`.

```
git push neworigin
```
```
git pull neworigin
```

# Trabalhando com ramificações remotas
## Enviar uma ramificação local para um remoto
## Obter uma ramificação remota para a cópia local
## Excluir uma ramificação remota
