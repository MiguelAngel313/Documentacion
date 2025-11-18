- Creación
	- `document.cookie = "nombre=Miguel; expires=Sun, 26 Oct 2023 12:00:00 UTC; path=;";`
- Mostrar
	- `document.cookie`

## **Funciones para crear cookies**

```
function setCookie (name, value, dias){
	const fecha = new Date();
	fecha.setTime(fecha.getTime() + (dias * 24 * 60 * 60 * 1000);
	let expira = "expires=" + fecha.toUTCString();
	document.cookie = `${name}=${value}; ${expira}; path=/;`;
};
```

## **Funciones para recuperar cookies**

```
function getCookie(name) {
	const cookies = document.cookie.split('; ');
	
	for (let cookie of cookies) {
		const [cookieName, cookieValue] = cookie.split('=');
		if(cookie === name){
			return decodeURIComponent(cookieValue);
		}
	}
	return null;
};
```
