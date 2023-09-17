#  :art: COLORES Y FONDOS
Los valores de los colores se pueden definir mediante su nombre, en código hexadecimal (#RRGGBBAA) o mediante sus valores en los siguientes formatos:

   * <a href="#1"> POR SU NOMBRE </a>
   * <a href="#2"> MODELOS </a>
       * <a href="#3"> RGB </a>
       * <a href="#4"> HEXADECIMALES </a>
       * <a href="#5"> HSL </a>
   * <a href="#6"> GRADUACIONES DE COLORES </a>
   * <a href="#7"> OPACIDAD </a>
       * <a href="#8"> ALPHA </a>
   * <a href="#9"> FONDO </a>


<br>

<a name="1"><h2> POR SU NOMBRE </h2></a>
* Recuerda que una forma de añadir color a un elemento es utilizando el nombre del color en inglés, como black ( negro ), cyan ( cian ) o yellow ( amarillo ).
  
<br>

<a name="2"><h2> MODELOS </h2></a>
* Hay dos modelos principales de colores: el modelo aditivo RGB (rojo, verde, azul) utilizado en dispositivos electrónicos, y el modelo sustractivo CMYK (cian, magenta, amarillo, negro) utilizado para impresión.
  
<br>

<a name="3"><h2> RGB </h2></a> 
* viene del significa ( Red, Green, Blue ) en español ( Rojo, Verde, Azul ) Cada valor rojo, verde y azul es un número de 0 a 255, 0 significa que hay 0% de ese color, y es negro. 255 significa que hay 100% de ese color.   

<br>

<div align="center">
  
### `rgb (255, 0 ,0)`

</div>

<br>

* En el modelo de color aditivo RGB, los colores primarios son colores que, al combinarse, crean blanco puro. Pero para que esto suceda, cada color debe estar en su máxima intensidad de 255 `(255,255,255)` y para generar negro todos los colores debe estar en 0 `(0,0,0)` , con estos se pueden hacer variaciones para tener colores secundario y la diferente variedad de colores.
  
<br>

<div  align="center" >
<img src="https://github.com/judali05/CSS-3/assets/129390687/2dbb861b-4303-47a3-94fe-db3c93cf5214" style=" width: 600px;" >
</div>

<br>

<a name="4"><h2> HEXADECIMALES </h2></a> 
* Es práctica muy común aplicar color a un elemento CSS con valores hexadecimales (hex). Puede sonar complicado, pero no es más que otra forma de expresar colores RGB.

<br>

* Los valores hexadecimales empiezan con el carácter  `#` , siguiendo seis caracteres entre  `0-9` y  `A-F` . El primer par de caracteres representa el rojo, el segundo el verde y el tercero el azul. Por ejemplo:
  
<br>

<div align="center">
  
### `#4B5320`

</div>

<br>

* Seguramente estés familiarizado con valores en base 10, o decimales, los cuales van de 0 a 9. Hexadecimales, o valores en base 16, van de 0 a 9 y a continuación de A a F:
  
<br>

<div align="center">
  
### `0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F`

</div>

<br>

* Para los colores en hexadecimal, 00 es 0% de ese color, y FF es 100%. De tal manera que #00FF00 se traduce en 0% rojo, 100% verde y 0% azul, siendo equivalente a rgb(0, 255, 0).

<br>

<a name="5"><h2> HSL </h2></a> 
* Otra forma de representar colores es el modelo HSL, siglas de hue, saturation y lightness (matiz, saturación y luminosidad).
La función CSS hsl acepta 3 valores: un número de 0 a 360 para el tono, un porcentaje de 0 a 100 para la saturación y un porcentaje de 0 a 100 para la luminosidad. 

<br>

* Sobre un círculo cromático, el matiz (hue) rojo está en 0 grados, el verde en 120 y el azul en 240.
La saturación es la intensidad de un color desde 0%, o gris, hasta 100% para color puro. Debes agregar el signo de porcentaje % tanto para los valores de saturación como para los valores de luminosidad.

<br>

<div align="center">

### `hsl (0, 100%, 50%)`

</div>

<br>

* La luminosidad (lightness) es lo brillante que parece un color, desde 0% o completamente negro, hasta 100%, completamente blanco, siendo neutro el 50%.
  
<br>

<a name="6"><h2> GRADUACIONES DE COLORES </h2></a>
* Hemos visto unas cuantas maneras de establecer colores planos en CSS, pero también se pueden aplicar transiciones de color, o gradientes, sobre un elemento.

<br>

* Se llama gradiente, o degradado, a la transición progresiva de un color a otro. La función CSS linear-gradient permite controlar la dirección de la transición a lo largo de una línea, y qué colores participan en el degradado.

<br>

* Una cosa a tener en cuenta es que la función linear-gradient lo que en realidad crea es un elemento image, y se asocia normalmente con la propiedad background, la cual puede aceptar una imagen como valor.

<br>

* La función linear-gradient es muy flexible, aqui la sintaxis básica para usarla:
  
<br>
<div aling="center">
  
### `linear-gradient (gradientDirection, color1, color2, ...);`

</div>
<br>

* gradientDirection es la dirección de la línea a lo largo de la cual tendrá lugar la transición. color1 y color2 son argumentos de color, representando los colores usados en la transición. Se pueden pasar a la función en cualquier formato, ya sea el nombre del color, hex, rgb o hsl.

<br>

* Las paradas de color permiten afinar el emplazamiento de los colores a lo largo de la línea que sigue el gradiente. Se definen, en la función linear-gradient, mediante unidades de longitud, como px o porcentajes, a continuación del color del cual se quiere definir la parada.

<br>

* Por ejemplo, en el gradiente que sigue, la transición del rojo al negro tiene lugar en el punto que representa el 90% de la línea del gradiente, de manera que el rojo ocupa la mayor parte del espacio disponible:
  
<br>

<div align="center">

### `linear-gradient (90deg, red, 90%, black);`

</div>

<br>

> [!IMPORTANT]
>Si en la función linear-gradient no se especifica el argumento gradientDirection, por defecto será de 180 grados, disponiendo los colores de arriba a abajo.

<br>

<a name="7"><h2> OPACIDAD </h2></a>
* Opacity describe cuán opaco o no transparente es algo. Por ejemplo, una pared sólida es opaca y no puede pasar la luz. Pero un vaso para beber es mucho más transparente, y puedes ver a través del vaso hacia el otro lado.

<br>

* Con la propiedad CSS opacity, puede controlar cuán opaco o transparente es un elemento. Con el valor 0, o 0%, el elemento será completamente transparente, y en 1.0, o 100%, el elemento será completamente opaco como lo es por defecto.
  
<br>

<div align="center">

`opacity: 0.5;`

</div>

<br>

<a name="8"><h2> ALPHA </h2></a>
* Otra forma de establecer la opacidad de un elemento es con el canal alpha. Similar a la propiedad opacity, el canal alfa controla qué tan transparente u opaco es un color.

<br>

* Ya has establecido la opacidad de la carátula con un color con nombre y la propiedad opacity, pero puedes agregar un canal alfa a las otras propiedades de color CSS.

<br>

* Ya está familiarizado con el uso de la función rgb para establecer colores. Para agregar un canal alfa a un color rgb, use la función rgba en su lugar.

<br>

* La función rgba funciona igual que la función rgb, pero toma un número más de 0 a 1.0 para el canal alfa:
  
<br>

<div align="center">

### `rgba (rojo, verde, azul, alfa) = rgba (255 ,0 ,0 ,0,5)`

</div>

<br>

* También puedes utilizar un canal alfa con colores hsl. Para agregar un canal alfa a un color hsl, use la función hsla en su lugar.

<br>

<div align="center">

### `hsla (matiz, saturación y luminosidad, alfa) = hsla (0, 100%, 50%, 0,5)`

</div>

<br>

* También puedes utilizar un canal alfa con colores hsl y hexadecimal. Para agregar un canal alfa a un color hex, se hace d la misma forma solo que se agrega un campo de mas al final no queda de 6 sino de 8 caracteres.

<br>

<div align="center">

### `hex (rojo, verde, azul, alfa) = #FF0000CC `

</div>

<br>

<a name="9"><h2> FONDO </h2></a>
* Algunas de las propiedades relacionadas con el color y el fondo más utilizadas son las siguientes:

<br>

<div align="center">
  
| Propiedad	| Descripción |
|---|---|
|`color`	|Color del texto |
|`background-color`	|Color de fondo |
|`background-image`	|Imagen de fondo |
|`background-repeat`	|Repetición de la imagen de fondo |
|`background-attachment`	|Desplazamiento de la imagen de fondo |
|`background-position`	|Posición de la imagen de fondo |
|`background-size`	|Tamaño de la imagen de fondo |
|`Opacity`	|Transparencia de un elemento |

</div>

<br>
<br>
