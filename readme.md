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

# POSITION
La propiedad position define el comportamiento de la posición de un elemento dentro de su contenedor y cómo interactua con el DOM.
Al usar esta propiedad se podrá modificar la posición y superposición de un elemento.

## PROPS
### TOP
Su valor se agrega a la parte superior del elemento.
### RIGHT
Su valor se agrega a la parte derecha del elemento.
### BOTTOM
Su valor se agrega a la parte inferior del elemento.
### LEFT
Su valor se agrega a la parte izquierda del elemento.
### Z-INDEX
Su valor establece el orden de superposición del elemento.
Se recomienda usar valores de 10 en 10 o de 100 en 100.

## VALUES
### STATIC
Este es el valor por defecto y las propiedades de posición no se aplican.

### RELATIVE
El elemento se posiciona teniendo en cuenta su posición original en el flujo del DOM y aplicando las propiedades de posición.
Por lo tanto, mantiene sus dimensiones y espacio en el DOM afectando a los demás elementos.

### ABSOLUTE
El elemento se posiciona sin tener en cuenta su posición original en el flujo del DOM pero manteniendose dentro de su contenedor.
Por lo tanto, los demás elementos pueden ocupar el espacio que originalmente ocuparia este elemento.

### FIXED
El elemento se posiciona sin tener en cuenta su posición original en el flujo del DOM ni su contenedor quedandose fijo en la pantalla en la posición establecida aún cuando el usuario haga scroll.

### STICKY
El elemento se comporta como un elemento relative hasta que se encuentre en la posición indicada en las propiedades top, bottom, left o right.
Desde ahí, se comporta como fixed permaneciendo fijo en la pantalla.
