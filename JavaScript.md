# Documentación de javaScript
## **Variables**
Declaración `let nombre = "Hola mundo";`  
Mostrar `console.log(nombre);`  
Redefinir `nombre = "Hola";`  
Declaración multiple `let nombre, apellido;`

## **Tipos de datos**

### **Primitivos**
- Number  
- String
- Boolean
- Undefined
- Null

### **De referencia**
- Array
- Object
- Functions
- Clases

## **Primitivos**

- `let numero = 1;`
- `let texto = "Hola mundo";`
- `let verdadero = true;`
- `let falso = false;`
- `let noDefinido;`
- `let undef = undefined;`
- `let nulo = null;`

## **Constantes**

Declaracion `const nombre = "Hola mundo";`

## **Tipado dinámico**
`console.log(typeof nombre);`

## **Comentarios**
>Ctrl + p: nombre de archivo a buscar  
//Línea comentada  
/*  
Varias líneas comentadas  
*/

## **Objetos**
```
    let personaje = {
        nombre: "Miguel",
        apellido: "Herrojo",
        edad: 22,
    };
```

- `console.log(personaje);`
- `console.log(personaje.nombre);`
- `console.log(personaje['apellido']);`
- `personaje.edad = 23;`
- `personaje['edad'] = 24;`
- `let llave = 'edad';`
- `personaje[llave] = 22;`
- `delete personaje.apellido;`