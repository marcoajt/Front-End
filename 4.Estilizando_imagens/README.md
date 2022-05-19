# Projeto da aula anterior

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/03/aula-3-completa.zip) o projeto do curso no ponto em que paramos na aula anterior.

# Identificador de elemento e tag de imagem

*Você pode baixar um ZIP com a imagem \**banner.jpg** aqui.*

https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/04/banner.zip

[00:00] Vamos começar nossa aula organizando um pouco nosso código, porque ele está bem bagunçado. Tem algumas coisas que não fazem mais sentido. Por exemplo, a tag style, que está vazia. Podemos removê-la.

[00:14] Outra coisa que não está legal é termos CSS no nosso código enquanto temos um arquivo de CSS. O ideal seria movermos todo esse conteúdo para lá. 

[00:27] O h1 é muito fácil. É só recortar o style, voltar para o nosso arquivo de CSS, e, como eu disse anteriormente, sempre tentando deixar a estrutura do CSS parecida com a estrutura do HTML. Temos o body, o h1, e aí o parágrafo. Vamos colocar o h1 e depois o style que tínhamos recortado.

[01:02] Vou apenas colar o que estava lá. Reparem no editor de código funcionando. Ele marcou que tem algo muito errado nessa linha, porque colocamos as aspas e o style, já que eu só recortei e colei. Nós não precisamos deles. 

[01:14] Se eu salvar, voltar para o navegador, recarregar, o código está perfeito. Não tem nada errado. Funcionando do mesmo jeito. Só movemos o CSS.

[01:28] Mas temos um problema com esse CSS, porque ele é específico para um parágrafo. Para resolver isso, precisamos ter uma marcação para o HTML específica para esse elemento, e no CSS referenciar isso. 

[01:49] Usamos para isso o marcador de identificação. É o id. Vamos colocar id = “”. Entre as aspas você coloca um nome qualquer, que é o mesmo que vai ser usado no nosso CSS. 

[02:07] Vamos chamar nosso id de “missao". Vamos recortar o código CSS e colar no arquivo CSS. O “missao" é um dos parágrafos, ele vem logo depois do anterior. E como fazemos para marcar? Toda vez que estamos marcando uma tag e queremos referenciar ela no CSS, usamos o nome da tag. Toda vez que temos um identificador no HTML e queremos referenciar ele no CSS, usamos a #. Logo: #missao. 

[02:50] Reparem que o editor de códigos já marcou com outra cor, para marcar que está certo. 

[02:57] Vamos colar aquele código que tínhamos e salvar. Se recarregarmos o navegador, o código está perfeito. Não tem nada errado.

[03:11] Vamos evoluir esse código então. Vamos adicionar mais conteúdo à página, uma imagem.

[03:21] Essa imagem já está na pasta do projeto de vocês, podem baixar. É uma imagem com cadeiras de barbearia e um balcão atrás. Ela está com o nome “banner.jpg”. 

[03:41] Assim como o CSS, a imagem também é um arquivo externo. Nós colocamos a chamada para o CSS no head, porque é uma informação que estamos passando para o navegador. A imagem é uma informação que queremos exibir na nossa página, então vamos colocá-la dentro do body.

[04:01] Na estrutura visual da nossa página, a imagem vai ser a primeira coisa que vai aparecer. Então, em cima de tudo, vou chamá-la. Usamos a tag img para adição da imagem ao conteúdo.

[04:19] A tag img serve para chamarmos uma imagem, e como ela é um arquivo externo, precisamos dizer onde está, dizer qual a fonte dessa imagem. Para isso, usamos a propriedade source. Só que não escrevemos isso por inteiro. Abreviamos para src e colocamos o endereço: img src=”banner.jpg”.

[04:53] Como essa é uma tag de chamada de arquivo externo, não abrimos e fechamos. Ela é só a definição da tag. 

[05:02] Se salvarmos o arquivo e abrirmos no navegador, recarregando a página, a nossa imagem já está ali. 

[05:12] A imagem é essa tag, com uma fonte e um endereço. 

