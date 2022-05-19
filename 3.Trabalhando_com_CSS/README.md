# Projeto da aula anterior

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/02/aula-2-completa.zip) o projeto do curso no ponto em que paramos na aula anterior.

# Começando com CSS

[00:00] Na aula passada nós mexemos na estrutura da página. Nesta, o objetivo é mudar a apresentação visual dos textos que temos. Até agora, só vimos uma forma de fazer isso, que é mudar a tag. 

[00:13] A tag do parágrafo tem essa apresentação simples, com esse tamanho de fonte, essa configuração, e vimos que se usarmos uma tag de título, por exemplo, do h1, o tamanho da fonte fica maior. Mas as tags têm um valor, um propósito, um significado, e para mexer na apresentação visual dos elementos, não usamos elas. Usamos o CSS.

[00:39] O CSS, que em uma tradução seria folha de estilo em cascata, é a forma como mexemos em cada um dos elementos granularmente, em cada um dos pontos desses elementos para podermos apresentar o nosso site do modo como quisermos.

[00:55] Vamos passo a passo mexer nessas fontes para começar a entender o CSS. 

[01:03] A primeira coisa que quero fazer é: na linha onde temos a missão, quero aumentar o tamanho da fonte. Vamos lá. 

[01:16] No nosso Sublime Text vamos encontrar o parágrafo desejado, onde ainda temos uma tag do strong e uma tag do em, onde fazemos o negrito e a ênfase, e na tag do parágrafo quero aumentar o tamanho da fonte. Por que na tag do parágrafo? Porque quero que seja aplicado em todo o conteúdo que está ali dentro. Por isso que quando falei “folha de estilo em cascata”, é isso. Quando vamos em um elemento anterior, ele reflete para todos os elementos que estão abaixo.

[01:47] Nesse parágrafo vou adicionar a propriedade style, que é o estilo do nosso elemento. Dentro do style e entre aspas vou inserir o que quero alterar. Nesse caso, quero alterar o tamanho da fonte. Para fazer isso, sempre em inglês, tamanho da fonte, font size. 

[02:09] Como escrevemos isso?

[02:22] O tamanho da fonte padrão no navegador é medido em pixels. Ocasionalmente o navegador adiciona o tamanho da fonte inicial como 16 pixels. O que estamos vendo neste momento no navegador é que essas fontes têm 16 pixels. Eu quero mudar a fonte da nossa missão para 20 pixels, por isso 20px ali em cima.

[02:48] Se eu salvar isso e voltar no navegador, a minha fonte já está com outro tamanho na hora da apresentação. 

[03:04] Vamos recapitular. Eu adicionei uma propriedade chamada style, coloquei um =, que é uma atribuição para esse conteúdo. Font size, tamanho da fonte, 20 pixels. Reparem que o Sublime Text coloriu de forma completamente diferente. É por isso que é importante, na hora de criarmos algum conteúdo, quando estivermos realmente escrevendo códigos, usarmos um editor de códigos programado para isso. Ele nos ajuda com esses pequenos detalhes, e quando algo está errado ele nos alerta.

[03:44] Por exemplo, se eu der um espaço no font size ele vai perder a marcação visual da apresentação daquela propriedade. Assim sabemos que está errado.

[03:57] Agora que isso está funcionando, quero alinhar todo esse conteúdo ao centro. Só que eu estou fazendo a divisão de quatro tags, tenho a tag do título e tenho três parágrafos. Para alinhar um elemento ao centro, uso uma propriedade chamada text align.

[04:24] Vou começar fazendo isso com o título. Nele também vou adicionar a propriedade style com o conteúdo text align e o valor center.

[04:37] Ou seja, quero alinhar ao centro, centralizar meu conteúdo. Se recarregarmos, meu título está alinhado ao centro. 

[04:46] Quero fazer isso agora em todos os meus elementos. Vou somente copiar aquilo, colar na linha do parágrafo, colar na linha do último parágrafo, e agora tenho um conflito, porque preciso adicionar duas informações no meu CSS. A primeira é o tamanho da fonte e a segunda é o alinhamento do texto. 

