# Projeto da aula anterior

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/04/aula4-completa.zip) o projeto do curso no ponto em que paramos na aula anterior.

# Trabalhando com listas

[00:00] Já evoluímos nosso site até aqui. Agora, vamos adicionar mais conteúdo. Vamos adicionar uma nova seção no site, que serão os benefícios da nossa barbearia.

[00:10] Para isso, vamos voltar ao nosso HTML. Abaixo do último parágrafo, vamos começar uma nova seção, chamada “Benefícios”.

[00:23] Vimos na primeira aula que para criarmos um título com HTML, usamos a tag h. e usamos h1 para ser o título principal da página. Agora que estamos criando uma nova seção, outra parte do nosso site, vamos colocar outro título. Seguindo a sequência, vamos usar h2. 

[00:46] O h2 começa nosso novo conteúdo. Se salvarmos isso e formos no navegador, veremos o “Benefícios” destacado em negrito, seguindo o mesmo padrão que vimos para o título principal da página. 

[01:07] Agora, queremos listar os benefícios da nossa barbearia, que são quatro.

[01:13] Vamos ao HTML. A estrutura que eu desejo é: o primeiro item, atendimento aos clientes é o nosso maior benefício. O segundo item, espaço diferenciado. Terceiro item, localização. Quarto e último item, profissionais qualificados. 

[01:51] Essa é a intenção que eu tenho. Quero que esses itens estejam listados. 

[01:58] Se formos até nossa página e recarregarmos, veremos que estão todos um do lado do outro, sem uma forma. Falta uma tag para marcarmos esses itens. 

[02:10] No nosso HTML, a solução mais fácil dadas as ferramentas que temos seria colocar uma tag de parágrafo, mas ela não é correta para essa demanda. Não é a semântica correta para uma lista. As listas têm uma tag própria.

[02:31] Temos as listas não ordenadas, onde não importa qual item vem primeiro ou depois. E temos as listas ordenadas, como por exemplo uma receita de bolo, onde primeiro tenho que ligar o forno e depois colocar a massa.

[02:49] Aqui queremos uma lista não ordenada. Para isso, usamos a tag ul, de unordered list. Uma lista sem ordem.

[03:01] Se quisermos uma lista ordenada, é só trocar para ol, de ordered list. 

[03:08] A tag ul é uma tag de conteúdo. Ela inicia e fecha. Precisa fechar ao final da lista. Vamos consertar a endentação dos nossos itens para visualmente sabermos tudo que está acontecendo. Todos os itens da nossa lista vão dentro da ul.

[03:29] Se salvarmos isso e recarregarmos o navegador, veremos que nada aconteceu, só temos agora um pequeno espaço no início da primeira linha. Por quê? A lista, além da tag ul ou ol, no caso usamos ul para lista não ordenada, ainda precisa de marcação para cada item.

[03:50] Para isso, usamos a tag li, de list item. Para cada um dos itens, vou colocar a tag li. Ela inicia em cada uma das linhas e termina ao fim daquele conteúdo, daquele item. 

[04:18] Agora que já temos os itens marcados podemos voltar ao navegador. Temos uma lista com os itens não ordenados. Podemos até remover o *, que serviu só para explicarmos visualmente qual era o objetivo principal.

[04:40] Agora que temos a lista, que temos toda essa estrutura para nosso conteúdo, queremos criar um CSS para ele. Mas até agora só vimos duas formas de marcar o CSS. Primeiro usando as tags e o segundo usando os identificadores. 

[05:02] O problema de usarmos as tags é que todas as listas do nosso site terão o mesmo estilo. E o problema de usar identificadores é que eles são únicos. Ou seja, temos uma lista com quatro itens e para marcar cada um deles, teríamos que criar quatro identificadores. 

[05:19] Existe uma solução para isso. É o conceito das classes no CSS. As classes no CSS servem para marcarmos itens, para posteriormente colocarmos estilo em cada um deles, só que são repetíveis. Ou seja, podemos marcar todos os nossos itens com a mesma classe. 

[05:38] Vamos fazer isso. 

[05:40] Assim como no identificador, em que adiciono a propriedade id e dou um nome para ela, nas classes faço a mesma coisa. Adiciono a propriedade “class” e entre aspas o nome dela.

[06:14] Podemos colocar o mesmo nome em todos os itens. Essa vai ser a classe que usaremos para marcar todos esses nossos itens.

