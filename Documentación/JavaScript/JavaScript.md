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

- **Mostrar toda la información**
    - `console.log(personaje);`
- **Mostrar un solo atributo**
    - `console.log(personaje.nombre);`
    - `console.log(personaje['apellido']);`
- **Asignar un valor a un atributo concreto**
    - `personaje.edad = 23;`
    - `personaje['edad'] = 24;`
- **Asignar el valor de un atributo a una variable**
    - `let llave = 'edad';`
    - `personaje[llave] = 22;`
- **Eliminar un atributo**
    - `delete personaje.apellido;`

## **Array**

- **Declaración de un array**
    - `let animalesm = ['conejo', 'caballo'];`
- **Mostrar todos los elementos del array**
    - `console.log(animales)`
- **Mostrar un elemento en concreto**
    - `console.log(animales[0])`
- **Añadir más elementos al array**
    - `animales[2] = 'dragon';`
- **Mostrar la longitud del array**
    - `console.log(animales.length);`

## **Funciones**
```
function saludar () {
    console.log('Hola Mundo');
}

saludar();

function suma () {
    return 2 + 2;
}

let resultado = suma();
console.log(resultado);
console.log(suma());
```


## **Argumentos y parámetros**

```
function suma(a, b){
    return a + b;
}

let resultado = suma(5, 6);

console.log(resultado);
```

## **Operadores**

- **Aritméticos**
    - `+` Adición / agregación
    - `-` Resta
    - `*` Multiplicación
    - `/` División
    - `%` Resto
    - `**` Potencia / elevado
    - `++i` Incrementa u luego muestra
    - `i++` Muestra y luego incrementa
    - `--i` Decrementa y después muestra
    - `i--` Muestra y después decrementa
- **Asignación**
    - `+=`
    - `-=`
    - `*=`
    - `/=`
    - `%=`
    - `**=`
- **Comparación**
    - `>` Mayor que
    - `>=` Mayor o igual que
    - `<` Menor que
    - `<=` Menor o igual que
    - `==` Igual que
    - `!=` Distindo / negación
    - `===` Tipo y valor iguales
    - `!==` Tipo y valor diferentes
- **Lógicos**
    - `&&` AND
    - `||` OR
    - `!variable` NOT

## **Short-circuit**

Se pueden utilizar para asignar un valor a una variable en función de si su contenido tiene un valor u otro.
- `let nombre = '';`
- `let username = nombre || 'Anonimo';`
En caso de que la variable nombre no contenga nada se asignará el valor `'Anonimo'`.

## **Ternarios**

Se utilizan para devolver un valor u otro en función de si su resultado es `true` o `false`.
- `edad > 17 ? 'Es mayor de edad' : 'Es menor de edad';`