[05:19] Para fazer essa divisão entre duas apresentações, dois itens que estamos apresentando, colocamos um ; e assim conseguimos fazer a separação. 

[05:37] Reparem que todos os meus elementos têm a propriedade style, o valor text align center, e o meu elemento da missão tem o font size 20 pixels. Vamos salvar e ver como isso ficou no navegador.

[05:57] Esse é o primeiro passo para começarmos a alterar o CSS, a mexer em cada um dos pequenos pontos e das possibilidades que temos. 

[06:13] Nesta aula, começamos a mexer na apresentação dos textos, no alinhamento deles e no tamanho da fonte. Na próxima, vamos ver como fazer isso em grandes quantidades de texto e de forma muito mais organizada. Te espero lá.

# Para saber mais: CSS externo

No **vídeo a seguir**, vamos descobrir que existem três formas de configurarmos o CSS. A que fizemos até agora foi a primeira delas, a chamada CSS inline. Ou seja, na linha onde temos nossa tag, adicionamos a propriedade do CSS. A segunda é incluindo a estilização em cada tag na propriedade `style`, no mesmo arquivo html. 

A terceira forma é através de um arquivo externo. Para que a estilização seja aplicada de forma correta, **fique atento**:

### Ao nome do arquivo e sua extensão

Geralmente, chamamos o arquivo que contem os estilos de `style.css`. Observe que este arquivo possui a extensão `.css`.

### Link do CSS no head

Para utilizar a estilização do arquivo `style.css` no `index.html`, precisamos incluir no `head` o seguinte código: 

```
 <link rel="stylesheet" href="style.css">
```

Veja o código completo do `index.html` com o `style.css`:

```
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Barbearia Alura</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

</body>
</html>
```

> Observação: É necessário referenciar o arquivo `style.css` no `head` do `index.html`, como mostra o código acima.

Sabendo dessas recomendações, vamos realizar essa etapa passo a passo, junto com o instrutor?

# Organizando o estilo

[00:00] Existem três formas de configurarmos o CSS. A que fizemos até agora foi a primeira delas, a chamada CSS inline. Ou seja, na linha onde temos nossa tag, adicionamos a propriedade do CSS. 

[00:17] Quais são as características dessa forma de criar o CSS? A primeira delas é que não usamos o nome CSS. Usamos uma propriedade chamada style. A segunda é que como este elemento é único e está marcando somente um conteúdo, toda vez que quisermos colocar a mesma configuração em elementos parecidos, vamos precisar repetir esse código. Por exemplo, todos os nossos parágrafos tem essa representação do alinhamento ao centro do texto. 

[01:01] Isso não é muito legal. Precisamos toda hora repetir o mesmo código. Aqui temos só três parágrafos. Imagine se tivéssemos vinte, cinquenta, se fosse a descrição de uma receita ou a descrição de como se constrói um prédio, se fosse a descrição de um artigo científico. Teríamos muitos parágrafos de texto, e é desumano e inviável ficar adicionando informações pontualmente a cada parágrafo. Pior ainda seria se a partir de agora quiséssemos mudar qualquer uma dessas informações e alinhar esse texto à esquerda, ao invés de ao centro.

[01:45] Para isso, temos uma forma de fazer esse conteúdo ser repetível nesta página. É a segunda forma de apresentarmos o CSS.

[01:55] Para fazermos isso, temos a opção de dentro do head (recordando: o head é o lugar onde passamos as informações para o navegador, e não onde colocamos as informações que queremos exibir). Dentro do head, adicionamos a tag style. Ela é uma tag que abre e fecha. Dentro da tag, podemos colocar marcações de CSS referentes aos elementos que temos no nosso HTML.

[02:30] O que eu quero fazer agora é que todos os parágrafos sejam alinhados ao centro. Da mesma forma como colocamos no inline, só que agora quero escrever uma vez só.

[02:41] Para fazer isso coloco a tag que quero usar, que é a tag do parágrafo, abro e fecho chaves, e dentro coloco a propriedade do CSS que eu quero, que é o text align. 

