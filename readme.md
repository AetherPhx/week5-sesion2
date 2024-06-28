# BOX MODEL
Los elementos HTML tienen un modelo de caja que define la forma y el tamaño de un elemento mediante sus atributos:
width, height, padding, margin, border.
Que en español serían el ancho, alto, relleno, borde y margen.

## WIDTH / HEIGHT
Dependiendo la configuración del box-sizing; el ancho y alto calcularán el tamaño del elemento en su totalidad o únicamente de su contenido.
Por defecto se calcula únicamente su contenido.

## CONTENT
Independientemente de la configuración del box-sizing, el contenido persé contará con su ancho y alto.

## PADDING
Es el espaciado interno del elemento y marca la distancia que se encuentra entre el borde y el contenido.
No puede ser negativo.

## BORDER
Es el borde del elemento y lo que marca el final del mismo.

## MARGIN
Es el espaciado externo del elemento y marca la distancia entre su borde y el resto de los elementos.

## ADDITIONAL
### Box Sizing
La propiedad box-sizing define cómo se calcula los tamaños de los elementos afectando así el box-model.
El valor 'content-box' calcula el tamaño del contenido y tanto el padding como borde se agregan al elemento, complicando el cálculo de todas las dimensiones del elemento.
El valor 'border-box' calcula el tamaño del elemento, por lo que incluye el contenido, padding y borde.
De esta manera se puede controlar más fácilmente el tamaño del elemento y no solo su contenido.

### '*' Selector
El selector '*'; también llamado selector universal, selecciona todos los elementos y les aplica los estilos definidos en su interior.
Su uso principal es para resetear estilos y aplicar el 'box-sizing: border-box'.

### Padding and Margin Differences
1. El padding es espaciado interno, mientras el margin es espaciado externo.
2. El margin si puede tener valores negativos y con ello lograr romper el flujo del DOM.

### Vertical Margin Collapsing
Al tener dos elementos con margenes verticales, el margen superior de uno de ellos se colapsa con el margen inferior del otro elemento.
De esta forma solo prevalece el que tiene mayor margen.