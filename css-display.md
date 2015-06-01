Aprovechando que estás acá ¿Sabes cuál es la diferencia entre los **elementos de bloque** y **elementos en línea** en HTML? Si no lo sabes, esta lectura es para ti.

## Elementos de bloque

Empecemos con un ejemplo. El siguiente código HTML tiene un encabezado `h3` y un párrafo `p` **sobre la misma línea**. ¿Cómo crees que se verá el resultado?

<div data-height="146" data-theme-id="0" data-slug-hash="PqWLog" data-default-tab="html" data-user="germanescobar" class='codepen'><pre><code>&lt;h3&gt;Hola&lt;/h3&gt;&lt;p&gt;Mundo&lt;/p&gt;</code></pre>
<p>See the Pen <a href='http://codepen.io/germanescobar/pen/PqWLog/'>PqWLog</a> by German Escobar (<a href='http://codepen.io/germanescobar'>@germanescobar</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
</div><script async src="//assets.codepen.io/assets/embed/ei.js"></script>

Los **elementos de bloque** (block elements) se caracterizan porque los navegadores los muestran en una nueva línea, y por defecto ocupan todo el ancho de la pantalla. Los elementos de bloque más usados son:

* Párrafos (`p`)
* Encabezados (`h1`, `h2`, `h3`, etc.)
* Secciones o divisiones (`div`)
* Tablas (`table`)
* Formularios (`form`)

## Elementos en línea

Veamos otro ejemplo. El siguiente código HTML tiene varios elementos en **diferentes líneas**. ¿Cómo crees que se verá el resultado?

<div data-height="200" data-theme-id="0" data-slug-hash="OVWqPe" data-default-tab="html" data-user="germanescobar" class='codepen'><pre><code>&lt;strong&gt;Estos&lt;/strong&gt; 
son 
&lt;em&gt;elementos&lt;/em&gt; 
en 
&lt;a href=&quot;/handbook&quot;&gt;línea&lt;/a&gt;
&lt;input type=&quot;text&quot;&gt;</code></pre>
<p>See the Pen <a href='http://codepen.io/germanescobar/pen/OVWqPe/'>OVWqPe</a> by German Escobar (<a href='http://codepen.io/germanescobar'>@germanescobar</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
</div><script async src="https://assets.codepen.io/assets/embed/ei.js"></script>

Los **elementos en línea** (inline elements) se caracterizan porque **los navegadores los muestran en la misma línea**, y su ancho y largo están determinado por su contenido. Algunos ejemplos de elementos en línea son:

* Links (`a`)
* Negrita (`strong`)
* Imágenes (`img`)
* Énfasis (`em`)
* Span (`span`)

## El atributo display

Es posible cambiar el comportamiento de los elementos de bloque y en línea usando el atributo `display` de CSS. Por ejemplo, la siguiente regla CSS cambia el comportamiento de todos los párrafos (un elemento de bloque) para que se comporten como elementos inline:

<div data-height="214" data-theme-id="0" data-slug-hash="RPKdbq" data-default-tab="css" data-user="germanescobar" class='codepen'><pre><code>p {
  display: inline;
}

.p1 { background: #E6D4BA; }
.p2 { background: #BACEE6; }</code></pre>
<p>See the Pen <a href='http://codepen.io/germanescobar/pen/RPKdbq/'>RPKdbq</a> by German Escobar (<a href='http://codepen.io/germanescobar'>@germanescobar</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
</div><script async src="https://assets.codepen.io/assets/embed/ei.js"></script>

De la misma forma podemos cambiar, por ejemplo, el comportamiento de todos los textos en negrita para aparezcan en una nueva línea y ocupen el ancho de la pantalla:

<div data-height="166" data-theme-id="0" data-slug-hash="NqdVvo" data-default-tab="css" data-user="germanescobar" class='codepen'><pre><code>strong {
  display: block;
  background: #ddd;
} </code> </pre>
<p>See the Pen <a href='http://codepen.io/germanescobar/pen/NqdVvo/'>NqdVvo</a> by German Escobar (<a href='http://codepen.io/germanescobar'>@germanescobar</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
</div><script async src="https://assets.codepen.io/assets/embed/ei.js"></script>

El atributo `display` puede tomar otro valores, pero los más comunes son: `inline`, `block` e `inline-block`. `inline-block` se comporta como `inline` pero respetando el ancho y el alto que le asignemos (recuerda que el ancho y el alto de `inline` está determinado por el contenido).

<div data-height="237" data-theme-id="0" data-slug-hash="NqdQZB" data-default-tab="html" data-user="germanescobar" class='codepen'><pre><code>&lt;p&gt;En esta línea, &lt;span&gt;el alto y ancho&lt;/span&gt; del span no se respeta.&lt;/p&gt;
&lt;p&gt;En esta otra, &lt;span class=&quot;respete&quot;&gt;el alto y el ancho&lt;/span&gt; si se respeta.&lt;/p&gt;</code></pre>
<p>See the Pen <a href='http://codepen.io/germanescobar/pen/NqdQZB/'>NqdQZB</a> by German Escobar (<a href='http://codepen.io/germanescobar'>@germanescobar</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
</div><script async src="//assets.codepen.io/assets/embed/ei.js"></script>

Si deseas conocer más del atributo `display`, te recomendamos que revises <a href="http://www.w3schools.com/cssref/pr_class_display.asp" target="_blank">este recurso</a>.