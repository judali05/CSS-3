# :page_with_curl: TIPOS DE SELECTORES 
Los selectores nos ayudan a indicar el elemento que vamos a modificar. Los selectores pueden apuntar a etiquetas específicos, clases, identificadores o incluso atributos de una etiqueta. <br>
 * Existen muchos tipos de selectores y algunos de los más destacados son los siguientes.
    * <a href="#1"> SELECTOR UNIVERSAL </a>
    * <a href="#2"> SELECTOR DE ETIQUETA </a>
    * <a href="#3"> SELECTOR DE CLASE </a>
    * <a href="#4"> SELECTOR IDENTIFICADOR </a>
    * <a href="#5"> SELECTOR DESCENDIENTE </a>
    * <a href="#6"> SELECTOR DE HIJOS </a>
    * <a href="#7"> SELECTOR DE HERMANOS ADYACENTES </a>
    * <a href="#8"> COMBINACIÓN DE SELECTORES </a>

<br>

<a name="1"><h2> SELECTOR UNIVERSAL </h2></a> 
Este selector se usa cuando deseas aplicar un estilo a todos los elementos sin excepción. Es una forma rápida y sencilla de establecer que afectarán a todos los elementos en el documento.<br>
* `Sintaxis:` * { atributo: valor; }
~~~
* {
width: 0px;
 }
~~~

<br>

<a name="2"><h2> SELECTOR DE ETIQUETA </h2></a> 
El estilo se aplicará a todos las etiquetas con el mismo nombre por ejemplo la etiqueta `<h1>` .<br>
* `Sintaxis:` etiqueta { atributo: valor; }
~~~
h1 { 
  color: blue; 
}
~~~

<br>

<a name="3"><h2> SELECTOR DE CLASE </h2></a>
El estilo se aplicará a todos las clases con el mismo nombre por ejemplo  `<h1 class="titulo">` . <br>
* `Sintaxis:` .clase { atributo: valor; }
~~~
.titulo {
color: blue;
}
~~~

<br>

<a name="4"><h2> SELECTOR IDENTIFICADOR </h2></a>
El estilo se aplicará a todos los valores ID con el mismo nombre por ejemplo `<p id="texto"> ` . <br> 
* `Sintaxis:` #id { atributo: valor; }
~~~
#text {
color: blue;
}
~~~

<br>

<a name="5"><h2> SELECTOR DESCENDIENTE </h2></a>
El estilo se aplicará a todas las etiquetas que esten entre las etiquetas de apertura y de cierre del elemeto hijo con el mismo nombre por ejemplo <br>
`<di> <h2></h2> </div>` .<br><br>
* `Sintaxis:` etiqueta_padre etiqueta_hijo { atributo: valor; }
~~~
div h2 {
  color: blue;
}
~~~

<br>

<a name="6"><h2> SELECTOR DE HIJOS </h2></a>
El estilo se aplicará a las etiquetas hijo que esten entre las etiquetas de apertura y de cierre del elemeto padre con el mismo nombre por ejemplo <br>
`<di> <span> <span></spam> </spam> </div>` .<br><br>
* `Sintaxis:` etiqueta_padre > etiqueta_hijo { atributo: valor; }
~~~
div > span {
  color: blue;
}
~~~

<br>

<a name="7"><h2> SELECTOR DE HERMANOS ADYACENTES </h2></a>
El estilo se aplicará a todos los primeros hermanos de una etiqueta que vengan inmediatamente después de otra etiqueta por ejemplo: <br>
`<h1></h1> <p></p>` .<br><br>
* `Sintaxis:` etiqueta_1 + etiqueta_2 { atributo: valor; }
~~~
h1 + p {
 color: blue;
}
~~~

<br>

<a name="8"><h2> COMBINACIÓN DE SELECTORES </h2></a>
El estilo se aplicará a todos las etiquetas que esten en el selector por ejemplo la etiqueta `<h1>`, `<p>`, `<span>` .<br>
* `Sintaxis:` etiqueta_1, eqtiqueta_2, etiqueta_3 { atributo: valor; }
~~~
h1, p, span { 
  color: blue; 
}
~~~
<br>
<br>