[05:20] Na próxima aula vamos entender como fazer com que a imagem ocupe toda a largura da página, como fazer ela se posicionar melhor no texto, como brincar com espaçamento, etc. Mas isso fica para a próxima. Aqui, nós vimos como reestruturar nosso código, criar um identificador para marcar especificamente um elemento e adicionar uma imagem à nossa página.

# O caminho da imagem

# Como inserir imagens de forma correta?

Para que a imagem apareça de forma correta, fique atento nesses pontos:

- Nome do atributo da tag é src

```
<img src="banner.jpg">
```

O atributo **src** caso escrito de outra forma, a imagem não será exibida. Por exemplo:

```
<img crs="banner.jpg"> 
```

Neste exemplo de código, a imagem não será exibida, pois não existe nenhum atributo da tag `img` chamada `crc` ou `crs`. **O atributo correto que especifica o caminho da imagem** é `src`, que significa *source* do inglês ou **fonte** em português. Sendo assim, fique atento com o nome do atributo.

- Imagem no mesmo nível do arquivo

Neste treinamento, recomendamos que as imagens do projeto estejam no mesmo nível do arquivo `index.html`, ou seja, as imagens do projeto devem estar na **mesma pasta**, como ilustra a imagem abaixo.

![Insira aqui a descrição dessa imagem para ajudar na acessibilidade](https://cdn1.gnarususercontent.com.br/1/58372/043e79d7-f174-4e7f-9ef2-82bd88ff7d4b.png)

# CSS para imagens

[00:00] Na aula passada, adicionamos uma imagem ao conteúdo da nossa página. Nesta aula, vamos aproveitar para mexer no CSS da nossa imagem.

[00:09] Se repararmos, podemos ver um erro. Nossa imagem não ocupa 100% da largura da página.

[00:18] Vamos aproveitar essa aula também para falar de todas as dimensões de um elemento no HTML.

[00:27] Se olharmos nosso HTML, vamos reparar que a imagem está adicionada antes do h1. Para criarmos um CSS que funcione para ela, vamos adicionar um identificador. Ele vai ter o mesmo nome da imagem, “banner”. 

[00:49] Já vimos no nosso CSS que a posição em que ele deve estar é logo acima do h1. Para criarmos um estilo para o identificador, colocamos uma # e no nome dele: #banner.

[01:05] Nele, vamos adicionar todo o estilo que queremos. 

[01:09] Voltando ao navegador, é importante falarmos sobre uma ferramenta que todos os navegadores modernos entregam para os desenvolvedores. É chamada de developer tools, ferramentas para o desenvolvedor. 

[01:25] Se vocês apertarem F12, irão reparar que a ferramenta do desenvolvedor está à direita. Ela tem, entre outras coisas, um layout mobile para sua página, te deixa mexer no console, saber que tipo de arquivos estão sendo transacionados. Mas isso é assunto para o futuro. O que é importante agora é vermos que no developer tools temos uma divisão muito clara entre o que é o HTML, o que é o CSS e o que está sendo exibido no nosso elemento.

[01:57] Como isso funciona? Digamos, por exemplo, que eu quero ver meu h1. Se eu clicar sobre ele, vou ver todo o estilo dele, todo o estilo que já foi criado, e esse estilo vem do nosso arquivo CSS, e verei também a marcação que ele tem na minha página. Ou seja, a largura, altura, qual o espaçamento que ele tem. 

[02:25] Essa ferramenta é fundamental para entendermos e trabalharmos com desenvolvimento. Com certeza você vai usar muito. 

[02:32] O que queremos agora é mudar a largura do nosso elemento. Falando sobre dimensões no CSS, temos quatro parâmetros muito importantes. A largura de um elemento, a altura do elemento, e os espaçamentos. Espaçamento interno e espaçamento externo.

[02:54] Vamos item por item. 

[02:56] Vou usar nosso h1 como exemplo e vou mexer no developer tools. Reparem que se eu clicar logo depois de text align center ele vai criar uma nova linha para eu poder inserir uma modificação. 

[03:10] Só por curiosidade, vamos colocar a cor azul, para vocês verem funcionando. 

[03:17] Imediatamente ele vai alterar a exibição do elemento, deixando o título do h1 em azul. Eu não quero em azul, então vou simplesmente apagar. 

[03:29] Posso também, voltando com o título azul, recarregar a página, e quando recarrego ele some com aquele estilo criado. É só uma ferramenta para o desenvolvedor, na máquina dele, enquanto ele está fazendo aquilo funcionar.

[03:50] No meu h1, vamos falar algumas coisas sobre a dimensão dos elementos. 

[03:55] A dimensão de altura é muito fácil de identificar. Eu insiro com height e coloco em pixels, por exemplo, 100 pixels, ou 100px. Esse elemento passou a ter um espaço muito maior.

[04:17] Colocando o mouse em cima, consigo ver no espaço sombreado de azul a altura do elemento. Vamos alterar para 150px. Vemos que a área aumentou na altura. Só que esse elemento já está ocupando a largura inteira da página. Vamos agora na nossa imagem, onde já temos o identificador do banner, mexer na largura. 

[04:43] A largura de um elemento geralmente é adicionada em pixels, ou podemos também colocar a largura em percentual. Se eu quero que ocupe a página inteira, vou colocar 100%. Imediatamente altero a largura da imagem. Ela passa a ocupar 100% da largura da página. 

[05:06] Vamos ver o que acontece se eu mexer na altura da imagem e colocar um height com 120px. Reparem que ele respeitou a medida de largura, ou seja, 100%, e ajustou a imagem para que ela ficasse apertada com 120px de largura. 

[05:27] A imagem mexe proporcionalmente. Então, se eu aumento a largura, a altura aumenta proporcionalmente. Se eu aumento a largura e a altura, preciso fazer um cálculo muito correto para essa imagem não ficar distorcida. Nós não queremos alterar a altura do elemento.

[05:48] Vamos voltar ao h1. Eu já falei sobre a largura e sobre a altura. Vamos falar sobre o espaçamento. 

[05:55] Para fazer isso, vou criar uma borda no elemento, que tem 10px, com formato sólido e cor preta. Não precisa se preocupar agora com essas configurações. Vamos entender sobre bordas e como elas funcionam no futuro.

[06:22] Mexendo na borda, conseguimos entender a largura e a altura do elemento. 100% de largura e 150px de altura. Vamos alterar a altura em pixels para entendermos o que acontece. 

[06:39] A borda vai se ajeitando. Ela é a finalização do elemento. 

[06:49] O que acontece então se colocamos um espaçamento interno? Ele é chamado de padding, e é configurado de várias formas. Ou ele funciona em todos os lados, ou só para cima, ou só para as laterais, ou só para baixo. 

[07:07] Vamos imaginar um espaçamento interno para todos os lados, para ficar fácil de entender. Se eu colocar um espaçamento de 20px internamente, ele aumenta o meu elemento, criando um respiro entre a borda e o conteúdo. Ou seja, ele criou uma margem interna no elemento.

[07:33] Vou clicar do lado para desmarcar o padding, ou seja, ele vai cancelar essa criação, para ficar clara a diferença. 

[07:42] Se eu colocar um espaçamento interno, ele vai criar um quadro dentro, dando um respiro para todos os lados. Se eu coloco, por exemplo, um espaçamento só para cima de 20px, ele cria esse respiro só na parte de cima. Esse é o espaçamento interno. É para fazer seu elemento se comportar melhor no espaço que ele tem.

[08:10] O espaçamento interno serve, por exemplo, para eu criar um respiro maior da borda para fora. Então, se eu quiser que a borda não esteja colada na lateral, preciso de um espaçamento externo lateral. Para fazer isso, adiciono a margin, que é o espaçamento externo, ou para a direita ou para a esquerda.

[08:35] Vamos fazer só na esquerda uma margem de 40px. Nossa borda descolou da lateral, criamos um espaço para fora do elemento, entre o elemento e a margem do navegador. 

[08:53] Nosso elemento já tem um espaço para cima e para baixo, que foram adicionados pelo navegador inicialmente. Se eu quiser colocar uma margem para todos os lados igual, coloco só o nome dela, só a declaração margin. E na hora que renderizo, ele vai criar uma moldura em volta do meu elemento. 

[09:14] Com isso, conseguimos mexer na configuração e na apresentação de todos os itens. Conseguimos mexer na largura, na altura, na borda, no espaçamento interno e no espaçamento externo. 

[09:28] Vou recarregar a página, voltando para o que já tínhamos. A única coisa que quero fazer é mudar a largura da imagem, então vamos ao nosso CSS. Agora que já aprendemos, vou mudar a largura com a propriedade width e vou colocar o valor 100%. 

[09:46] Salvando e recarregando no navegador temos o site do jeito como queremos.

[09:55] Reparem que quando fechei o developer tools, a imagem se ajustou para sempre o tamanho da página. Isso vai acontecer com qualquer tamanho de tela. Ela vai sempre ocupar 100%. 

[10:09] Nós ainda vamos praticar muito espaçamento, largura e altura dos elementos. Se isso não ficou extremamente claro, não se preocupe. Aos poucos, com a prática, vai ficando natural.

[10:22] Na próxima aula, vamos melhorar ainda mais esse conteúdo. Te vejo lá.

# Extra: Time de Front-End

[00:00] Vamos fazer aqui uma aula bônus com um vídeo rápido, só para falarmos como se comporta um time de front end hoje em dia. 

[00:07] As interfaces do front end estão cada vez com mais responsabilidade, são cada vez mais robustas, tem cada vez mais funções. E por isso o time foi crescendo muito.

[00:19] É importante destacar que um time de front end, ou seja, um time para fazer uma interface não é composto só pelo desenvolvedor front end. Geralmente, temos alguém responsável pela usabilidade do site. 

[00:34] A usabilidade é responsável por responder como vai entregar aquelas informações, a forma. 

[00:42] Temos ainda o time da interface do usuário. O time do design, que vai pegar a forma como aquilo vai ser feito e vai dar o visual para aquilo.

[00:55] Por último, temos o codificador, aquele desenvolvedor front end que vai pegar o design, a forma como o site foi apresentado com aquele visual e vai transformar em código para web, para um aplicativo ou para algum sistema.

[01:14] Essas responsabilidades muitas vezes estão acumuladas em algumas pessoas, mas é importante pontuar cada uma delas. No nosso site, no nosso projeto, reparem que não paramos para discutir sobre qual cor iríamos escolher, ou qual imagem escolher. No nosso projeto, o designer já fez isso para nós.

[01:36] Geralmente é assim que um desenvolvedor front end vai trabalhar. Ele vai receber os inputs e vai extrair daquilo o melhor código possível. 

[01:47] Espero que vocês consigam trabalhar assim e que consigam entregar o melhor código possível.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Remova todo o CSS *inline* da página **index.html**.

2) Como primeiro item do `body`, adicione a imagem **banner.jpg** (se você ainda não a baixou, faça o seu download [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/04/banner.zip)). Adicione também um identificador para a *tag* `img`:

