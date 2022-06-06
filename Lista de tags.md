não sei o que acontece mas acho que se eu não especificar o tipo de arquivo ele não vai ser nada além de uma nota então eu vou usar como caderno pra anotar as tags
______________________________________________________________

<!> Monta a base do html sozinho, lembrando de mudar a linguagem para pt-br

<h1> Serve para criar um título no site 

<hr> Cria uma linha que divide o site

<p> É um parágrafo e sempre escreve na mesma linha

<br> Serve pra pular uma linha no meio do parágrafo

<!-> Serve para criar comentários no meio do código 

<&> Alguns caracteres especiais usam o & para aparecer 

"&#x" Usando &#x e mais um código aparece um emoji específico  

<tabindex> numera a ordem que vai usando TAB no site

______________________________________________________________

<img> serve pra exportar uma imagem 
  <src=""> significa source, é o caminho da pasta do arquivo de imagem 
    <Atalho>: Ctrl + Barra de espaço pra aparecer os arquivos dentro da pasta
  <alt=""> é o texto alternativo pra aparecer caso a imagem não possa aparecer

<link:favicon> Serve para escolher o favicon do site. Favicon é o ícone que fica na aba das páginas

______________________________________________________________
<envelopar> atalho para colocar tags em textos Ctrl + Shift + P

______________________________________________________________

<strong> Serve para colocar frases em negrito tendo semântica (Alternativa não semântica sendo apenas a forma do conteúdo é a tag <b>)

<em> Serve para deixar as frases em itálico tendo semântica (Tag <i> como não semântica)

<mark> para destacar como marcar texto (amarelo por padrão)

<big> Texto maior que o normal como destaque (obsoleto)

<small> texto pequeno mas com significado de importância

<del> texto deletado, deve ser lido mas desconsiderado

<ins> texto inserido, enfâse e que foi adicionado depois (sublinhado mas com importância, com semântica)

<u> sublinhado (sem semântica)

<sup> texto sobrescrito

<sub> texto subescrito

<addres> infomações adicionais de contato

<mark> destaque como marca texto (background amarelo)

______________________________________________________________

<code> serve para mudar o código fonte do texto e deixar monoespaçado

<pre> utiliza todo o espaço das linhas abaixo incluindo tabulação

<q> citação simples colocando aspas mas com semântica 

<blockquote> citação completa, frases de livro por exemplo
  é possível colocar a origem da citação se ouver um link adicionando <cite> no primeiro blockquote

<abbr> colocar nome completo de uma sigla ou comentário dentro do site ao passar o mouse em cima do conteúdo

<bdo> mudar a direção de leitura das letras, invertendo elas

______________________________________________________________

<ol> Uma lista com ordem certa, type 1 por padrão
  <type> 1, A, a, I, i
  um <li> para cada item da lista

<ul> Lista sem ordem definida, type disc por padrão
  <type> disc, circle, square
  um <li> para cada item da lista

<dl> Lista de definição: Mostra um item e uma descrição logo em seguida para só então passar para o próximo item
  <dt> para cada item, seguido de um <dd> com a descrição desse item
  
______________________________________________________________

<a> Serve para colocar links no sites. Parâmetros abaixo
  <target> e <rel>
    <target>: _blank para o link abrir outra aba
              _self para manter a pesquisa na própria aba
    <rel> parâmetro para SEO
      rel="next" próxima página do site
      rel="prev" página anterior do site
      rel="external" link não faz parte do site
      rel="nofollow" o site do link não teve criar relações com o site que o referencia
    
    <title> diz o nome da página quando mantém o mouse por cima do link

  <download> e <type>  
    <download> serve para indicar que arquivo deve ser baixado (precisa ser o mesmo marcado no <href> da tag <a>)
    <type> serve para indicar qual o tipo de arquivo que está sendo baixado. Cada tipo de arquivo pode ser verificado no site https://www.iana.org/assignments/media-types/media-types.xhtml

  <href> usando # no link ele vai direto para a parte da página marcada
    <a href="#parte3"> 
    <p id="parte1">
    <p id="parte2">
    <p id="parte3">
      neste caso pularia para onde a parte 3 estivesse no site

______________________________________________________________

<picture> serve para criar uma imagem dinâmica, imagem que muda de tamanho se ajustando ao tamanho da tela. 
  se coloca as imagens da maior para a menor usando:
    <source media="(min-width: tamanho da imagem )" srcset="local da imagem" type=" tipo da imagem como: image/png">  
  usando <img> quando chegar na imagem de menor tamanho
  a ordem importa, deve ser da maior para menor, de baixo para cima

