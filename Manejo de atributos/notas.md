# DOM
- Documen Object Model.

## Realccion entre DOM y javascript
- DOM es un API que representa la estructura de nodo en forma de arbol.

## Elementos del DOM
### Objeto Window
- Variable global que representa la ventana o pestaña del navegador.
- Implementa el interfaz Window.

### Objeto Document
- Objeto inicial o punto de entrada.
- Objeto donde se carga la web, con la estructura arbórea indicada.
- Implementa la interfaz Document.

### Node
- Todo lo que cuelga del documento.

### Elements
- Los nodos pueden ser del tipo elemento.

### NodeList
- Array de elementos.
- Por ejemplo, podemos pedir todos los parrafos de una página y se retornará un array de párrafos.

### NameNodeMap
- Obtenemos los elementos en un mapa (clave-valor).

### Atributos
- Son propiedades de los elementos.
- Los más importantes son:
#### attributes
#### className
#### id
#### innerHtml
#### outerHtml
#### ariaXXXXX
#### hidden
#### dragable
#### innerText
#### style

## INTERESANTE CONSULTAR LA DOCU DE MOZZILA-DEV
https://developer.mozilla.org/es/


## Herrameintas de Chrome (f12) para desarrollar con DOM
### Panel Elements:
- Seleccionar elementos de forma visual (seleccion con click)
- Pantallazos
- Puntos de ruptura
- Exopandir/Colapsar
- Guardar elementos como variables

### Panel Console
- Interprete JS
- Ver valor de variables en un momento de la ejecución (console.log(variable))
- Depurar y acceder directamente al código que genera los mensajes de error.

### Panel Sources
- Dispone de gran variedad de herrameintas de gran utilidad

## Modificación del contenido
### innerHTML 
- Establece el contenido del elemento seleccionado.
- No incluye el elemento seleccionado.

### element.outerHTML
- Establece el contenido del elemento seleccionado.
- Incluye el elemento seleccionado.

### element.innerText
- Elementos hijos de una clase determinada

### element.draggable
- Valores booleanos
- Establece si el elemento puede ser usado para DRAG&DROP
- En otras palabras, dice al navegador si el elemento se puede arrastrar y soltar

### element.hidden
- Valores booleanos
- Muestra y oculta el valor seleccionado

### element.tabIndex = XX(intteger)
- Orden del elemento para la navegación usando el tabulador

### element.title
- Establece un mensaje que se muestra al opasar el ratón por encima

### element.id
- Modifica el identificador de manera programática de un elemento seleccionado.
- Siempre ID único (claro está). 


## Principales Propiedades y Funciones 
### element.attributes 
- NameNodeMap que recorre los atributos del elemento seleccionado

### elemento.hasAttributes()
- Retorna booleano en función de si un elemento contiene atributos

### element.hasAttribute("...")
- Reporna booleano en funciónde si un elemento contioene el atributo que se le ha pasado por parámetro

### element.getAttribute("...")
- Retorna el valor del atributo que se le ha pasado por parámetro

### element.getAttributeNames()
- Retorna un array de string con los nombres de los atributos

## Atributos Class
### element.classList
- Propiedad de solo lectura
- Retorna DOMTokenList con la lista de clases que posee un elemento

### elemento.classList.add("...", ...., "...")
- Añade una o varias clases a un elemento

### elemento.classList.remove("...", ...., "...")
- Elimina una o varias clases a un elemento

### element.classList.toggle("...")
- Añade la clase si no estña y la elimina si está

### element.classList.contains("...")
- Retorna booleano en función de si el elemento contiene clase




