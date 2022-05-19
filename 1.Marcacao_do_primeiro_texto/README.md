# Introdução

[00:00] Bem-vindo ao curso de HTML e CSS.

[00:02] Meu nome é Pedro Marins e eu vou te guiar nessa jornada de aprendizado.

[00:06] Neste curso, nós separamos a página da Barbearia Alura. 

[00:11] Nós vamos criar texto, imagem, blocos de conteúdo, listas de informações. Vamos aprender a mudar cor, posicionar elementos, mudar espaçamento. Enfim. Vamos mexer em tudo do HTML e CSS. 

[00:28] O curso foi separado em blocos incrementais, para que você possa fazer detalhe por detalhe, melhorando sua página.

[00:35] No curso, vamos falar sobre HTML, CSS, tags, sobre cada uma das propriedades. Como usar cada uma dessas coisas.

[00:44] Depois desse curso, você vai poder criar uma página igualzinha a essa ou qualquer outra página web.

[00:51] Vem comigo que tenho certeza que você vai gostar.

# Download do texto base

No próximo vídeo, o instrutor irá utilizar um **texto base** para o início do treinamento. Você pode baixar um ZIP com esse texto [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/01/texto-base.zip).

# O primeiro desafio do curso

## Seu primeiro desafio

Seu primeiro desafio no curso é se apresentar na **comunidade da Alura no Discord** no canal "apresente-se":