[02:56] Vou recortar daqui, para sermos obrigados a mexer nesse conteúdo, e agora o meu parágrafo recebe a propriedade text align center. 

[03:08] “Mas Pedro, só um dos parágrafos?”. Não, todos os parágrafos desta página.

[03:15] Se salvarmos isso e repararmos no primeiro parágrafo, ele não tem mais essa descrição do text align center. Vamos voltar no navegador e recarregar a página.

[03:30] Reparem que a apresentação não foi alterada. Ou seja, essa propriedade do text align está sendo aplicada a todos os parágrafos. E como temos no primeiro parágrafo esse elemento removido, ela está sendo aplicada uma vez, mas nos parágrafos seguintes estamos aplicando duas vezes, tanto no inline quanto na tag style. 

[03:56] Vamos remover essa descrição dos parágrafos.

[04:04] O que esperamos agora é que esse conteúdo não seja alterado. Ou seja, que a apresentação seja a mesma com tudo centralizado.

[04:14] Vamos salvar o arquivo, voltar ao navegador e recarregar a página. 

[04:22] A primeira forma é única e exclusivamente para esta tag, tanto que o tamanho da fonte só está alterado na linha do meio, no parágrafo da nossa missão. E o parágrafo geral, onde temos o estilo de todos os elementos, está sendo aplicado nos três parágrafos. 

[04:53] Já falamos do inline e já falamos da tag style. A terceira forma, que é a mais comum de encontrarmos a criação e apresentação do CSS é com um arquivo externo. Para isso, vamos criar um novo arquivo. Se quiserem um atalho, é ctrl+n.

[05:17] Vamos salvar esse arquivo na mesma pasta com o nome style.css. O nome do arquivo vai ser style, onde vamos guardar todo o nosso estilo, e a extensão  do arquivo é CSS. 

[05:34] Agora que temos o arquivo criado na mesma pasta, no nosso HTML vamos fazer uma referência para ele. Vamos fazer com que o HTML busque o arquivo externo e passe a ler e aplicá-lo na nossa página.

[05:52] Para fazer isso, vamos usar a tag link, que é justamente a ligação de um arquivo para o outro. Vamos dizer o relacionamento desse link com a propriedade rel e o valor stylesheet, ou seja, folha de estilo, e vamos dizer onde o arquivo está, href, que é o endereço de referência: 

[06:28] Agora que temos essa ligação, podemos simplesmente recortar o conteúdo da tag style e jogar no nosso arquivo .css. 

[06:43] Na hora de copiar e colar, ele muda um pouco a endentação. Eu vou corrigir, salvar o arquivo CSS, o arquivo HTML e voltar para o meu navegador. O esperado é que quando eu recarregue a página tudo esteja centralizado e o valor da fonte não esteja alterado. 

[07:05] Agora que alteramos a posição do nosso código, a visualização não foi modificada.

[07:17] Vamos recapitular rapidamente. Temos a possibilidade de colocar um elemento com uma micro alteração, com a possibilidade de colocar um CSS inline, ou seja, na mesma linha, e o mais importante do inline é destacar que ele só vai ser aplicado no elemento onde foi criado. 

[07:43] Temos a possibilidade de colocar a tag style, onde tudo que fizermos vai ser aplicado na página inteira, economizando muita escrita de código; e temos a possibilidade de adicionar um arquivo externo ao HTML, em que teremos todo o CSS.

[08:05] Essa é a forma mais comum de ser feita, criar um arquivo externo, porque não só o código pode ser aplicado nesta página, como em qualquer outra página em que criarmos um link para esse CSS. Se imaginarmos um site em que temos vinte páginas diferentes, todas elas terão o mesmo estilo. É isso que buscamos quando estamos criando um bom código.

[08:34] Nesta aula, vimos como aplicar o CSS das três formas diferentes. Na próxima aula, vamos evoluir ainda mais essa apresentação, entendendo ainda mais como funciona o CSS e aplicando detalhes diferentes. Te espero lá.

