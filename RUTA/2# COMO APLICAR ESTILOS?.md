# COMO APLICAR ESTILOS :pencil:
Hay tres formas de aplicar estilos CSS estos son en línea en una etiqueta HTML, incrustado en la cabecera de un doucmento HTML o mediante hojas de estilo externas.

## CSS EN LÍNEA:
Estas declaraciones CSS están incrustadas en las etiquetas HTML por medio del atributo  `style`.

~~~
<h1 style="color:blue">Hola Mundo</p>
~~~

> [!NOTE]
> El CSS en línea es complicado de entender y mantener ya que mezcla los estilos CSS con el código HTML.

<br>

***

## CSS INCRUSTADO EN LA CABECERA:
En este caso el estilo se agrega dentro de la etiqueta `<head>`  con la etiqueta `<style>` en un documento HTML.

~~~
<html>
<head>
    <style> p { color: blue; } </style>
</head> 
<body>
     <p>Hola Mundo</p>
</body> 
</html>
~~~

> [!NOTE]
> La desventaja de este método es que, a la hora de realizar cualquier cambio, se debe realizar en múltiples documentos diferentes y el código puede estar repetido.

<br>

***

## CSS EN HOJAS DE ESTILO EXTERNA:
Las hojas de estilo externas se crean de la siguiente forma el archivo de estilos debe contar con la extensión .css y se referencia desde HTML mediante el elemento `<link>` en la cabecera del documento HTML. 

Index.html
~~~
<html>
<head>
    <link rel="stylesheet" href="styles.css">
</head> 
<body>
     <p>Hola Mundo</p>
</body> 
</html>

~~~

Style.css
~~~
p { 
  color: blue; 
}
~~~

> [!NOTE]
> Este es el método más eficiente y más sencillo de mantener ya que el código CSS se encuentra separado del fichero HTML.



