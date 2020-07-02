# @media -> média query
-- É uma técnica de CSS introduzida no CSS3. usa a regra **@media** para incluir     um bloco de propriedade CSS apenas se uma determinada condição for verdadeira
  
   # ex: -> quando o body for menos de 600px vai ficar azul->blue
      @media only screen and (max-width: 600px) {
         body: background-color: blue;
      }


**é mais prático desenha primeiro para dispositivos menos.** 
**envez de mudar a largura quando a tela for menor, muda-se que a tela for maior**

*+outros Breakpoint+*
podem sem adicionados vários breakpoints: [desktop-tablet-phone]

ex: 
   adicinado mais uma media query (em 600px), e um conjunto de novas clases para dispositiovos maiores que 600px (mas menores doque 768px):

   [class*="col-"] {width: 100%}
   @media only screen and (min-width: 600px) {
      .col-s-1 {width: 8.33%;}
   }
   @media only screen and (min-width: 768px) {
      .col-1 {width: 8.33%;}
   }

**another example**
# Extra small devices (phones, 600px and down)
@media only screen and (max-width: 600px) {...}

# Small devices (portrait tablets and large phones, 600px and up)
@media only screen and (min-width: 600px) {...}

# Medium devices (landscape tablets, 768px and up)
@media only screen and (min-width: 768px) {...}

# Large devices (laptops/desktops, 992px and up)
@media only screen and (min-width: 992px) {...}

# Extra large devices (large laptops and desktops, 1200px and up)
@media only screen and (min-width: 1200px) {...}




*************************************************+*+***********++*******+**
# orientacion -< Portrait / Landscape >
-- media query podem tambem ser usados para mudar o layout de uma página dependendo      da orientação do browser

ex: a pagina terá fundo azul se a orientação for paisagem->landscape
   @media only screen and (orientacion: landscape){
      body {background: blue}
   }



*************************************************+*+***********++*******+**
# ocultar elementos com media query
-- Outro uso comum de consultas de mídia é ocultar elementos em diferentes tamanhos      de tela:
ex: @media only screen and (max-width: 600px) {
  div.example {
    display: none;
  }
}




*************************************************+*+***********++*******+**
# layouts flexiveis
um uso comum é criar layouts flexivéis.
ex: layout varia entre quatro, dois e colunas completas, dependendo das diferentes        tamanho de tela 
   **as telas que são <=992px vão de 4 para duas colunas**
   @media screen and (max-width: 992px) {
      .column {
         width: 50%;
      }
   }
   **as telas que são <=600px vão de 2 para 1 coluna**
   @media screen and (max-width: 600px) {
      .column {
         width: 100%;
      }
   }


*************************************************+*+***********++*******+**
# tips
@media screen and (max-width: 900px) and (min-width: 600px) {
  div.example {
    font-size: 50px;
    padding: 50px;
    border: 8px solid black;
    background: yellow;
  }
}
# OU -> ,
@media screen and (max-width: 900px) and (min-width: 600px), (min-width: 1100px) {
  div.example {
    font-size: 50px;
    padding: 50px;
    border: 8px solid black;
    background: yellow;
  }
}



*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
*************************************************+*+***********++*******+**