# Mudando a cor

[00:00] Na aula passada, vimos como dividir o CSS e como temos vários níveis para implementar o CSS no nosso HTML. Nessa aula, vamos avançar no CSS, entendendo como podemos colorir nossos elementos no nosso site.

[00:17] A primeira coisa é entender o que queremos mudar. Quero que toda a área ao fundo do texto seja uma área cinza. Quero ter um fundo cinza. E que a cor do texto seja um pouco diferente.

[00:36] A primeira coisa que vamos fazer é mexer em um dos elementos. Eu quero começar mexendo no h1. Para mexer nele, tenho a propriedade style. Quero mexer também na cor de fundo deste elemento. Para mexer na cor de fundo, vou adicionar um ; e vou adicionar a propriedade background. Background é o que define tudo que será o fundo do elemento. Podemos colocar cor, imagem, várias propriedades. Depois vamos falar mais sobre isso. Por enquanto quero mudar só a cor.

[01:16] Para isso, vamos usar a linguagem hexadecimal. Vou fazer um vídeo extra sobre como a cor se comporta no CSS, que tipos de linguagens podemos usar para marcar uma cor. Mas isso fica para depois. Por enquanto, vamos usar a definição da cor cinza, que vai ser “cccccc”. 6 letras c’s.

[01:47] Se salvarmos isso e voltarmos à nossa página, nosso background do título já está cinza. Já atingimos o primeiro objetivo.

[02:00] Mas eu não disse que quero tudo tendo um fundo cinza? Vamos voltar então ao nosso HTML, copiar esse background cccccc e adicionar em todos os parágrafos. Para adicionar esse background em todos os parágrafos, eu poderia colocar linha a linha ou no nosso CSS, onde já temos a descrição do parágrafo. Vou adicionar um ; vou quebrar a linha para ficar mais organizado e vou colocar a mesma definição de background.

[02:34] Quando salvarmos esse arquivo e voltarmos ao navegador, veremos as alterações.

[02:40] Reparem que nesse momento as alterações são só de cor de fundo do elemento. Mas não quero que fique quebrado.

[02:51] Como funciona a visualização nesse momento? Temos a divisão entre os elementos, e essa divisão, esse espaço entre um item e outro, no momento não queremos mexer. Queremos só que o fundo seja cinza. 

[03:11] Vamos voltar ao HTML para entender um pouco mais a estrutura. Nela, temos a tag h1 e as tags de parágrafo. São as tags que alterei até agora. Se pensarmos em níveis hierárquicos, todas elas estão dentro da tag body. Ou seja, a tag body é pai de todas essas tags. É quem envolve todas elas. 

[03:42] Se eu quero que um fundo seja extra essas tags, ou seja, que ele envolva todas as tags, preciso mudar essa descrição da tag h1 e parágrafo para a tag do body. Podemos fazer isso.

[04:00] A primeira coisa que vou fazer é retirar a descrição. Também vou retirar a descrição do background no parágrafo. E no meu arquivo de CSS vou adicionar a tag body, que é a nova tag em que estou colocando o estilo. E aí vamos colar de volta aquela definição de background e a cor de fundo.

[04:31] Quando salvamos isso e voltamos ao navegador, temos uma alteração. Todo o nosso body passou a ter a cor de fundo. Ou seja, o elemento superior, que envolvia todos, agora tem essa propriedade.

[04:51] Uma coisa importante a se falar sobre o CSS é que idealmente, em um bom padrão de projeto, nosso CSS corresponde à mesma estrutura do HTML. Como o body vem antes do parágrafo, vamos também aqui adicionar antes do parágrafo. Assim nosso código fica mais organizado.

[05:20] Vamos então também, ainda falando sobre cores, mudar a cor de um dos textos.

[05:30] Digamos que eu queira colocar a nossa missão, que hoje é preta, na cor vermelha. Onde está a marcação específica dessa frase? Qual tag está marcando isso? A tag do parágrafo marca tudo, a tag da ênfase marca toda a linha, e a tag strong marca especificamente só aquele conteúdo. 