[06:20] Agora que temos os itens marcados, queremos criar um tamanho de fonte específico para eles e colocar todos em itálico. 

[06:30] Vimos nas primeiras aulas como colocar um elemento em itálico visualmente simplesmente usando uma tag, que é ênfase, a tag em. 

[06:43] Como fazemos para colocar vários elementos em itálico sem ser uma ênfase, sendo só um detalhe visual? No nosso CSS, vamos criar a referência para classe. Para fazer isso, quando usamos o identificador, usamos a #. Quando usamos uma classe, colocamos um “.”.

[07:02] Então .itens, e aí podemos criar todo o CSS para aqueles quatro itens da nossa lista. Quero dizer que o texto está em itálico, e para isso vamos colocar a propriedade font style, com a variável itálico: font-style: italic.

[07:22] Ou seja, estamos transformando todos aqueles itens em itálico. 

[07:28] Se recarregarmos nossa página, veremos todos os itens marcados com itálico. 

[07:35] Só que no nosso layout visual quero separar esse conteúdo. Quero que comecemos a ter um fundo branco nos itens, ao invés do fundo cinza, justamente para gerar esse destaque.

[07:48] Por isso, na próxima aula nós vamos falar em como criar divisões no nosso conteúdo.

# Divisões de conteúdo

> *Você pode baixar um ZIP com a imagem \**beneficios.jpg** aqui.*

https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/05/beneficios.zip

[00:00] Agora, queremos criar mais uma divisão no nosso site, uma separação entre as duas seções.

[00:06] A primeira, onde teremos todo o texto de apresentação do nosso site, e a segunda, onde teremos os benefícios apresentados ao nosso cliente.

[00:14] Para isso, realmente precisamos ter o conceito de uma divisão. Criar dois blocos de conteúdo e separá-los com tags de HTML. 

[00:25] Se formos ao nosso HTML, veremos que toda essa primeira parte, a partir do h1, e os quatro parágrafos, respondem a uma primeira seção, que poderíamos chamar de principal; e o h2 e nossa lista pertencem a uma segunda seção, que poderíamos chamar de Benefícios.

[00:52] Para fazer isso, criamos a tag de divisão, a tag div. A primeira vai englobar o h1 e os três parágrafos, e aí vamos indentar isso para ficar correto. Uma dica: se você selecionar tudo com o mouse ou com o teclado e apertar tab uma vez, ele vai indentar tudo como um bloco para você. 

[01:25] Vamos fazer a mesma coisa nos benefícios. Criar outra divisão que fecha depois da nossa lista e indentar isso para ficar correto.

[01:42] Temos então no nosso HTML duas divisões. Vamos entender como isso ficou visualmente no nosso navegador. Observando, não notamos diferença alguma.

[01:52] As divisões têm por padrão não interferir na apresentação visual do nosso conteúdo. Elas servem para marcarmos nosso conteúdo, e, a partir do CSS fazermos os efeitos que quisermos. Mas como vamos marcar o conteúdo?

[02:12] Temos duas tags com o mesmo nome. Para isso, precisamos de especificidade, precisamos ou criar um identificador, ou criar uma classe. 

[02:25] Já falamos a diferença dos dois. O identificador serve para itens únicos e a classe serve para itens que serão repetidos.

[02:33] Como só temos esse conteúdo, sabemos que eles são únicos, mas se quisermos criar um layout robusto, com todas as técnicas, e quisermos replicar esse conteúdo no futuro, o ideal é criarmos classes. Vamos seguir esse padrão a partir de agora. Sempre que quisermos marcar um conteúdo visualmente, vamos criar uma classe para ele. 

[02:54] A classe que queremos criar é a dos benefícios, então vamos criar uma classe com o nome “benefícios”.

[03:02] Se formos no CSS, a marcação de uma classe é um ponto e o nome dela. O que queremos aqui é que ele tenha um fundo branco, e um fundo branco, como vimos, é com a propriedade background. 

[03:27] Para fazer a cor branca, precisamos que todos os itens da nossa cor estejam no máximo, ou seja, todas as cores. Então, #FFFFFF. 

[03:41] Se recarregarmos, veremos que essa nossa divisão está perfeita no nosso conteúdo. Mas temos um problema. Ela está com fundo branco, mas o fundo da minha página inteira está cinza. Por que isso aconteceu?

[04:00] Quando colocamos o fundo cinza, colocamos na tag do background, e não no nosso conteúdo de texto de apresentação. Portanto, vamos mudar isso a partir de agora.

