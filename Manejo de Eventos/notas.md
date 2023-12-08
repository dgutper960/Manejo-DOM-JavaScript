# En este apartado veremos los diferentes tipos de eventos

## Eventos Generales
- Todos los elementos responden a estos eventos

## Especificos
- Reponderán ciertos elementos de la página

## Dependiendo de quien los genera
### Eventos de ratón
- Revisar la lista de eventos principales

### Eventos de taclado
- Revisar la lista de eventos principales

### Eventos de formulario
- Revisar la lista de eventos principales

### Eventos de navegador
- Revisar la lista de eventos principales

### Loop de eventos de JS
- Para evitar el colapso del navegador se genera una pila de CallBackQueue que permite la concurrencia
- La pila Call Stack junto a CallBack Queue, permiten la ejecución asincrona con un solo hilo

## Formas de propagar eventos
### Bubbling
- El evento se propaga de los nodos hijos a los nodos padres
- Propagación por defecto

### Capturing
- El evento se propaga de los nodos padre a los nodos hijos

## Formas de capturar un evento
### inline -> Desde el html
- No recomendado
- Menos eficiente respecto al mantenimiento

### Con propiedades propias

### addEventListener
- La opción más recomendada
- Funcion que tiene como entrada el evento y la funcion a la que se llama
- Previamente se captura el elemento con getElementById
- elemento.addEventListener(evento, funcion);
- Se puede borrar el manejador previamente añadidio con -> removeEventListener()

## Propiedades del objeto Evento
### .bubbles 
- Si es un bubbling event

### .preventDefault()
- Evita el comportamiento por defecto

### .stopPropagation()
- Detiene la propagación

### .stopImmediatePropgation()
- Detiene además los eventos que puedan estar capturando dicho evento

### .target / .currentTarget
- Elemento que lanzó el evento / cuyos manejadores lanzaron el evento

### .pageX / .pageY
- Posición X/Y dónde se produjo el evento

## Eventos Sintéticos
- Son eventos creados por del desarrollador, en contra de los eventos del navegador


