# libGDX


## O que é libGDX ?


  A libGDX trata-se de uma framework java focada na criação de jogos. Ela possui diversas aplicações que facilitam o trabalho de seus usuários, como funções de áudio e de renderização de imagens, mas não se trata de uma engine, dado que não possui interface gráfica como a Unity ou a Unreal. Sendo cross-platform, essa ferramenta de desenvolvimento permite que o jogo criado com ela funcione em diversas plataformas sem haver a necessidade de ter seu código modificado.

  Para instalar a framework basta acessar o link https://libgdx.badlogicgames.com/download.html e clicar em "Download Setup App". É importante ressaltar que, antes de instala-la, a máquina na qual a libGDX esta sendo usada deve possuir uma IDE para o Java(IntelliJ, NetBeans ou Eclipse, por exemplo), o JDK e o Android SDK.

  Nos tutoriais de libGDX vinculados ao treinamento profissional "Desenvolvimento de aplicativos para dispositivos móveis aplicados ao Ensino a Distância na Universidade Federal de Juiz de Fora" será utilizado o Android Studio, cuja IDE é o IntelliJ.


## Primeiros passos com a libGDX

  Com a framework instalada, o computador possuirá o arquivo "gdx-setup.jar", o qual tem uma interface gráfica e serve para dar o passo inicial no projeto que utilizará a libGDX, criando o escopo básico do código e selecionando as plataformas nas quais o jogo irá rodar. Os campos de texto presentes na interface gráfica são os mesmos que apareceriam caso um projeto estivesse sendo utilizado no Android Studio. Ou seja, basta colocar nesses campos o que esta sendo pedido, o nome, o pacote Java, o nome da classe principal, o diretório de saída e o local em que o Android SDK esta localizado no computador. Normalmente o Android SDK já foi localizado pelo gdx-setup.jar, portanto, não precisa fazer modificações neste campo de texto. Após isso, pode-se perceber checkboxs com nomes de plataformas diferentes(IOS, android, html...), elas determinam para quais dessas plataformas o projeto libGDX ira rodar, neste tutorial usaremos apenas *desktop e android*. Logo abaixo, também em checkboxs, é possível ver extensões que podem ser adicionadas ao projeto, ou seja, elementos que complementarão o desenvolvimento com libGDX, neste tutorial usaremos apenas *Box2d*. Após estes passos, basta clicar em "Generate".

  A opção "Generate" cria um projeto Gradle que deve ser importado para a IDE que o usuário de libGDX esta usando. Para fazer isso,*VER COM O IGOR KNOP*. Após a importação, o projeto esta pronto para ser trabalhado. Se o código for compilado, será exibido uma janela com fundo vermelho e a imagem do mascote da libGDX.
