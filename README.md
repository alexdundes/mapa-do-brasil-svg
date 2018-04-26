# mapa-do-brasil-svg
Mapa do Brasil em SVG para ser usado em sites como gráfico (indicativo)

## História

Eu precisava construir um sistema em que indicava por estado uma cor e quantidade... procurei por várias soluções, mas o que eu queria era bem simples. Então resolvi criar a minha própria.

Comecei pegando um SVG pronto deste site: https://simplemaps.com/resources/svg-br

Depois editei algumas características como cor inicial e colocar caixas de textos sobre os estados para representar os números.

Para isso usei o seguinte editor de SVG: http://editor.method.ac/

Por fim, abri o arquivo salvo pelo editor anterior e ajustei muita coisa na mão até ficar como eu realmente queria.

obtendo então o arquivo brasil.svg

## Como usar

Assegure que esteja usando jQuery no seu site
Inclua uma tag no seu código:

```html
<div id="mapa-do-brasil"></div>
```

e no javascript inclua esse código

```javascript
        $("#mapa-do-brasil").load("brasil.svg",
            function () {
                // pinta o estado de SP de vermelho
                $("#mapSP").css("fill", "#e74c3c");
                // coloca o número 15 sobre SP
                $("#lblSP").text("15");
                // pinta o estado de RJ de verde
                $("#mapRJ").css("fill", "#62cb31");
                // coloca o * sobre RJ
                $("#lblRJ").text("15");
            }
        );
```
