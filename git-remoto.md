Caso seja interessante saber quais foram os commites enviados ao repositório até o momento, basta digitar "git log".

Se, além dos commites, deseja-se saber quais foram as modificações exatas nos arquivos que estão no Git Directory, basta digitar "git log -p". Esse comando pode ser encarado como uma mistura do "git diff" com o "git log".

Como o "git diff" e o "git log"(juntamente com suas variações) são mostrados pelo terminal, muitas vezes a análise das mudanças nos arquivos através desses comandos torna-se pouco produtiva. Para resolver esse problema, também existe o comando "gitk", que da acesso à interface gráfica do Git. Com essa interface, pode-se analisar todas as mudanças nos arquivos de forma clara e objetiva.

Após terminar o projeto, para enviar o projeto para o github.com(site no qual outros membros da sua equipe podem ver suas modificações), basta, na pagina inicial do github.com, clicar em "new repository" e, após nomea-lo, enviar suas modificações através dos comandos

git remote add origin endereço da página no git
git push -u origin master

#### exemplo:

#### git remote add origin h ttps://github.com/Fulano/projeto-.git
#### git push -u origin master
