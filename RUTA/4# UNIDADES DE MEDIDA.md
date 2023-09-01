#  :symbols: UNIDADES DE MEDIDA
En CSS, hay varias unidades de medida que puedes utilizar para especificar tamaños y dimensiones de elementos en tu documento. 

## UNIDADES ABSOLUTAS
Las unidades absolutas son aquellas que mantiene su aspecto independientemente en el dispositivo en el que se encuentre.

<div  align="center" >
  
| unidad | representación |
|---|---|
| in	| `Pulgadas` (1 pulgada = 2.54 cm) |
| cm	| `Centímetros` | 
| mm	| `Milímetros` |
| pt	| `Puntos` (1 pt = 1/72 pulgadas) |
| pc	| `Picas` (1 pica = 12 puntos) |

</div>

> [!NOTE]
> Es recomendable usar unidades relativas en la medida de lo posible, ya que mejora la accesibilidad de la página web ya que permiten que los documentos se adapten fácilmente a cualquier medio.

***

## UNIDADES RELATIVAS
Las unidades relativas son aquellas que se ajustan a cada tipo de dispositivo ya que dependen de la resolución de cada pantalla.

<div  align="center" >

| unidad | representación   |
|---|---|
| px 	| `Píxeles` (relativo al dispositivo) |
| em	| `Relativo al tamaño de la fuente del elemento` ( 2 em significa 2 veces el tamaño de la fuente actual) |
| %	| `Porcentaje` (relativo al elemento padre) |
| vh y vw 	| `Medidas relativas de acuerdo al viewport` 1vh = 1% de la altura del viewport 100vh = altura del viewport |
| fr	| `Flexible Grid Units` (fr) Se utiliza en Grid Layout y representa una fracción del espacio disponible en un contenedor |

</div>

 ### `Píxeles (px)`

Es la unidad más utilizada y representa un punto en la pantalla. Se usa para tamaños fijos y proporciona control preciso sobre el diseño.

### `Porcentaje (%)`

Representa una proporción del tamaño del elemento padre. Es útil para hacer diseños fluidos y responsivos teniendo en cuenta la relación de los elementos con su contenedor padre.

### `Viewport Width (vw) y Viewport Height (vh)`

Representan un porcentaje del ancho y alto de la ventana del navegador, respectivamente. Son útiles para crear diseños responsive basados en el tamaño de la pantalla.

### `Flexible Grid Units (fr)`

Se utiliza en Grid Layout y representa una fracción del espacio disponible en un contenedor. Es útil para distribuir el espacio disponible entre elementos flexibles.

<br>
<br>












