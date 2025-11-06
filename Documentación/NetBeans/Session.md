- Crear session
```
List<String> listaElementos = (List<String>) session.getAttribute("misElementos");

if(listaElementos == null){
	
	listaElementos = new ArrayList<String>();
	
	session.setAttribute("misElementos", ListaElementos);
}
```
La primera vez que el usuario entra la lista está vacía ya que el formulario aún no ha enviado ningún parámetro que se pueda guardar en la lista por lo que la lista va a ser igual a `null` por lo que inicializa la lista y se crea la session.

- Agregar elementos
```
String[] elementos = request.getParameterValues(name);

if (elementos != null){

	for (String elemTemp : elementos){
	
		listaElementos.add(elemTemp);
	
	}
}
```
La lista elementos recibe los valores del formulario y mediante un `foreach` lo almacena en la lista de elementos.