<audio> para reproduzir áudios no site
  <autoplay> inicia sozinho se o navegador permitir
  <controls> para exibir os controles do áudios
  <loop> mantém o áudio sempre em reprodução
  <preload> pare definir como carregar quando o site for acessado
    <metadata> apenas informações como tempo de duração
    <auto> carrega todo o áudio (consegue banda)
    <none> não carrega nada do áudio

  também é possível usar a tag <source> dentro da tag <audio> em caso de multiplos tipos de arquivo

<video> funciona como <picture> e <audio>
  <width> para tamanho que o video ocupa visualmente
  <poster> capa do vídeo

Grouping Tags
  <header> cabeçalho
  <footer> rodapé
  <main> conteúdo principal

<button> Cria um botão 

<table> cria uma área de tabela
  <thead> cabeçalho da tabela, primeira linha com título e marcações de cada coluna
  <tbody> corpo da tabela, são os itens da tabela em si
  <tr> cria uma linha para a tabela
    <td> cria a coluna dentro da linha
  <border> borda da tabela, normalmente se coloca em 0 ou não coloca para definir isso apenas com o CSS

______________________________________________________________

<form> serve para criar uma área de formulário 
  <action> pode colocar uma página que deve seguir após responder e enviar o formulário
  <method 
    GET - O resultado do fomulário aparece no link
    POST - O resultado fica oculto no site
  >
<input
  Type="" name="">
    Types de input
      <text> serve para textos
      <password> para senhas, muda os caracteres para asteriscos para serem visualmente secretos
      <email> permite apenas email, não funciona sem um @ com endereço de email funcional
      <radio> funciona para seleção de opções mas é necessário que haja mais de um e que o name deles sejam os mesmo para que possa haver apenas uma seleção como no exemplo a seguir
        <input type="radio" name="mes"> Janeiro
        <input type="radio" name="mes"> Fevereiro
      <checkbox> cria um check box
      <submit> serve pra o envio do formulário
      <color> para selecionar uma cor
      <date> seleciona uma data
      <datatime-local> seleciona data e hora
      <month> seleciona um mês
      <range> cria uma linha para selecionar a medida
      <number> aceita apenas números
      <search> não sei pra que serve na verdade mas acho que tem a ver com semântica e criar um box essencialmente para fazer pesquisas dentro do site
      <tel> número de celular, acho que também é semântico já que nada é formatado
      <time> seleciona a hora
      <url> aceita apenas url
      <week> seleciona a número da semana do ano
      <hidden>  o tipo hidden serve para gravar informações que o usuário não precisa preencher ou alterar
      <file> serve para que o usuário possa enviar um arquivo
        <input type="file" accept="image/*"> accept serve para definifir que tipo de arquivo pode ser enviado, o * serve para dizer que qualquer tipo de arquivo que seja imagem é válido
        <form enctype="multipart-form/data"> necessário para que o envio do arquivo ocorra com segurança e não se perca no meio do caminho 
    

<select name=""> cria uma área de seleção de escolhas dadas pelo desenvolvedor
  cada opção é feita com a tag:
  <option> option tem alguns parâmetros
    <value=""> serve para dizer que valor ele vai retornar e que pode ou não aparecer na url depois do envio do formulário
    <selected> serve para determinar qual das opções vem selecionada por padrão, caso não seja definido a primeira option sempre é o padrão
    <multiple> faz com que a seleção vire de multipla escolha mas antes deve haver outra tag para dizer quantas opções podem ser escolhidas. tag a seguir
    <size> diz a quantidade de opções que podem ser escolhidas juntas

<texarea name=""> serve para criar uma área de texto maior que o normal, podendo ser redimensionada pelo próprio usuário, mas acho que tem como mudar isso com as CSS

<button> serve para criar um botão novo, dentro da tag <form> ela vai enviar o formulário, mas diferente do <input type="submit"> ela é programável e pode ser usada em outras áreas do código além do <form>

<label> Serve para criar um texto que redireciona para outra área da página
    <label for="nome">Digite o seu nome</label>
      <for> indica para onde o label irar redireionar, só marcar o id que quiser. nesse caso o label iria redirecionar para o input de texto com o id "nome"

    <input type="text" name="" id="nome">