[04:13] Na nossa tag do conteúdo principal, vamos criar uma classe com o nome “principal”. Para esta tag, quando voltarmos no nosso HTML, lembrando que a estrutura do CSS deve ser correspondente à estrutura do HTML, logo abaixo do banner vamos criar a classe principal. E nela vamos recortar o fundo cinza do background e vamos colar no principal. 

[04:54] Agora, temos o site inteiro com o fundo branco e nosso espaço também com fundo branco.

[05:05] Um problema que temos que resolver no nosso site é que temos um espaço branco indesejado entre a imagem e o nosso conteúdo principal, e um espaço branco indesejado na lateral do nosso site.

[05:23] Isso foi o navegador que adicionou. Já vamos aprender a resolver.

[05:29] No momento, temos nosso título de benefícios e nossa lista de itens. Vamos continuar estilizando-os.

[05:38] Seguindo o padrão do bloco de cima, quero que o Benefícios seja centralizado. Para fazer isso, lembrando que no nosso HTML ele está com a tag h2, voltando no nosso CSS, vou criar um marcador para ele a partir da tag h2: text-align: center

[06:06] Voltando na nossa página, já temos um título centralizado. 

[06:12] Por último, para completar esse bloco de conteúdo, precisamos adicionar mais uma imagem. Também já sabemos como fazer isso. Através da tag img.

[06:25] Vamos criar a img e vamos colocar o source dela, a fonte, onde essa imagem está. Ela é nossa imagem beneficios.jpg, que está na pasta do projeto. 

[06:42] Quando voltarmos ao nosso navegador, a imagem está lá.

[06:48] Reparem que ela está muito grande, ocupando a largura inteira da página. O ideal é que ela fique ocupando 50% da página do lado direito, ao lado dos itens da lista. 

[07:06] Na próxima aula, vamos entender como criar essa divisão e posicionar esses elementos do jeito que queremos.

# Inline e Block

[00:00] Vamos criar o estilo necessário para fazer este bloco de conteúdo ficar perfeito.

[00:06] A primeira coisa que temos que fazer é ajustar a imagem. Ela está muito grande, ocupando 100% da largura do elemento, e não é isso que queremos. Queremos que ela fique posicionada ao lado da lista de benefícios. 

[00:21] Para fazer isso, vamos mexer na nossa imagem, e já sabemos como. Precisamos criar uma classe para esse elemento. 

[00:31] Eu vou criar a classe e chamá-la de “imagembeneficios”. 

[00:45] No meu CSS, vou criar uma marcação para essa classe: .imagembeneficios

[00:56] E vou dizer que ela vai ter, a partir de agora, 50% da largura: width: 50%

[01:05] Quando voltamos ao navegador, essa imagem já passou a ocupar 50% da largura da página. Só que o que aconteceu para ela não estar ao lado dos itens?

[01:16] Se lembrarmos quando fizemos nossa lista sem a marcação dos itens, da tag li, estavam todos em uma linha. A mesma coisa aconteceu quando fizemos os parágrafos iniciais. Quando colocamos a tag li, ela passou a ocupar 100% da largura da página e quebrar a linha depois dela. Ou seja, o próximo item começava na linha de baixo.

[01:41] Esse comportamento de uma tag ocupar a largura inteira da página é chamado “block”. Ele bloqueia o conteúdo daquela linha. Todos os itens da nossa linha têm o comportamento block. Uma imagem não bloqueia o conteúdo, ela deixa que existam outros na lateral, e esse tipo de conteúdo é considerado inline. 

[02:10] A diferença entre eles é que mesmo que eu diminua o tamanho, diminua a largura de um elemento block, ele vai sempre ocupar aquela linha, mesmo preenchendo só metade.

[02:25] Um elemento inline não me deixa alterar, por exemplo, o espaçamento externo e interno dele.

[02:34] Para isso, existe uma terceira característica, quando o elemento possui as duas condições. Ele é inline e block ao mesmo tempo. Ou seja, ele bloqueia uma largura, mas essa largura é fixa. Sou eu que dou o tamanho. E ele me deixa também mexer na largura e nos espaçamentos interno e externo.

[02:58] Vamos aplicar isso para ficar mais claro.

[03:01] A primeira coisa que temos que fazer é que a nossa lista precisa de uma marcação. Ou seja, nosso ul precisa de uma marcação. Eu falei do inline e do block. Isso são características do display. Ele pode ser block, inline ou juntar as duas coisas e ser do tipo inline block. 

