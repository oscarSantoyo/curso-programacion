# Nivel 1

## Introduccion

### Variables
Las sirven para almacenar datos durante la ejecucion del programa y dicho dato puede variar (cambiar de valor). 
Las `keyWords` con las que se pueden declarar variables en JavaScript son `let` `var` y existe un tipo especial de variables que no permite modificaciones es decir, sirve para contener valores estaticos: `const`

#### Declaracion de variables 
```javascript
var variable; // variable comun
let variable; // variable comun
const variable; // variable constante
```

#### Tipos de variables 


// En este ejemplo la primera variable es 'el valor de la variable es:' y la segunda es la variable declarada llamada ejecutar codigo cuyo valor es true.

let variableNumerica = 10 // Esta es una variable numerica ya que contiene un numero
let variableBooleana = false // Esta es una variable booleana ya que contiene un valor booleano (true, false)
let variableString = 'soy un string' // Esta es una variable string ya que contiene un valor String, cualquier cadena o texto usando comilla simple o comilla doble

### Impresion a la terminal
Usamos `console.log()` para imprimir texto a la terminal, es una funcion que recibe como parametro las variables que se quieran imprimir es por eso que las separamos con comas.
```javascript
let variable = 10
console.log('Esto sera impreso en consola', variable)
```

#### USE STRICT 
Esta instruccion especifica a Node ejecutarse de modo estricto, lo que significa que reportar los errores encontrados en el codigo.

```javascript
"use strict"
```