[06:00] Para a tag strong, vamos dar uma definição de cor. Dentro do nosso arquivo de CSS, vamos abrir uma nova definição para a tag strong e vamos colocar a definição de cor.

[06:15] Até agora, só falamos sobre a cor de fundo, que é o background. Para a cor do elemento vamos a propriedade color. Vou usar o nome vermelho, red.

[06:28] Reparem que usei aqui um nome, lá em cima usei um hexadecimal. Não se preocupem, isso tudo funciona, o CSS nos dá essa liberdade para fazer essas modificações. Aos poucos vamos entendendo mais sobre isso.

[06:43] Salvando esse arquivo e voltando para o navegador, a nossa tag está em vermelho.

[06:52] Reparem no que aconteceu. Como estou usando a tag strong para marcar nossa missão, mas também estou usando a tag strong para marcar Barbearia Alura, as duas palavras ficaram em vermelho.

[07:07] Se voltarmos ao nosso HTML, conseguimos ver muito claramente essa similaridade. Ou seja, temos a tag strong usada em dois momentos diferentes. 

[07:23] Como faço então para deixar um CSS específico para somente um elemento? Precisamos que: ou o CSS seja aplicado in line ou que mudemos o CSS para atender a uma estrutura. 

[07:45] Como assim? Temos um strong dentro de um parágrafo. Na linha de baixo, temos um strong dentro de em, que está dentro de um parágrafo. No nosso CSS, temos como fazer isso. Temos como selecionar especificamente o strong que está dentro do em.

[08:07] Fazemos isso colocando a seguinte estrutura: em strong.

[08:16] Lendo isso como o navegador vai ler, ele vai procurar todos os strongs que estão dentro de todos os ems. No nosso caso, no nosso site, só temos uma possibilidade para essa marcação. 

[08:34] Se salvarmos e voltarmos à página, vamos ter marcado especificamente somente este elemento.

[08:42] Aos poucos vamos entender como marcar mais especificamente os elementos e como fazer o código ficar menos complexo. Mas o importante aqui é entendermos como funciona o CSS e essa propriedade do estilo em cascata. Ou seja, marcamos o body e isso refletiu para todos os filhos dele. Marcamos o parágrafo e ele replicou para todos os parágrafos. E na última linha, marcamos o strong, que está dentro do em, ou seja, fazendo essa cascata. Conseguimos procurar este elemento usando a estrutura do HTML.

# Extra: Cores hexadecimais

[00:00] Neste bônus, vamos falar sobre cores e como elas funcionam no CSS, no navegador.

[00:06] A primeira coisa sobre a qual precisamos falar são alfabetos. Temos o nosso alfabeto padrão, abcde e por aí vai. Esse é o alfabeto que usamos no português. 

[00:26] Os alfabetos para computação são um pouco diferentes. Por exemplo, temos o binário. É o 0 e o 1. Temos o numérico, que vai do 0 ao 9. E aí conseguimos representar todos os números com isso. Ainda temos o dicionário hexadecimal, que é a mesma coisa que o dicionário numérico adicionando as letras abcdef. 

[01:03] Com esse dicionário conseguimos representar muito mais coisas do que só com o dicionário numérico. É ele que usamos para marcar cores.

[01:14] Vamos voltar e entender como funcionam as cores para nós.

[01:20] Nós conseguimos enxergar três espectros de cor, e o HTML monta isso. Nós enxergamos o espectro RGB, que quer dizer Red Green Blue. Ou seja, vermelho, verde e azul.

[01:38] Montamos a cor seguindo essa mesma característica, usando o dicionário hexadecimal. Para fazer isso, colocamos # e marcamos seis elementos. Os dois primeiros para marcar o vermelho, os dois segundos para marcar o verde e os dois últimos para marcar o azul. 