[03:33] O display inline block ocupa só o tamanho do conteúdo, mas me deixa mexer na largura e espaçamentos. Vamos ver na prática.

[03:43] No nosso navegador, quando recarregamos, vemos que o elemento está ocupando só o tamanho do seu conteúdo, e do lado dele já entrou nossa imagem. Mas aconteceu um erro. Na verdade, é uma características do CSS. 

[04:01] Todos os elementos são alinhados pela linha de baixo e queremos que sejam alinhados pela linha de cima. Para isso, no nosso CSS, adicionaremos a propriedade “vertical-align: top”.

[04:18] Quando recarregamos a página, nosso título está centralizado, nossa lista de itens está ocupando só o tamanho dela e nossa imagem está ocupando 50% da página. 

[04:33] Vamos agora mexer um pouco na nossa lista de itens. Dar um espaço e aumentar a largura. Como ele é um elemento do tipo inline block, eu posso dizer que ela tem de largura 20% da página e que ela ainda tem um espaçamento externo para a direita de mais 15%.

[05:00] Se recarregarmos a página, veremos os itens se dividirem melhor. Veremos a imagem ocupando metade do conteúdo, alinhada à nossa lista de itens e alinhada também a esse espaçamento que desejamos no meio. 

[05:22] Para finalizar esse layout desses dois blocos, agora que estamos revisando largura e espaçamento, vamos mexer também no espaçamento inteiro dos dois blocos. 

[05:35] No primeiro, no Benefícios, vamos adicionar um espaçamento interno para todos os lados de 20px, ou seja, padding: 20px

[05:48] Quando voltarmos ao navegador, veremos as coisas se organizando um pouco melhor. Temos uma margem de respiro em baixo e na lateral.

[05:59] No nosso bloco principal, quero adicionar um espaçamento interno de 30px, padding: 30px

[06:13] Agora nosso conteúdo está melhor distribuído e nosso site começando a ter uma cara mais definitiva. 

[06:23] Para finalizar todo o nosso visual, precisamos apenas adicionar um cabeçalho à nossa página. Mas isso é matéria da próxima aula.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Na página **index.html**, envolva o texto em uma `div`:

```
<div class="principal">
    <h1>Sobre a Barbearia Alura</h1>

    <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
    Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

    <p id="missao"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

    <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
    O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
</div>
```

2) E abaixo da `div` `principal`, crie a `div` `beneficios`, com a lista de benefícios e a sua imagem:

```
<div class="beneficios">
    <h2>Benefícios</h2>

    <ul>
        <li class="itens">Atendimento aos Clientes</li>
        <li class="itens">Espaço diferenciado</li>
        <li class="itens">Localização</li>
        <li class="itens">Profissionais Qualificados</li>
    </ul>

    <img src="beneficios.jpg" class="imagembeneficios">
</div>
```

3) No CSS **style.css**, remova a estilização da cor de fundo do `body` e passe-a para a `div` `principal`. Além disso, dê um espaçamento interno para ela: 

```
body {

}

.principal{
    background: #CCCCCC;
    padding: 30px;
}
```

4) Mude a fonte dos itens da lista para *itálico*, estilize a cor de fundo da `div` `beneficios` e alinhe o texto do `h2` ao centro:

```
.itens {
    font-style: italic;
}

.beneficios {
    background: #FFFFFF;
    padding: 20px;
}

h2 {
    text-align: center;
}
```

5) Na lista, modifique o seu `display` para `inline-block` e faça ela ser alinhada pela linha de cima. Além disso, altere a sua largura para ser 20% da página e sua margem externa à direita para ser de 15%:

```
ul {
    display: inline-block;
    vertical-align: top;
    width: 20%;
    margin-right: 15%;
}
```

6) Por fim, altere a largura da imagem dos benefícios:

```
.imagembeneficios {
    width: 50%;
}
```

# O que aprendemos?

Nesta aula, aprendemos:

- A trabalhar com listas não-ordenadas e listas ordenadas

  - Para cada um dos itens da lista, utilizamos a *tag* **<li>**

- O conceito das 

  classes

   no CSS

  - Elas servem para marcar itens, que são repetíveis

- Como referenciar uma classe no CSS

- Divisões de conteúdo, utilizando a *tag* **<div>**

- Os comportamentos **inline** e **block**

