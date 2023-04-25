<link rel="stylesheet" href="style.css"> - link para referenciar o css dentro do codigo.


<body>

 - O conseito de caixa (BOX) se dá ao html, pois quando declaramos uma div class, para o codigo isso é uma caixa.
Vale ressaltar que todas as tagas que se " encolhem" também são caixas dentro de caixas.>

  <div class="page">

antes tinhamos colocado o 'header' porém, não é uma bia pratica colocar o nav dentro do header por serem parecidos em carateristicas, tipo irmaos!
entao colocamos tag <a id="logo">, para referenciar a logo e separar as navegações(as interações.)
    <nav>
      <a id="logo" href="#">
        <img src="image/logo.svg" alt="Treine.me">
      </a>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Sobre</a></li>
          <li><a href="#">Treinar</a></li>
        </ul>

    </nav>
 - a tag 'href="#"' é uma forma de dizer que nao há um link ou um caminho para seguir.


    <main>

    <section class="text">
        <h1>Treinos exclusivos para você!</h1> titulos maiores 

        <p>Nós criamos treinos <strong>exclusivos e únicos para você.</strong>  
          Invista no seu corpo e <strong>tenha muito mais performance</strong>  e qualidade de vida.</p> - parágrafos <strong> - usamos para manupular as cores e aspectos.

        <button>
          <img src="image/whats.svg" alt="icone do whatsapp">Comece já
        </button> - criar um botao na tela. 
    </section>

    <img src="image/img.png" alt="Desenho de mulher pulando corda na academia">

    </main>
      <footer>
    fale conosco no instagram <a href="https://instagram.com/treineme" target="_blank"> @treine.me </a>
      </footer>

  </div>

    <img src="image/balls.svg" alt="bolinhas verdes no canto inferior da página.">

</body>
</html>

<!--As propriedades das caixas são as larguras, alturas, conteúdo, espaçoas ao redor da caixa, tem a ideia de "bordas", e dentro das caixas tem seus preenchimenstos.-->
<!--Quando você colocar uma margem no site que estiver desenvolvendo, por padrao o Google Chrome da uma borda de 8px( um espaçamento do final da pagina para a borda criada.)-->



PARA CSS: 

body{
  margin: 0px;  - margem para zerar a padrao ou aumentar o tamanho do espaço da borda 

  min-height: 100vh; - tag utilizada para fazer com que se visualiza 100% de tudo que está fora da margem do body. pode ocorrer de nao completar a pagina toda.
  utilizado para dizer ao motor de navegação que no minimo é 100 view port, ou seja, se passar tudo bem, mas ele mantem sua caracteristica ate 100vh. 
  colocando somente o heigth entende que o valor é fixo. 
}

.page {
  border: 1px solid red; - coloca borda na página
  
  width: 1000px; - coloca o tamanho da "caixa" de ponta a ponta.
  
  padding: 8px; - preenchimento, ou seja, um espaço em brnco entre a borda e o conteúdo.
  
  margin: 65px auto 0;  - na opção automático, faz com que a caixa fique centralizada. Para delimitar os espaços dos demais conteúdos, pasta colocar os valores respeitando a regra de: em cima vem primeiro depois centralização e pra baixo.
}

OBS.: por padrão, os codigo já vem com o "flex-direction: row;", logo nao é necessário colocar no codigo. essa tag significa a direção que sera colocado os itens da pagina. por esse motivo colocamos "display: flex;" para que possamos orientar novas posições dos itens da pagina.

header {

  display: flex; - Faz o item/ elemetento selecionado ter a disponilidade de ser reposicionado.

  justify-content: space-between; -  significa conteudo 'justificado' e'espaço entre', se observar a imagem da pagina, irá fazer mais sentido com o significado, ou seja, os elementos da pagina sao espaçados de forma igual de acordo com os limites dados. 
  
  align-items: center;  -  Usado para alinhar de acordo com o eixo dos itens. O eixo sempre será por padrão o 'MAIN AXIS' eixo principal, geralmente da esquerda para direita. 

  margin-bottom: ;  - 'margin-bottom' (margem de baixo) serve para dar limites as partes inferiores do conteudo especificado.
}

ul {
  display: flex;

  gap: 48px;  -  GAP é o espaçamento entre os itens que está sendo separado. Nesse caso é o 'UL', são os menus na parte superior da pagina.

  list-style: none;  -  Retira as bolinhas ou marcações de listas.

  margin: 0px;
  padding: 0px;  -  nesse caso está sendo retirado as margem e de preenchimentos para que se caso voce utilize uma imagem atras desse menu expecifico, nao mostrar o uma margem e preenchimento dos menus .
}

ul li a:hover{
  font-weight: bold; - ':houver' é para uma interação quando passar o mouse em cima do item da pagina, onde ele fica negrito.
}

border-radius: 4px; - serve para arredondar os botoes. quanto ao px, é refetente aos cantos da caixa botton.

text-transform: uppercase; - faz com que toda a escrita fique em maiúscula. 

CONSEITOS: 

REFATURAÇÃO - é quando você autera o codigo sem modificar o resultado final do site.

MUITO IMPORTANTE!!! - Lembre-se de colocar os links das fontes utlizadas no projeto. isso ajuda a ter mais velocidade e certeza de estar funcionando.