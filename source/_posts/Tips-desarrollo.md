---
title: Sistema de filas y columnas de Bootstrap3 con ejemplos
date: 2018-09-09 15:24:47
tags:
---
{% img center-block https://www.codejobs.com/media/321c90743897052.png %}
{% blockquote %}
<p>Hola chicos, espero se encuentren de lo mejor, el día de hoy quiero dejarles esta publicación sobre el sistema de filas y columnas de Bootstrap versión 3 con ejemplos.</p> 
<p>Si vamos a la documentación de Bootstrap, nos dirá que tenemos una rejilla con 12 columnas (siempre son 12 columnas ojo aquí) y estas columnas las podemos optimizar para cada una de las distintas resoluciones de nuestras pantallas (desktop, celulares, etc.). Ver aquí la documentación oficial de Bootstrap.</p>
<br>
<h3>A continuación la rejilla de columnas que maneja Bootstrap:</h3>
{% endblockquote %}
{% img center-block https://www.codejobs.com/media/8768a34f9e0a5a0.png %}

{% blockquote %}
<h3>La resoluciones que maneja Bootstrap son:</h3>
{% endblockquote %}
{% img center-block https://www.codejobs.com/media/8e28a32e6039748.png %}

{% blockquote %}
<h3>Ahora, vamos a ver cómo usarlo:</h3>
<p>Lo primero que hice fue descargar bootstrap.min.css y añadirlo en mi  head del HTML5. </p>
<pre class="hljs"><code class="html"><span class="hljs-tag">&lt;<span class="hljs-name">head</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">title</span>&gt;</span>Sistema de filas y columnas de Bootstrap 3 <span class="hljs-tag">&lt;/<span class="hljs-name">title</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">meta</span> <span class="hljs-attr">charset</span>=<span class="hljs-string">"UTF-8"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text/css"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"style.css"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text/css"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"bootstrap.min.css"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">head</span>&gt;</span>
</code></pre>
<h3>Clase .col-lg-numerocolumnas</h3>
<p>Ahora bien en el caso de la clase de bootstrap .col-lg-numerocolumnas; nos dice que si la resolución de mi pantalla es mayor o igual  a 1200px el comportamiento de las columnas será horizontal  y si la resolución es menor a 1200px entonces el comportamiento de las columnas será de forma vertical (apiladas), veamos el siguiente ejemplo:</p>
<pre class="hljs"><code class="html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-lg-2"</span>&gt;</span>.col-lg-2<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-lg-10"</span>&gt;</span>.col-lg-10<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
{% endblockquote %}

{% blockquote %}
<h3>Resolución >= 1200px comportamiento de las columnas en horizontal</h3>
<p>En la siguiente imágen tengo la resolución de 1201px es por eso que mis columnas son horizontales:</p>
{% endblockquote %}
{% img img-responsive https://www.codejobs.com/media/0d1637f9a3579cc.png %}

{% blockquote %}
<h3>En la siguiente imágen tengo  la resolución de 1199px es por eso que mis columnas son verticales:</h3>
{% endblockquote %}
{% img img-responsive https://www.codejobs.com/media/e42c9a2188d574b.png %}

{% blockquote %}
<p><strong>Nota:</strong> Aunque las columnas se coloquen en forma vertical esto NO quiere decir que se ha creado otra fila, es decir, las columnas se apilan pero dentro de la misma fila, a continuación te pongo en color “rosa fuerte” la fila.</p>
<p>Columnas en forma vertical dentro de la misma fila:</p>
{% endblockquote %}
{% img img-responsive https://www.codejobs.com/media/7ff20084154f934.png %}

{% blockquote %}
<p>En general bootstrap implementa medias queries que afectan las columnas cuando la resolución de la pantalla tiene cierta medida de pixeles.</p>
<br>
<h3>Clase .col-md-numerocolumnas</h3>
<p>Para el caso de md(tamaños medianos) nos dice que las columnas se van a comportar de forma horizontal si la resolucion es >=992px y de manera vertical si la resolucion es menor a 992px, veamos el siguiente ejemplo:</p>
<pre class="hljs"><code class="html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-md-7"</span>&gt;</span>.col-md-7<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-md-5"</span>&gt;</span>.col-md-4<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
{% endblockquote %}

{% blockquote %}
<p>En la siguiente imágen tengo la resolución de 992px es por eso que mis columnas son horizontales:</p>  
{% endblockquote %}
{% img img-responsive https://www.codejobs.com/media/0434a563461a7e9.png %}

{% blockquote %}
<p>En la siguiente imágen tengo  la resolución de 991px es por eso que mis columnas son verticales:</p>
{% endblockquote %}
{% img img-responsive https://www.codejobs.com/media/a4372719108d52d.png %}

{% blockquote %}
<h3>Clase .col-sm-numerocolumnas</h3>
<p>Para el caso de sm(small - tamaños pequeños) nos dice que las columnas se van a comportar de forma horizontal si la resolucion es >=768 px y de manera vertical si la resolucion es menor a 768px, veamos el siguiente ejemplo:</p>
<pre class="hljs"><code class="html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-sm-9"</span>&gt;</span>.col-sm-9<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-sm-3"</span>&gt;</span>.col-sm-3<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    
{% endblockquote %}

{% blockquote %}
<p>En la siguiente imágen tengo la resolución de 768px es por eso que mis columnas son horizontales:</p>
{% endblockquote %}
{% img center-block https://www.codejobs.com/media/5d24a3d37de476d.png %}

{% blockquote %}
<p>En la siguiente imágen tengo  la resolución de 767px es por eso que mis columnas son verticales:</p>
{% endblockquote %}
{% img center-block https://www.codejobs.com/media/81755a2845e3942.png %}

{% blockquote %}
<h3>Clase .col-xs-numerocolumnas</h3>
<p>Para el caso de xs(extra pequeño) por más pequeña que sea la resolución mis columnas nunca van a cambiar, es decir siempre se comportarán de manera horizontal.</p>
<pre class="hljs"><code class="html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-xs-8"</span>&gt;</span>.col-xs-8<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-xs-4"</span>&gt;</span>.col-xs-4<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
{% endblockquote %}
{% img center-block  https://www.codejobs.com/media/f96014270447e18.png %}

{% blockquote %}
<h3>Código completo del ejemplo:</h3>
<p>HTML</p>
<pre class="hljs"><code class="html"><span class="hljs-meta">&lt;!DOCTYPE html&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">html</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">head</span>&gt;</span>
	<span class="hljs-tag">&lt;<span class="hljs-name">title</span>&gt;</span>Sistema de filas y columnas de Bootstrap 3 <span class="hljs-tag">&lt;/<span class="hljs-name">title</span>&gt;</span>
	<span class="hljs-tag">&lt;<span class="hljs-name">meta</span> <span class="hljs-attr">charset</span>=<span class="hljs-string">"UTF-8"</span>&gt;</span>
	<span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text/css"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"style.css"</span>&gt;</span>
	<span class="hljs-tag">&lt;<span class="hljs-name">link</span> <span class="hljs-attr">rel</span>=<span class="hljs-string">"stylesheet"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text/css"</span> <span class="hljs-attr">href</span>=<span class="hljs-string">"bootstrap.min.css"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">head</span>&gt;</span>
	<span class="hljs-tag">&lt;<span class="hljs-name">body</span>&gt;</span>
		<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"lg"</span>&gt;</span>Tamaño lg (large) <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
		<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-lg-2"</span>&gt;</span>.col-lg-2<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-lg-10"</span>&gt;</span>.col-lg-10<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
		<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

		<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"md"</span>&gt;</span>Tamaño md (mediano)<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
		<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-md-7"</span>&gt;</span>.col-md-7<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-md-5"</span>&gt;</span>.col-md-4<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
		<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

		<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"sm"</span>&gt;</span>Tamaño sm (small - pequeño)<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
		<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-sm-9"</span>&gt;</span>.col-sm-9<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-sm-3"</span>&gt;</span>.col-sm-3<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
		<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

		<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"xs"</span>&gt;</span>Tamaño xs (extra small - extra pequeño)<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
		<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"row"</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-xs-8"</span>&gt;</span>.col-xs-8<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"col-xs-4"</span>&gt;</span>.col-xs-4<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
		<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
	<span class="hljs-tag">&lt;/<span class="hljs-name">body</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">html</span>&gt;</span>
</code></pre>
<p>CSS</p>
<pre class="hljs"><code class="css"><span class="hljs-selector-class">.lg</span> {
	<span class="hljs-attribute">color</span>: <span class="hljs-number">#3333FF</span>;
	<span class="hljs-attribute">font-weight</span>: <span class="hljs-number">700</span>;
}

<span class="hljs-selector-class">.md</span> {
	<span class="hljs-attribute">color</span>: red;
	<span class="hljs-attribute">font-weight</span>: <span class="hljs-number">700</span>;
	<span class="hljs-attribute">margin-top</span>: <span class="hljs-number">20px</span>;
}

<span class="hljs-selector-class">.sm</span> {
	<span class="hljs-attribute">color</span>: green;
	<span class="hljs-attribute">font-weight</span>: <span class="hljs-number">700</span>;
	<span class="hljs-attribute">margin-top</span>: <span class="hljs-number">60px</span>;	
}

<span class="hljs-selector-class">.xs</span> {
	<span class="hljs-attribute">color</span>: purple;
	<span class="hljs-attribute">font-weight</span>: <span class="hljs-number">700</span>;
	<span class="hljs-attribute">margin-top</span>: <span class="hljs-number">90px</span>;	
}

<span class="hljs-selector-class">.col-lg-1</span>,
<span class="hljs-selector-class">.col-lg-2</span>,
<span class="hljs-selector-class">.col-lg-3</span>,
<span class="hljs-selector-class">.col-lg-4</span>, 
<span class="hljs-selector-class">.col-lg-5</span>, 
<span class="hljs-selector-class">.col-lg-6</span>, 
<span class="hljs-selector-class">.col-lg-7</span>,
<span class="hljs-selector-class">.col-lg-8</span>,
<span class="hljs-selector-class">.col-lg-9</span>,
<span class="hljs-selector-class">.col-lg-10</span>,
<span class="hljs-selector-class">.col-lg-11</span>,
<span class="hljs-selector-class">.col-lg-12</span> {
	<span class="hljs-attribute">border</span>: <span class="hljs-number">1px</span> solid <span class="hljs-number">#3333FF</span>;
}

<span class="hljs-selector-class">.col-md-1</span>,
<span class="hljs-selector-class">.col-md-2</span>,
<span class="hljs-selector-class">.col-md-3</span>,
<span class="hljs-selector-class">.col-md-4</span>, 
<span class="hljs-selector-class">.col-md-5</span>, 
<span class="hljs-selector-class">.col-md-6</span>, 
<span class="hljs-selector-class">.col-md-7</span>,
<span class="hljs-selector-class">.col-md-8</span>,
<span class="hljs-selector-class">.col-md-9</span>,
<span class="hljs-selector-class">.col-md-10</span>,
<span class="hljs-selector-class">.col-md-11</span>,
<span class="hljs-selector-class">.col-md-12</span> {
	<span class="hljs-attribute">border</span>: <span class="hljs-number">1px</span> solid red;
}

<span class="hljs-selector-class">.col-sm-1</span>,
<span class="hljs-selector-class">.col-sm-2</span>,
<span class="hljs-selector-class">.col-sm-3</span>,
<span class="hljs-selector-class">.col-sm-4</span>, 
<span class="hljs-selector-class">.col-sm-5</span>, 
<span class="hljs-selector-class">.col-sm-6</span>, 
<span class="hljs-selector-class">.col-sm-7</span>,
<span class="hljs-selector-class">.col-sm-8</span>,
<span class="hljs-selector-class">.col-sm-9</span>,
<span class="hljs-selector-class">.col-sm-10</span>,
<span class="hljs-selector-class">.col-sm-11</span>,
<span class="hljs-selector-class">.col-sm-12</span> {
	<span class="hljs-attribute">border</span>: <span class="hljs-number">1px</span> solid green;
}

<span class="hljs-selector-class">.col-xs-1</span>,
<span class="hljs-selector-class">.col-xs-2</span>,
<span class="hljs-selector-class">.col-xs-3</span>,
<span class="hljs-selector-class">.col-xs-4</span>, 
<span class="hljs-selector-class">.col-xs-5</span>, 
<span class="hljs-selector-class">.col-xs-6</span>, 
<span class="hljs-selector-class">.col-xs-7</span>,
<span class="hljs-selector-class">.col-xs-8</span>,
<span class="hljs-selector-class">.col-xs-9</span>,
<span class="hljs-selector-class">.col-xs-10</span>,
<span class="hljs-selector-class">.col-xs-11</span>,
<span class="hljs-selector-class">.col-xs-12</span> {
	<span class="hljs-attribute">border</span>: <span class="hljs-number">1px</span> solid purple;
}
</code></pre>
<p>ESTRUCTURA</p>
{% endblockquote %}
{% img center-block https://www.codejobs.com/media/2e207c1e203d04c.png %}

{% blockquote %}
<p>Espero que esta información les haya servido, Bye.</p>
<p>Fuente:<a href="https://www.codejobs.com/es/blog/2015/12/01/sistema-de-filas-y-columnas-de-bootstrap3-con-ejemplos"> Codejobs</a></p>

<div class="form-group">
  <label for="comment">Comentarios:</label>
  <textarea class="form-control" rows="5" id="comment"></textarea>
  <button type="button" class="btn btn-primary">Enviar</button>
</div>
{% endblockquote %}