[02:02] Como é a representação numérica, ou em hexadecimal, para esses números? O zero é a ausência de cor, e o F é o máximo de cor. Então, se eu quiser representar, por exemplo, o preto, que é a ausência de todas as cores, coloco #000000. Ou seja, 00 para vermelho, 00 para verde e 00 para o azul. Se eu quiser representar o branco, coloco #FFFFFF. FF para o vermelho, FF para o verde e FF para o azul.

[02:42] Lembrem que no nosso exercício, se voltarmos ao style do CSS, usamos a representação #CCCCCC. Se olharmos no espectro do hexadecimal, o CC é quase o branco. Não é o preto completo e nem o branco completo.

[03:10] Essa é a representação dos elementos. 

[03:16] Como faríamos, por exemplo, para representar a cor vermelha em hexadecimal? Precisamos colocar # e precisamos que o vermelho seja completo, ou seja, no máximo, e que todas as outras cores não existam: #FF0000.

[03:36] Podemos voltar ao nosso CSS e alterar para, ao invés de vermelho, #FF0000. Assim, marcamos o vermelho em hexadecimal, e é assim que vamos usar as cores em hexadecimal no nosso projeto. 

[03:55] É importante saber também que existe outra forma de representar as cores, além das que já vimos. Temos as cores básicas, a linguagem hexadecimal e a RGB. O mesmo padrão RGB que falamos sobre as cores que conseguimos enxergar, temos um dicionário RGB. Um alfabeto. Ele vai do 0 até 255. Ou seja, ele tem 256 níveis de representação de cada cor. 

[04:44] Para isso, o 0 também é a ausência e o 255 é o máximo. A representação no CSS é um pouco diferente. Ao invés de colocar #, eu coloco RGB( , , ), separando as cores por vírgula. Antes da primeira vírgula vem o vermelho. Então, se eu quiser representar o branco, coloco RGB(255, 255, 255). Se eu quiser representar só o azul, RGB(0, 0, 255).

[05:32] Essa é a forma que usamos para representar as cores com esses alfabetos no CSS e isso ser renderizado pelo nosso navegador.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Na mesma pasta da página **index.html**, crie o arquivo CSS **style.css**. Neste arquivo, modifique a cor de fundo do `body`, centralize os parágrafos e altere a cor das *tags* `strong` que estão dentro de *tags* `em`:

```
body {
    background: #CCCCCC
}

p {
    text-align: center;
}

em strong {
    color: #FF0000;
}
```

2) Na página **index.html**, como último elemento do `head`, importe o CSS **style.css**:

```
<link rel="stylesheet" href="style.css">
```

3) Centralize o texto do `h1`:

```
<h1 style="text-align: center">Sobre a Barbearia Alura</h1>
```

4) E altere o tamanho da fonte do segundo parágrafo:

```
<p style="font-size: 20px"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>
```

5) A página completa ficará da seguinte forma:

```
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <title>Barbearia Alura</title>
        <link rel="stylesheet" href="style.css">
    </head>

    <body>
        <h1 style="text-align: center">Sobre a Barbearia Alura</h1>

        <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
        Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

        <p style="font-size: 20px"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

        <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
        O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
    </body>
</html>
```

# O que aprendemos?

Nesta aula, aprendemos:

- A mexer na apresentação dos textos

  - No alinhamento deles (`text-align`)
  - No tamanho da fonte (`font-size`)
  - Na cor de fundo (`background`)
  - Na cor do texto (`color`)

- CSS 

  inline

  - Na linha onde temos a nossa *tag*, adicionamos a propriedade do CSS

- A tag 

  `<style>`

  - Dentro da *tag*, podemos colocar marcações de CSS referentes aos elementos que temos no nosso HTML

- A apresentação do CSS com um arquivo externo

- Como funciona o estilo em cascata do CSS

- Como importar um arquivo externo de CSS dentro da nossa página HTML

- Como representar cores no CSS

  - Através do nome da cor
  - Através do seu hexadecimal 
  - Através do seu RGB

Nesta aula, começamos a mexer na apresentação dos textos, no alinhamento deles e no tamanho da fonte. Na próxima, vamos ver como fazer isso em grandes quantidades de texto e de forma muito mais organizada. Te espero lá.

