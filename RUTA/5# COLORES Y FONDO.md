#  :art: COLORES Y FONDOS

Los valores de los colores se pueden definir mediante su nombre, en código hexadecimal (#RRGGBBAA) o mediante sus valores en los siguientes formatos:

## POR SU NOMBRE
Recuerda que una forma de añadir color a un elemento es utilizando el nombre del color en inglés, como black ( negro ), cyan ( cian ) o yellow ( amarillo ).
<br>
<br>

***

## MODELOS
Hay dos modelos principales de colores: el modelo aditivo RGB (rojo, verde, azul) utilizado en dispositivos electrónicos, y el modelo sustractivo CMYK (cian, magenta, amarillo, negro) utilizado para impresión.
<br>
<br>

***

## RGB 
viene del significa ( Red, Green, Blue ) en español ( Rojo, Verde, Azul ) Cada valor rojo, verde y azul es un número de 0 a 255, 0 significa que hay 0% de ese color, y es negro. 255 significa que hay 100% de ese color.   
<br>
<div align="center">
  
### `rgb (255, 0 ,0)`

</div>
<br>
En el modelo de color aditivo RGB, los colores primarios son colores que, al combinarse, crean blanco puro. Pero para que esto suceda, cada color debe estar en su máxima intensidad de 255 `(255,255,255)` y para generar negro todos los colores debe estar en 0 `(0,0,0)` , con estos se pueden hacer variaciones para tener colores secundario y la diferente variedad de colores.
<br>
<div  align="center" >
<img src="https://github.com/judali05/CSS-3/assets/129390687/2dbb861b-4303-47a3-94fe-db3c93cf5214" style=" width: 600px;" >
</div>
<br>
<br>

***

## HEXADECIMALES
Es práctica muy común aplicar color a un elemento CSS con valores hexadecimales (hex). Puede sonar complicado, pero no es más que otra forma de expresar colores RGB.

<br>

Los valores hexadecimales empiezan con el carácter  `#` , siguiendo seis caracteres entre  `0-9` y  `A-F` . El primer par de caracteres representa el rojo, el segundo el verde y el tercero el azul. Por ejemplo:
<br>
<div align="center">
  
### `#4B5320`

</div>
<br>
Seguramente estés familiarizado con valores en base 10, o decimales, los cuales van de 0 a 9. Hexadecimales, o valores en base 16, van de 0 a 9 y a continuación de A a F:
<br>
<div align="center">
  
### `0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F`

</div>
<br>
Para los colores en hexadecimal, 00 es 0% de ese color, y FF es 100%. De tal manera que #00FF00 se traduce en 0% rojo, 100% verde y 0% azul, siendo equivalente a rgb(0, 255, 0).
<br>
<br>

***

## HSL
Otra forma de representar colores es el modelo HSL, siglas de hue, saturation y lightness (matiz, saturación y luminosidad).
La función CSS hsl acepta 3 valores: un número de 0 a 360 para el tono, un porcentaje de 0 a 100 para la saturación y un porcentaje de 0 a 100 para la luminosidad. 

<br>

Sobre un círculo cromático, el matiz (hue) rojo está en 0 grados, el verde en 120 y el azul en 240.
La saturación es la intensidad de un color desde 0%, o gris, hasta 100% para color puro. Debes agregar el signo de porcentaje % tanto para los valores de saturación como para los valores de luminosidad.
<br>
<div align="center">

### `hsl (0, 100%, 50%)`

</div>
<br>
La luminosidad (lightness) es lo brillante que parece un color, desde 0% o completamente negro, hasta 100%, completamente blanco, siendo neutro el 50%.
<br>
<br>

***

## GRADUACIONES DE COLORES
Hemos visto unas cuantas maneras de establecer colores planos en CSS, pero también se pueden aplicar transiciones de color, o gradientes, sobre un elemento.

<br>

Se llama gradiente, o degradado, a la transición progresiva de un color a otro. La función CSS linear-gradient permite controlar la dirección de la transición a lo largo de una línea, y qué colores participan en el degradado.

<br>

Una cosa a tener en cuenta es que la función linear-gradient lo que en realidad crea es un elemento image, y se asocia normalmente con la propiedad background, la cual puede aceptar una imagen como valor.

<br>
La función linear-gradient es muy flexible, aqui la sintaxis básica para usarla:
<br>
<div aling="center">
  
### `linear-gradient (gradientDirection, color1, color2, ...);`

</div>
<br>

gradientDirection es la dirección de la línea a lo largo de la cual tendrá lugar la transición. color1 y color2 son argumentos de color, representando los colores usados en la transición. Se pueden pasar a la función en cualquier formato, ya sea el nombre del color, hex, rgb o hsl.

<br>
Las paradas de color permiten afinar el emplazamiento de los colores a lo largo de la línea que sigue el gradiente. Se definen, en la función linear-gradient, mediante unidades de longitud, como px o porcentajes, a continuación del color del cual se quiere definir la parada.

<br>
Por ejemplo, en el gradiente que sigue, la transición del rojo al negro tiene lugar en el punto que representa el 90% de la línea del gradiente, de manera que el rojo ocupa la mayor parte del espacio disponible:
<br>
<div align="center">

### `linear-gradient (90deg, red 90%, black);`

</div>
<br>

> [!IMPORTANT]
>Si en la función linear-gradient no se especifica el argumento gradientDirection, por defecto será de 180 grados, disponiendo los colores de arriba a abajo.

<br>
<br>

***





## RGBA
Este agrega una A de Alpha, este representa el grado de transparencia u opacidad del color, este se coloca al final de los colores ( Rojo, Verde, Azul, opacidad ) El canal de opacidad se expresa mediante un valor entre cero y uno, siendo 0 totalmente transparente y 1 totalmente opaco. Todos los valores decimales entre el cero y el 1 expresan distintos grados de opacidad.

<br>
<br>
