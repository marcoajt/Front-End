# Projeto da aula anterior

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/05/aula-5-completa.zip) o projeto do curso no ponto em que paramos na aula anterior.

# Cabeçalho

[00:00] O que queremos agora é criar o cabeçalho da nossa página, onde estarão o nome da nossa barbearia e as informações mais importantes do nosso site.

[00:09] Para isso, no nosso HTML, antes da primeira imagem, dentro do body, vamos criar outra divisão. Essa divisão vai ter um conteúdo. Esse conteúdo vai ser o nome Barbearia Alura. 

[00:33] Duas coisas sobre isso: essa divisão é a divisão do cabeçalho. Como isso é uma coisa muito comum em todas as páginas web, na última versão do HTML criaram uma tag específica para o cabeçalho. É uma tag mais semântica que diz para o navegador que aquilo ali é a primeira informação a ser apresentada. 

[01:01] Ao invés de div, nós vamos usar a tag header. Ao invés de fechar div, vamos fechar o header. 

[01:09] É importante destacar que header é o cabeçalho da página, e fica dentro do conteúdo, e o head é a tag padrão do HTML que serve para passarmos a informação para o navegador. Não vamos confundir as duas coisas.

[01:26] A segunda coisa sobre o cabeçalho é que queremos que o nome da nossa barbearia seja a coisa de mais destaque. Vamos entender como isso funciona no navegador.

[01:37] Salvando e recarregando a página, teremos o nome como a primeira coisa a ser lida pelo usuário. Se pensarmos em qualquer matéria de jornal ou texto, a primeira coisa que lemos é  o que está no canto superior esquerdo. Ou seja, este título é o conteúdo principal da nossa página. 

[02:02] Sempre que temos o conteúdo principal da página, o título principal, usamos a tag h1. Só que no nosso conteúdo usamos a tag h1 para o título Sobre a Barbearia Alura. Vamos trocar. 

[02:17] Sobre a Barbearia Alura passa a ter a tag h2, o Benefícios passa a ter a tag h3, e o nosso principal título, nossa informação principal, passa a ter a tag h1. 

[02:40] Se recarregarmos e voltarmos ao nosso site, veremos que ficou uma bagunça. Por quê? Usamos a tag h2 para marcar nosso CSS, usamos a tag h1 para marcar o CSS, e no cabeçalho ganhamos aquele estilo que tínhamos criado sem precisar. 

[03:04] Essa é a maior dificuldade quando criamos estilos usando tags. Por isso é sempre recomendado usarmos classe para tudo. 

[03:14] Vamos então modificar o conteúdo que já temos para que os estilos que criamos fiquem em tags. 

[03:22] A primeira coisa no nosso CSS é que  o nosso h1 tinha um alinhamento ao centro. Só que o nosso h2 também tinha a mesma informação. Ou seja, criamos dois estilos para a mesma coisa. 

[03:39] Se viermos no nosso HTML, podemos transformar em uma classe, chamando essa classe de “titulo-centralizado”, copiar isso e botar essa mesma classe para nosso h3 e copiando o nome, indo no CSS, posso apagar a declaração do h2, e onde tenho a declaração para o h1, trocar ela para .titulo-centralizado

[04:20] Com isso, temos essa mesma característica sendo aplicada nos dois elementos. Se salvarmos nosso HTML CSS e recarregarmos no navegador, nosso título Barbearia Alura já está posicionado à esquerda, nosso título Sobre a Barbearia Alura, que agora é o h2 está posicionado ao centro, e nossos Benefícios também estão centralizados. 

[04:48] Por fim, só para termos mais uma perspectiva visual e mexermos um pouco mais nos espaçamentos, vamos dar um espaço interno no nosso título principal para a esquerda. Ou seja, criaremos um espaçamento de 20px. 

[05:09] No nosso HTML, vamos dar uma classe para ele, chamando de titulo-principal. Vamos copiar isso, salvar a página, no nosso CSS vamos criar a classe titulo-principal, que vai ter um espaçamento interno para a esquerda de 20px: padding-left: 20px

[05:38] Salvando esse conteúdo, voltando para o navegador e recarregando a página temos esse respiro do nosso título para nossa página. 

[05:50] Com isso, marcamos e criamos todo o conteúdo necessário para a primeira página da Barbearia Alura.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Crie o cabeçalho da página **index.html**:

```
<header>
    <h1 class="titulo-principal">Barbearia Alura</h1>
</header>
```

2) Altere a *tag* do título **Sobre a Barbearia Alura** para `<h2>` e a *tag* do título **Benefícios** para `<h3>`. Além disso, dê uma mesma classe para os dois:

```
<h2 class="titulo-centralizado">Sobre a Barbearia Alura</h2>
```

E:

```
<h3 class="titulo-centralizado">Benefícios</h3>
```

3) No arquivo **style.css**, dê um espaçamento interno à esquerda para o cabeçalho, de 20px:

```
.titulo-principal {
    padding-left: 20px;
}
```

4) E por fim, remova os estilos das *tags* `h1` e `h2` e centralize-os em um único lugar, através da classe `titulo-centralizado`:

```
.titulo-centralizado {
    text-align: center
}
```

# Projeto do curso

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/06/aula-6-completa.zip) o projeto completo implementado neste curso.

# O que aprendemos?

Nesta aula, aprendemos:

- O conceito de cabeçalho da página e como criá-lo

- Que o cabeçalho da página deve ter mais destaque

- Que não é recomendado criar estilos usando 

  tags

  - O ideal é usarmos classes para tudo

# Conclusão

[00:00] Concluímos com sucesso a criação da página da Barbearia Alura.

[00:03] Tínhamos o desejo de criar essa página e passo a passo conseguimos.

[00:08] Obrigado por me acompanhar nessa jornada. Espero que você tenha aprendido bastante.

[00:14] Nossa página Barbearia Alura já tem agora todo o conteúdo que queríamos. Esse conteúdo não só está bem marcado com as tags do HTML, como está perfeitamente estilizado com o CSS. 

[00:25] Vamos rapidamente revisar o que fizemos. 

[00:28] No nosso HTML, falamos desde a estrutura do HTML, com as tags do DOCTYPE, HTML, head, body, como falamos também das informações que passamos para o navegador, como por exemplo o link do CSS.

[00:44] Falamos ainda de todas as tags que montam o conteúdo, desde a separação do header e das divisões, falamos de imagem, de títulos, dos textos e listas. 

[00:56] Também falamos sobre como marcar esses elementos usando identificadores e classes. Pegamos essa marcação inteira e fomos para o CSS.

[01:06] No CSS, vimos como marcar com uma tag, como marcar com identificador, como marcar com uma classe. E abordamos os detalhes principais do CSS, todas as questões das dimensões, como a largura, altura, padding, a margem. Abordamos a criação de um fundo colorido ou de uma cor no elemento. Mexemos ainda no alinhamento dos elementos, no estilo da fonte.

[01:34] Passamos por isso tudo para chegar na página da Barbearia Alura.

[01:41] Espero que você tenha aprendido muito, mas tenho certeza que você está com várias dúvidas ainda. Por exemplo, como criamos outras páginas e fazemos um link entre elas? Como colocamos um formulário de contato? Um preço? Como vendemos algo da Barbearia Alura? Como podemos criar um rodapé e outros estilos básicos que vemos em todas as páginas da web? Por isso, quero que você me acompanhe na parte 2 desse curso. Espero que você aprenda ainda mais.

[02:14] Te espero lá.

