# Uso de Cookies

## **Declaración**
- Para saber si el checkbox está marcado se utiliza la función `request.getParameter(name).equals("on");` 
- Creación de cookie
	- `Cookie cookie = new Cookie(clave, valor);`
- Asignación de tiempo de vida
	- `cookie.setMaxAge(60 * 60 * 24); // Un día` 
- Almacenar la cookie en el response HTTP
	- `response.addCookie(cookie);`
## **Uso**
- Obtener todas las cookies
	- `Cookie[] cookies = request.getCookies();`
- Obtener una cookie en concreto
	- ``` 
	  String valor = "";
	  for (Cookie c : cookies){
			  if(c.getName().equals("usuario")){
				  valor = c.getValue();
			  }
	  }
	  ```