```
<img id="banner" src="banner.jpg">
```

3) Adicione um identificador para o segundo parágrafo do texto:

```
<p id="missao"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>
```

4) No arquivo **style.css**, adicione o CSS que foi removido da página **index.html**, ou seja, alinhe o `h1` e os parágrafos no centro da página e aumente a fonte do segundo parágrafo (use o seu identificador para referenciá-lo): 

```
h1 {
    text-align: center
}

p {
    text-align: center;
}

#missao {
    font-size: 20px
}
```

5) Ainda no arquivo **style.css**, altere a largura da imagem:

```
#banner {
    width: 100%;
}
```

6) O CSS completo ficará da seguinte forma:

```
body {
    background: #CCCCCC
}

#banner {
    width: 100%;
}

h1 {
    text-align: center
}

p {
    text-align: center;
}

#missao {
    font-size: 20px
}

em strong {
    color: #FF0000;
}
```

# O que aprendemos?

Nesta aula, aprendemos:

- Como reestruturar o nosso código, removendo os CSS *inline* e colocando-os no arquivo CSS externo
- Como criar um identificador para marcar especificamente um elemento
  - Como fazer referência a esse identificador no CSS
- Como adicionar uma imagem à nossa página
- Como ajustar a altura do elemento, através da propriedade `height`
- Como ajustar a largura do elemento, através da propriedade `width`
- Como ajustar o espaçamento interno do elemento, através da propriedade `padding`
- Como ajustar o espaçamento externo do elemento, através da propriedade `margin`
- Como se comporta um time de front-end hoje em dia

