## **Utilización**
- Dentro de un documento con extensión .css
```
<h1> Titulo de la página </h1>
<p> Texto del párrafo </p>

p {color: white;}

p, h1{
	font-size: large;
}
```
- Dentro de la etiqueta HTML
```
<p style="color: red"> Texto de color rojo </p>
```

## **Tipos de selectores**

- Etiquetas
	- `body, h1, div`
- Id
	- `#titulo`
- Clases
	- `.parrafo`

Se pueden agregar varias clases a un mismo elemento HTML colocando un espacio entre clase y clase.

```
//html
<p class="texto especial"> Texto con dos clases </p>

//css
p.texto{color: white;}

p.especial {color: blue;}
```
   
## **Selectores de css**

- Se pueden seleccionar elementos específicos que se encuentren dentro de otros elementos

```
div p { color: gray; }
```
- Todos los elementos `<p>` que se encentren dentro del div recibirán ese estilo.
- Para seleccionar varios elementos podemos declararlos separados por `,` . 
```
div h2, div h3 { color: blue;}
```

## **Selector universal**
- Asigna los estilos a todas las etiquetas HTML que no tengan estilos asignados.
```
* { color: black;}
```


## **Variables**
```
//Declaración de una variable

:root{
	--blanco: #EAEAEA;
}

//Utilización

background: var(--blanco);

```