<fieldset> serve para criar uma área reservada no formulário, como por exemplo uma área só para dados pessoais e outro apenas para dados profissionais
  <legend> cria uma legenda/título para o <fieldset>

<input required> required serve para fazer com que o campo seja preenchido obrigatoriamente

<input minlenght> serve para determinar um mínimo de preenchimento do campo
<input maxlenght> serve para determinar um máximo de preenchimento do campo
<input type="number" step="2"> step serve para determinar de quantos números ele deve aumentar ou diminuir no valor 
<input min="10"> serve para determinar um valor mínimo requerido, também serve parqa datas se colocar o valor no formato internacional ano-mês-dia
<input max="10"> serve para determinar um valor máximo permitido, também serve parqa datas se colocar o valor no formato internacional ano-mês-dia
<input partten=""> serve para criar um requerimento no campo, como por exemplo, exigir que o campo tenha um @email 
<input placeholder=""> serve para deixar uma mensagem no campo de input, se for possível digitar nele, e remove automaticamente quando algo é inserido
<input autofocus> quando a página é aberta o curso já abre dentro da caixa de input para poder inserir as informações 
<input autocomplete=""> 
  off- não salva nesse bloco 
  on-  passa a salvar as infomações para outros futuros acessos
______________________________________________________________

<background-image>: linear-gradient(135deg , purple, yellow);
  degradê de fundo do site

background-attachment: fixed; 
  usado para o gradiente seguir na tela inteira mesmo depois do scroll

"@font-face" para usar fontes externas
      font-family: "Love" ;
      src: url("fonts/love\ larry\ ttf.ttf") format("truetype");
      font-weight: normal;
      font-style: normal;
      /*Tipos de Formats
      - opentype (otf)
      -truetype (ttf)
      -embedded-opnetype
      - trutype-aat
      -svg */

<id> em CSS é o "#"
<class> em CSS é "."

<pseudo classes > em css é representado por ":" e é utilizado para mostrar "estados"

<pseudo elemtentos> em css é representado por "::" e serve para adicionar elementos em linhas específicas 

Modelo de Caixas
  box-level
    
    ordem do shorthand <border>
      border-width: 10px;
      border-style: solid;
      border-color: darkslategray;
        border: 10px solid darkslategray;

    ordem do shorthand <padding>
      padding-top: 10px;
      padding-right: 10px;
      padding-bottom: 10px;
      padding-left: 10px;

      podendo colocar:
      1 valor para todos os lados
      2 valores para vertical e horizontal
      4 valores para cada lado seguindo sentido horário
      auto em right e left para centralizar automaticamente
        padding: 10px auto 10px auto;

    ordem do shorthand <margin>
      margin-top: 10px;
      margin-right: 10px;
      margin-bottom: 10px;
      margin-left: 10px;

      podendo colocar:
      1 valor para todos os lados
      2 valores para vertical e horizontal
      4 valores para cada lado seguindo sentido horário
      auto em right e left para centralizar automaticamente
        margin: 10px auto 10px auto;

    ordem shorthand <outline>
      outline-width: 5px;
      outline-style: dashed;
      outline-color: salmon;
        outline: 5px dashed salmon;

:root serve para criar coisas na raiz do código de css

* usado para criar regras globais de todo o código html

<box-sizing>: serve para mudar o padrão das caixas
  content-box tamanho da caixa vai manter o tamanho do conteúdo
  border-box vai manter o tamanho da caixa independente de margin ou padding, o tamanho do conteúdo diminui

<a>
  <text-decoration
  none pra tirar
  overline pra linha acima do texto
  underline para linha abaixo do texto>

  <text-transform
  uppercase para todos maiúsculos
  lowercase para tudo minúsculo>

<letter-spacing> px espaçamento entre as letras
<word-spacing> px espasçamento entre as palavras
<line-height> altura de cada linha, distância entre elas

<inherit> serve para forçar uma herança
  <box font-size="15px"> boz vai ficar com 15px
  <h1 font-size="30px"> h1 vai ficar com 30px 
  nesse ponto se tiver um h1 dentro de box ele vai ficar com 30px, para forçar ele a herdar o tamanho do box podemos usar o inherit

  <box> <h1>{
    font-size="inherit" 
  } isso fará o h1 herdar a propriedade do box 

<background-repeat> repetoção da imagem no fundo do site
  <norepeat> não repete
  <repeat> padrão
  <repeat-x> repete horizontal
  <repeat-y> repete vertical

<background-size> tamanho do background