![print do discord da alura mostrando os canais geral, apresente-se, off-topic, filmes, jogos e cafezinho, uma seta vermelha aponta para o canal apresente-se](https://cdn1.gnarususercontent.com.br/1/20140/3537c6b8-945b-499c-9d08-9249b3524454.png)  

Uma vez [na dashboard da Alura,](https://cursos.alura.com.br/dashboard) no menu vá em `Comunidade` e depois em `Discord da Alura`. 

## Como funciona o Discord?

Confira este Alura+ e aprenda como é e como funciona a **Comunidade da Alura no Discord:**

[Alura+ sobre o Discord da Alura](https://cursos.alura.com.br/extra/alura-mais/comunidade-no-discord-c1400)

------

Lembrando que utilizar o Discord é opcional, mas pode te ajudar a se conectar com mais pessoas da área

O Discord é da Alura inteira mas na lateral esquerda você pode encontrar as categorias de cada Escola da Alura.

(Programação, Front-end, Data Science, Devops, UX & Design, Inovação & Gestão)

# Definindo texto

[00:00] Vamos começar os nossos desafios, então.

[00:03] Na aula anterior, apresentamos como seria a página desejada, o que vamos construir ao longo deste curso.

[00:11] Nesta primeira aula, nós vamos trabalhar o texto, que é o miolo dessa página.

[00:15] Vamos construir passo a passo esse conteúdo para que você consiga chegar na página desejada.

[00:22] O primeiro passo vai ser trabalhar o parágrafo de texto e os títulos que existem na página. 

[00:28] Para isso, existe disponível um arquivo. Tem um [link](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/01/texto-base.zip) aí para você. É o arquivo “texto base”. 

[00:37] Se você abrir esse arquivo, temos o que seria um título e três parágrafos de texto. Usando o próprio Word, nós poderíamos aumentar o tamanho da fonte, deixar o texto em negrito, selecionar alguma coisa de destaque no nosso primeiro parágrafo, como por exemplo o nome “Barbearia Alura” e colocar em negrito. Poderíamos selecionar a missão da barbearia e deixar em itálico. Formatar esse texto de forma a dar destaque para algumas informações específicas. 

[01:17] Isso é a forma como trabalhamos essa apresentação do texto no Word. 

[01:23] Vamos pensar nisso agora para nossa página, no HTML. 

[01:30] A primeira coisa que precisamos fazer usando HTML é que não vamos usar o editor de texto do Word. Vamos usar um editor de código. Eu vou usar o Sublime Text 3. Vocês podem baixar ele na internet. É gratuito, disponível para todos os sistemas operacionais. Podem inclusive usar o Atom, que é outro editor de código, também gratuito e disponível para ser baixado. Ou o Visual Studio Code. Essas são as três recomendações para você usar durante este curso. 

[02:18] Eu vou usar o Sublime Text 3. Já tenho ele instalado. Assim que eu abrir o programa, ele me dá uma tela preta, onde vamos escrever todo o nosso código. 

[02:31] A primeira coisa que vou fazer é copiar aquele texto do Word e jogar no Sublime Text. Se vocês repararem, toda aquela formatação que nós criamos foi perdida. Este é um editor de código, e o negrito, tamanho de fonte, eles não vêm por padrão. Nós vamos chegar lá. 

[03:02] A primeira coisa que precisamos fazer no Sublime Text é salvar este arquivo, pode salvar em uma pasta sua ou na área de trabalho, com o nome index.html. O nome index é padrão para o arquivo principal da sua página. E como nesta página vamos criar somente um arquivo HTML, esse vai ser o nome do nosso arquivo durante todo o projeto. Vamos mexer nesse mesmo arquivo.

[03:32] O .html, diferente do .doc para o Word, diz que este arquivo é uma página web. Salvando este arquivo index.html, se voltarmos na nossa área de trabalho, minimizar tudo, ele agora está com o ícone do Chrome para ser aberto. E se eu der dois cliques ele vai abrir direto no navegador. [04:00] Reparem o que ele fez com o nosso texto. Ele não botou quebra de linha, negrito, itálico, não aumentou a fonte.

[04:14] Se voltarmos para o editor de código, vamos ver que o texto está simples, e não é isso exatamente o que temos, quando vemos uma página web. Uma página web tem o seu conteúdo com HTML. Nós usamos o HTML para fazer uma marcação desse texto. O HTML quer dizer “hyper text markup language”. Uma linguagem de marcação de texto. 

[04:40] Para marcarmos esse texto, precisamos usar o que são chamadas de “tags”. O formato de uma tag é um sinal de < um nome qualquer e um sinal de >. Isso é o que fecha uma tag. É o conteúdo que vamos ter para uma tag.

[05:01] E que tags vamos usar neste texto? Por exemplo, na primeira linha temos um título. Vamos usar uma tag chamada “h”, de heading, que é o título do conteúdo. 

[05:18] Existem seis níveis de título. Para o primeiro título da página, vamos usar h1. Já na sequência, vamos ter o primeiro parágrafo de texto. O parágrafo de texto é marcado com a tag “p", de paragraph. Vamos fazer isso para o segundo e terceiro parágrafo também.

[05:49] Mas... quando o HTML vai saber onde termina um h1 e começa um parágrafo? Por padrão, ele não vai saber. Nós precisamos informar isso para o nosso navegador. Como precisamos marcar o conteúdo, eu marco o início e o final. Marquei o início do título com h1 e para marcar o final, além do sinal de <, preciso colocar uma barra. Assim ele fecha o conteúdo.

[06:25] Preciso também nos parágrafos botar p. Reparem que não estou digitando o p. Eu coloco a barra, e como estamos usando um editor de código, ele já faz o favor de complementar para mim o que está faltando.

[06:45] Com isso aqui, nós já temos um título e três parágrafos. 

[06:50] Vamos salvar o arquivo. Ou, se você quiser ser mais rápido, ctrl+s. Vamos voltar no navegador e recarregar a página. Ou também com o atalho ctrl+r. 

[07:06] Reparem nas modificações que já foram feitas. Temos o conteúdo quebrando a linha, porque o marcamos com os parágrafos. Temos um título com uma fonte maior e em negrito, porque usamos a tag do h1, e já começamos a ter o nosso conteúdo estruturado. 

[07:27] Isso é o primeiro passo para modificar e estruturar nosso conteúdo.

[07:35] Agora, vamos evoluir o conteúdo marcando todas as informações do meio do texto que colocamos em destaque.

# Melhorando o texto

[00:00] Na aula passada, configuramos basicamente o texto que vai ser o miolo da nossa página. Mas ele ainda não está perfeito. Já marcamos o conteúdo de um título, de parágrafos, já dividimos esses conteúdos, e hoje nossa página está assim. Um título com uma fonte grande e em negrito e parágrafos separados. Temos o título h1 e todos os parágrafos separados. 

[00:35] Só que na nossa página queremos dar destaque para algumas informações, por exemplo, o nome “Barbearia Alura”. Também queremos nossa missão em itálico. Vamos fazer esses detalhes passo a passo.

[00:53] O primeiro deles é transformar Barbearia Alura em um texto de destaque. Geralmente, esse texto de destaque se apresenta em negrito, porque dá uma importância visual e semântica para o conteúdo. 

[01:11] Já falamos que as tags servem para marcar o início e o final do conteúdo. Logo, Barbearia Alura precisa estar com uma tag no início e uma no final. Essa tag que serve para marcar a importância de um conteúdo leva o nome “strong”. Em uma tradução, seria “forte”. 

[01:40] Quando usamos a palavra strong para marcar a tag e salvamos usando ctrl+s, voltamos para a página e recarregamos, imediatamente vemos que o conteúdo foi marcado com negrito. O negrito é só um detalhe visual sobre essa tag. Ela serve, novamente, para dar uma importância para aquela palavra, para aquele conteúdo. 

[02:10] Já que isso foi feito, vamos marcar a linha inteira com itálico. Queremos colocar ênfase no texto. 

[02:20] Para usar a tag da ênfase usamos em. Essa tag vai começar no início do texto, dentro do nosso parágrafo, e vai terminar no final do texto, também dentro do parágrafo. Essa é uma tag que vai marcar todo o conteúdo e transformar a linha inteira em itálico.

[02:45] Se salvarmos, voltarmos para o navegador e recarregarmos a página, veremos que essa transformação já foi aplicada. 

[02:54] Para complementar, vamos marcar nossa missão com negrito, para dar ainda mais ênfase e marcar esse texto como muito importante.

[03:07] Dentro, antes das aspas, vamos botar a tag strong. E depois das aspas, antes do ponto, vamos fechar a tag.

[03:19] Voltando ao navegador essa aplicação já foi feita. 

[03:28] Resumindo, marcamos a Barbearia Alura como um conteúdo importante, transformamos a linha inteira para ter ênfase no nosso texto, e dentro da linha, ainda marcamos uma frase como importante. Vamos reparar que no HTML temos a tag parágrafo, dentro dela a tag de ênfase e dentro dela a tag de strong. Uma tag dentro da outra. Usamos o HTML dessa forma. Marcamos um conteúdo e se dentro tem um conteúdo menor que precisa de outra marcação, ele também é marcado, e dentro disso outro conteúdo ainda menor que precisa de mais uma marcação também recebe uma tag. 

[04:19] Usar uma tag dentro da outra não é problema. É como as coisas são feitas, e na leitura faz sentido quando você começa a entender todas essas tags.

[04:32] Nosso próximo desafio é como expandir o texto, como ir além desses conteúdos. Mas para isso, vamos parar por aqui e se ver na próxima aula.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Crie o arquivo **index.html**.

2) Copie o conteúdo do texto base, que você baixou no início desta aula, para dentro do arquivo **index.html**.

3) Marque o título do texto e os seus parágrafos, usando as **tags HTML** próprias para isso:

```
<h1>Sobre a Barbearia Alura</h1>

<p>Localizada no coração da cidade a Barbearia Alura traz para o mercado o que há de melhor para o seu cabelo e barba. 
Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

<p>Nossa missão é: "Proporcionar auto-estima e qualidade de vida aos clientes".</p>

<p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
```

4) Destaque algumas informações do texto, deixando-as em **negrito**. Da mesma forma, dê ênfase em alguns pontos do texto, deixando-os em *itálico*. Use as **tags HTML** próprias para isso:

```
<h1>Sobre a Barbearia Alura</h1>

<p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

<p><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

<p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
```

# O que aprendemos?

Nesta aula, aprendemos:

- Uma introdução ao HTML e às suas **tags**
- Como definir o título e os parágrafos de um texto
  - Utilizando as *tags* **<h1>** e **<p>**, respectivamente
- Como dar destaque para algumas informações do texto, deixando-as em **negrito**, utilizando a *tag* **<strong>**
- Como dar ênfase para algumas informações do texto, deixando-as em *itálico*, utilizando a *tag* **<em>**

