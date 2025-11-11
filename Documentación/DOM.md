
## **Selectores**
- `document.getElementById('id');` Obtiene un elemento por su id
- `document.getElementByClassName('clase');` Devuelve un array de elementos
- `document.getElementByName(h1);` Devuelve un array de elementos

## **Query selector**
- `document.querySelector('[type = "number"]');` Selecciona un elemento a partir de un atributo. (Devuelve un array).
	- `querySelector('#id');` Devuelve un elemento por su id
	- `querySelector('.clase');` Devuelve un elemento por su clase
	- `querySelector('[type = "text"]');` Devuelve un elemento por su atributo

## **Acceso a nodos**
- `docuemnt.body.childNodes;` Accede a los hijos de la etiqueta
- `documemt.body.firstElementChild;` Devuelve el primer elemento hijo
- `documemt.body.lastElementChild;` Devuelve el último elemento hijo
- `elemento.previusElementSibling;` Devuelve el elemento hermano anterior
- `nextElementSibling;` Devuelve el siguiente elemento hermano
- `div.parentNode;` Accede al nodo padre de un elemento
- `elemento.outerHTML;` Devuelve todo lo que esté al nivel del elemento
- ``

## **Atributos**
- `elemento.getAttribute("href");` Obtiene el atributo de un elemento
- `elemento.setAttribute('atributo', 'valor');` Asigna un atributo a un elemento
- `elemento.hasAttribute('atributo');` Comprueba si un elemento contiene el atributo especificado
- `elemento.removeAttribute("atributo");` Elimina un atributo de un elemento

## **Clases e Id**
- `elemento.className = "clase";` Agrega una clase al elemento eliminando las demás
- `elemento.id = "id1";` Agrega un id a un elemento

## **Estilos**
- `elemento.style.background = 'black';` Modifica o agrega estilos a los elementos
- `elemento.style.color = 'white';`
- `document.documentElement.style.color = 'white';` Modifica el estilo de todos los elementos a la vez

## **Creación de elementos**
- `const divElement = createElement('div');` Crea un elemento nuevo
- `divElement.setAttribute('class', 'clase1');` Agrega una clase al elemento creado
- `body.appen(divElement);` Agrega el elemento creado al elemento especificado

## **Contenido de las etiquetas**
- `textContent` Permite obtener o modificar el texto contenido en un elemento HTML
	- `h1.textContent;` Obtiene el contenido del elemento h1
	- `h1.textContent = "Nuevo texto";` Modifica el texto contenido dentro del elemento
- `innerHTML` Permite modificar el contenido HTML de un elemento
	- `div.innerHTML;` Devuelve el contenido HTML del elemento
	- `div.innerHTML = '<h2> Contenido del elemento </h2>'` Agrega el contenido al elemento
- Ambos se pueden concatenar con su contenido actual con `+=`

## **Eventos**
- Son acciones que se realizarán cuando se desencadene el evento sobre el elemento:
```
  elemento.addEventListener('evento', function(){
	  //Accion a realizar cuando se produzca el evento
  })
  ```
- `onevento = "alert('Texto a mostrar en la alerta')"` En el documento HTML dentro de una etiqueta de elemento.
- `promt('Texto a mostrar');` Permite introducir contenido a través de una alerta
- `elemento.onclick = funcion;` Evitar poner paréntesis para que la función no se ejecute sin que se produzca el evento (click)
- `elemento.onclick = null;` desactiva el evento