----------------------------
  2 Grid Layout Container  |
----------------------------


2-1 Layout 
>>> Explicando funcionalidades

2-2 display: grid;
>>> exemplos de grid-template-columns (FR, %)

2-3 Grid Template Columns 
>>> grid-template-columns: minxmax (100px, 1fr) 1fr 1fr;    {100px = min e 1fr = max}
>>> grid-template-columns: repeat (3, 1fr);    {  exemplo: grid-template-columns: 1fr 1fr 1fr 1fr    ===  repeat(4, 1fr)   }  OBS: AUTO-FIT
>>> responsividade = grid-template-columns: repeat(auto-fit, minmax(100px, auto));

2-4 Grid Template Rows
>>> grid-template-row: 100px 50px 200px { muda o tamanho das linhas }
>>> pode usar repeat e minmax também.

2-5 Grid Template Areas 
>>> Define as áreas do grid na div principal com grid-template-area e em cada item o grid-area correspondente.
>>> Para usar o media query basta mudar o grid-template-area: (como se fosse o flex virando de row para column)
>>> ex: "logo nav nav"
>>>     "sidenav content advert"
>>>     "sidenav footer footer "
>>> vira: 
>>>     "logo logo logo"
>>>     "sidenav sidenav sidenav"
>>>     "content content advert"
>>>     "footer footer footer"
>>> usar "..." cria uma área vazia

2-6 Grid Template (atalho)
>>> grid-template: linha / coluna
>>> ex: grid-template: 100px 50px / 1fr 1fr ( 1ª linha com 100px, 2ª linha com 50px e duas colunas de 1fr)

2-7 Grid Gap 
>>> Um tipo de margin do grid 
>>> gap: 20px;
>>> o gap difere do margin porque quando o gap é usado apenas cria espacamentos internos, já o margin cria em volta de todo o item.
>>> gap: 20px 10px; ( gap-row de 20px e gap-column de 10px )

2-8 Grid Auto Columns
>>> Colunas criadas automaticamente

2-9 Grid Auto Rows
>>> Linhas criadas automaticamente
>>> exemplo em foto ["grid-template.jpg"] 

2-10 Grid Auto Flow
>>> Mudar o grid de row para column grid-auto-flow: column;
>>> grid-auto-flow: dense; (tira uma div que caiba num lugar diferente)

2-11 Grid
>>> Definições padrão com o display: grid

2-12 Justify Content :O
>>> Parecido com flex
>>> Eixo Horizontal

2-13 Align Content
>>> Parecido com flex
>>> Eixo vertical 


-----------------------
  3 GRID LAYOUT ITEM  |
-----------------------

3-1 Grid Column
>>> Define em qual coluna o item vai ficar.
>>> .item-1 { grid-column: 2 (diz para o grid que quer esse item na segunda coluna) }
>>> grid-column: 1 / 3; (começa na linha 1 e termina na linha 3) para ocupar toda a linha pode-se usar 1 / -1
>>> nomeando as colunas > grid-template-columns: [inicio] 1fr [meio] 1fr [fim];
>>> grid-column: inicio / fim; este item vai ocupar toda a linha

3-2 Grid Row
>>> Grid row = linhas normais
>>> Grid line = linhas do grid (tipo excel)
>>> grid-row: 2; (serve para posicionar o item)
>>> posso usar / para dizer que quero o item de um lugar até o outro: ex: grid-row: 1 / 4;  (da posição 1 até a posição 4)
>>> grid-row: span 5; (expande ele até a linha 5)


3-3 Grid Area
>>> row start / column start / muito confuso!
>>> Rever essa aula ******

3-4 Justify Self 
>>> Fala com um item específico 
>>> padrão é stretch

3-5 Align Self 
>>> Fala com um item específico
>>> padrão é stretch


=-=-=-=-=-=-=-=-=-=-=-=-=-= INÍCIO DO PROJETO WILDBEAST =-=-=-=-=-=-=-=-=-=-=-=-=-=



