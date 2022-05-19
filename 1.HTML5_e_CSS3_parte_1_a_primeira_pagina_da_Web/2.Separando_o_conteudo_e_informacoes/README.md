# Projeto da aula anterior

Caso queira, você pode baixar [aqui](https://caelum-online-public.s3.amazonaws.com/1179-html5-css3/01/aula-1-completa.zip) o projeto do curso no ponto em que paramos na aula anterior.

# Estrutura básica

[00:00] Nas aulas passadas, nós começamos a criar o nosso HTML, a modificar o texto para ele ter uma formatação e o significado que nós queremos. Só que precisamos dar um passo atrás para pensar de forma mais ampla nesse HTML.

[00:17] O que fizemos para que o nosso navegador soubesse que aquele arquivo abriria no navegador? Que seria uma página da web? Simplesmente colocamos .html no nome do arquivo. Só que não é apenas isso que o navegador precisa de informação para renderizar nossa página de forma correta.

[00:41] Neste curso, estamos abordando a versão 5 do HTML. Como o navegador vai saber isso e não colocar a versão 3 ao invés da 5, por exemplo, na nossa página, fazendo ela parar de funcionar?

[00:56] Precisamos estruturar o nosso conteúdo e passar informações para o navegador, para que ele consiga transformar a nossa página e lê-la da forma correta. Para isso, precisamos falar de uma tag muito importante que vai na primeira linha do arquivo: a tag DOCTYPE.

[01:23] Por padrão, escrevemos essa tag com o nome todo em maiúsculas. As outras tags do HTML não precisam seguir esse padrão, podem estar em minúscula ou maiúscula, mas, por padrão, escrevemos o nome dessa tag em maiúsculo para que o navegador e para que todos os desenvolvedores possam ler este padrão. 

[01:46] Essa tag tem alguns detalhes. O primeiro deles é que o primeiro caractere dentro dela tem uma exclamação. Essa exclamação serve para que essa tag seja identificada como DOCTYPE. E outra informação que colocamos é a versão do HTML que estamos usando. No caso, estamos usando a versão 5. Ela trouxe várias modificações e modernidades para o código. Uma delas é que não precisamos mais botar a versão 4.0, 3.0 ou 5.0. Se declararmos DOCTYPE html, estamos dizendo para o navegador que estamos usando a última versão disponível do HTML.

[02:37] Como estamos fazendo uma página extremamente moderna, usando o que há de mais novo, a tag html atende aos nossos requisitos.

[02:48] Se salvarmos esse arquivo e voltarmos ao navegador, recarregarmos a página, vamos reparar que nenhuma mudança aconteceu no visual, mas uma mudança muito brusca aconteceu no entendimento do navegador sobre esta página.

[03:06] O HTML ainda tem mais uma tag estrutural, que é a própria tag HTML. Ela é uma tag de conteúdo que serve para marcarmos tudo que é, dentro desta página, o HTML que vai ser renderizado no navegador. 

[03:27] Como essa tag é de conteúdo, ela precisa abrir na primeira linha, e na última linha, a última informação vai ser o fechamento dessa tag /html.

[03:39] A tag do DOCTYPE não precisa ser fechada. Ela é uma tag de informação, não de conteúdo. E a tag HTML, por ser uma tag de conteúdo precisa marcar tudo que está dentro. Só que fica sempre muito difícil de ler o texto se ele estiver todo na linha da esquerda. Para isso, vamos usar a indentação e com o tab vamos jogar todo esse conteúdo para a frente. 

[04:07] Agora fica muito fácil lermos o que está dentro do HTML, porque está tudo espaçado.

[04:18] Conseguimos organizar o nosso conteúdo para que ele seja melhor entendido pelo navegador e que esteja estruturado corretamente. É importante destacar que os navegadores modernos, como o Google Chrome, como o Firefox, Microsoft Edge tentam te ajudar se você deixa de acrescentar uma informação, por exemplo. 

[04:47] Nossa página funcionou quando não colocamos a tag HTML ou a DOCTYPE, mas por ser um padrão de projeto, é extremamente importante que sempre adicionemos as tags. Mesmo que o navegador hoje não deixe de rodar a página por falta de informação, não sabemos como vai ser o dia de amanhã e como os navegadores vão se comportar. É importante que nossa página esteja correta independente do que o navegador está fazendo.

[05:14] Na próxima aula vamos aprender como melhorar ainda mais essa marcação, como lidar com acentuações, título da página, etc.

# Passando dados para o navegador

[00:00] Na aula passada, nós criamos a estrutura do nosso HTML. Usamos a tag DOCTYPE, a tag HTML. 

[00:06] Agora, vamos evoluir, passando mais informações para o navegador. O navegador precisa de informações para renderizar nossa página corretamente. Por exemplo, se o sistema operacional do seu telefone, do seu computador ou até mesmo do seu navegador está usando o idioma inglês, você não vai conseguir exibir os acentos da página. 

[00:27] No nosso caso, no meu computador, como tudo está em português, os acentos aparecem perfeitamente. Pode ser que isso não aconteça na sua página. 

[00:36] Como podemos resolver isso? Ou para que independente da configuração do meu usuário, minha página esteja correta? Precisamos passar a informação corretamente. Para isso, criamos a tag meta. 

[00:50] A tag meta é escrita da seguinte forma dentro do nosso HTML: meta charset=”UTF8” entre os sinais < e >.

[01:11] Vamos quebrar essa tag passo a passo para entendermos. O nome da tag é meta, ela passa informações para o navegador. Dentro dela, reparem que diferente do h1, que é uma tag de conteúdo, colocamos uma propriedade dentro dela. 

[01:30] Temos o atributo charset, que é o conjunto de caracteres, o characters set, que é o dicionário que estamos escolhendo. E escolhemos o dicionário UTF8. Ele tem as linguagens Unicode, ASCII, mas o mais importante que você deve saber é que ela tem todos os caracteres que são usados na maioria das línguas da Europa, da América Central, América do Norte, América do Sul. A maioria das linguagens com que trabalhamos no dia a dia.

[02:02] Com esses caracteres, vamos resolver o problema do acento. Ele tem ç, crase, acentuação de ~, qualquer uma que usamos na língua portuguesa.

[02:14] Na nossa página, recarregando, não vai fazer diferença nenhuma no meu computador. Pode ser que no seu ele tenha consertado os acentos.

[02:25] Também precisamos dizer para o navegador qual é a linguagem da minha página. Muitas vezes estamos usando o navegador e ele se oferece para traduzir uma página. Por que ele faz isso? Ele entende que uma página está, por exemplo, em inglês, e que seu sistema operacional está em português, então te oferece essa vantagem.

[02:46] Além dele ler o conteúdo, nós costumamos informar qual é a linguagem da página. Fazemos isso dentro da tag HTML. Vamos adicionar a propriedade lang, de language, idioma, e dentro vamos usar PT-BR, que é português do Brasil.

[03:08] Com isso, temos a página sendo entendida em português. Se algum usuário que não entende português estiver lendo nossa página, o navegador vai oferecer a opção de traduzir.

[03:21] Temos tudo que precisamos para que o conteúdo da nossa página seja lido perfeitamente.

[03:27] Além disso, toda vez que estamos navegando, costumamos olhar para a aba do navegador para saber o nome da página, e a nossa hoje exibe o nome “index.html”. Vamos consertar.

[03:42] Para fazer isso, usamos uma tag chamada “title”, que é o título da página. Vamos usar o nome “Barbearia Alura”. E salvamos a página. 

[04:02] Quando voltarmos ao navegador e recarregarmos, o título está lá. 

[04:07] É importante passar todas essas informações para o navegador para que nossa página seja lida e exibida corretamente.

[04:16] Por hoje é só. Na próxima aula vamos ver como quebrar ainda mais esse conteúdo e fazer nosso código ficar menos complexo. Te vejo lá.

# Separando conteúdo e informações

[00:00] Na aula passada, demos ao navegador mais informações sobre o idioma da nossa página e consertamos o título que estava na aba do navegador. 

[00:07] Mas se repararmos no nosso conteúdo, a tag meta e title estão perdidas no meio do que seria o que iríamos exibir na nossa página. Reparem que se olharmos no navegador, vamos ver todo o nosso conteúdo, mas as tags não estão exibidas, porque uma coisa é o que estamos exibindo na página dentro da janela branca do navegador e outra coisa são as informações que estamos passando para ele.

[00:37] Dentro do HTML existe essa divisão estrutural. Como ela é feita? 

[00:43] O HTML é dividido em duas partes. A primeira delas é o head, e a segunda é o body. Vamos pensar o seguinte, traduzindo os nomes: head é cabeça e body é corpo. Se pensarmos em um documento, a cabeça são as informações que estamos passando para o navegador e o corpo são as informações que queremos exibir na página. 

[01:14] A tag meta é uma informação que quero passar para o navegador. Essa informação vai dentro do head. A tag title é uma informação que quero passar para dentro do navegador. Também vai dentro do head. E toda a informação que quero exibir, todo o texto que já criei vai ser jogado dentro do body. 

[01:39] Reparem que para ficar correto o código, ele precisa ser bem indentado. É o que eu falei na aula sobre colocar o espaçamento correto na estrutura do navegador. Para isso, vou jogar os parágrafos para a frente.

[01:57] Conseguimos visivelmente entender que os elementos estão dentro do body. E conseguimos entender visivelmente que os outros elementos estão dentro do head. É assim que fazemos para criar a estrutura do HTML e para que ele esteja correto na hora de ser apresentado ao navegador. 

[02:18] As informações que estamos passando para o navegador ficam no head e as informações que queremos exibir na nossa página ficam no body. Com isso, concluímos a estrutura da nossa página. Vamos evoluir colocando mais conteúdo, mexendo nesse conteúdo e melhorando a página que temos até o momento.

# Consolidando o seu conhecimento

Chegou a hora de você pôr em prática o que foi visto na aula. Para isso, execute os passos listados abaixo.

------

1) Defina a estrutura básica do HTML **index.html**, não esquecendo de definir a linguagem da página:

```
<!DOCTYPE html>
<html lang="pt-br">
    <h1>Sobre a Barbearia Alura</h1>

    <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
    Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

    <p><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

    <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
    O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>

</html>
```

2) Passe as informações de renderização da página para o navegador e defina o seu título:

```
<!DOCTYPE html>
<html lang="pt-br">
    <meta charset="UTF-8">
    <title>Barbearia Alura</title>

    <h1>Sobre a Barbearia Alura</h1>

    <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
    Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

    <p><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

    <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
    O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
</html>
```

3) Por fim, separe as informações e conteúdo da página:

```
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <title>Barbearia Alura</title>
    </head>
    <body>
        <h1>Sobre a Barbearia Alura</h1>

        <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. 
        Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

        <p><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

        <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. 
        O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
    </body>
</html>
```

# O que aprendemos?

Nesta aula, aprendemos:

- A definir a estrutura básica do HTML

  - Com a *tag* `DOCTYPE`, definimos qual versão do HTML estamos utilizando

  - A 

    tag

    `<html>`

    , que marca o conteúdo a ser renderizado no navegador

    - Dentro desta *tag*, podemos definir a linguagem da página, através da propriedade **lang**

- Como passar as informações do *encoding* da nossa página para o navegador, através da *tag* **<meta>** e da propriedade **charset**

- Como definir o título de uma página, através da *tag* **<title>**

- Como separar as informações que estão sendo passadas para o navegador, utilizando a *tag* **<head>**

- Como separar o conteúdo da página, utilizando a *tag* **<body>**



