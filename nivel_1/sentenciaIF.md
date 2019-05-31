# Sentencia de control if
Sirve para ejecutar un bloque de codigo al evaluar una expresion booleana (true, false), si dicha exprecion booleana (condicion) es verdadera entonces se ejecuta.

### Estructura de un if

```javascript
if( <expresion booleana> ) {
    // codigo a ejecutar si la evaluacion es true
} else {
    // codigo a ejecutar si la evaluacion es false
}
```
### Expresion booleana
Una expresion booleana es toda aquella evaluacion logica que tenga como resultado un `true` o `false` ejemplos de expresiones booleanas son las siguientes: 

```javascript
let ejecutarCodigo = true;
console.log('ejecutarCodigo', ejecutarCodigo)
// ejecutar codigo true
```

#### Ejemplos:

1. En el ejemplo 
```javascript
if (10 > 5) {
    // codigo...
}
```
la expresion `10 > 5` tiene como resultado `true` ya que es cierto que `10` es mayor que `5`, y por lo tanto se ejecuta el codigo dentro del if.

2. El siguiente codigo
```javascript
let numero1 = 2000
let numero2 = 100

if (numero1 < numero2){
    // codigo de if
} else {
    // codigo de else
}
```
El resultado de la expresion booleana `numero1 < numero` resulta ser `false` ya que 2000 no es menor que 100, por lo que se pocede a evaluar el codigo contenido en el bloque `else`.

### Negar una expresion booleana
Negar una expresion booleana significa cambiar negar el valor de una variable, negar true da como resultado false, negar false da como resultado true.

```javascript
let ejecutarCodigo = true;
console.log('negacion ejecutarCodigo', !ejecutarCodigo)
// negacion ejecutarCodigo false
console.log('doble negacion ejecutarCodigo', !!ejecutarCodigo)
// doble negacion ejecutarCodigo true

if ( ejecutarCodigo ){
    console.log('Este codigo se va a ejecutar')
}

if( !ejecutarCodigo ) {
    console.log('Este codigo no se va a ejecutar')
}
```

## Ejercicios
0. Ejemplo: dados dos vasos de bebida embriagantes elige el mezcal
Respuesta:
```javascript
let vaso1 = 'mezcal'
let vaso2 = 'cerveza'

if( vaso1 == 'mezcal' ) {
    console.log('me tomo el vaso 1')
}

if( vaso2 == 'mezcal' ) {
    console.log('me tomo el vaso 2')
}
```
1. Dados dos hermanos y sus edades encontrar al hermano menor,
   caso 1 => hermano1 = 21, hermano2 = 12
   caso 2 => hermano1 = 45, hermano2 = 52
   caso 3 => hermano1 = 1,  hermano2 = 4
Respuesta: 
```javascript
let hermano1 = 1
let hermano2 = 4

if (hermano1 < hermano2) {
    console.log(hermano1,'es menor que el ', hermano2)
}else{
    console.log(hermano2, 'es menor que el ', hermano1 )
}

```

```javascript
////////////////////////
/////////////////////////
///////////////////////

let azul = 'azul'
if (azul){
    console.log('si es azul', !!azul)
} else {
    console.log('no es azul')
}

let blanco = ''
console.log('blanco', !!blanco)
if(blanco) {
    console.log('soy color?', blanco)
} else {
    console.log('no soy color')
}


console.log('Ejercicio 0: -----------------------------------------------------------------------')
/*
*/

///////////////////////////////////////
let lumbreEncendida = false
let hayArroz = true

if(lumbreEncendida && hayArroz){
    console.log('me cocino arrocito')
} else {
    console.log('no hay arrocito hoy :(')
}
/////////////////////////////////////////

/*
  ejercicio: En una tienda de licor no se permite venta a menores de 18 anhos ni a mayores de 80, determinar si se puede vender o no
  caso 1 => persona = 25
  caso 2 => persona = 40
  caso 3 => persona = 17
  caso 4 => persona = 120
 */
console.log('Ejercicio 1: ------------------------------------------------------------------------')
/* ejecicio: dados 3 numeros encontrar el numero mayor: 
   caso 1 => a = 1, b = 2,  c = 3
   caso 2 => a = 4, b = 23, c = 0
   caso 3 => a = 5, b = 5,  c = 5
   caso 4 => a = 100 b = 200, c = 900
 */
let a = 1
let b = 2
let c = 3

if ( a > b) {
    console.log('a es mayor a b')
}

/*
  Ejercicio: Dado un numero x imprimir el numero en letas
  Ejemplo: x = 1 Resultado: UNO
  Ejemplo 2: x = 10 Resultado: Diez
  Caso 1 => x = 1
  Caso 2 => x = 2
  .
  .
  .
  Caso 10 => x = 10
 */

/*
  Ejercicio: Dados tres numeros, a,b,c calcular e imprimir a + b - c
  Caso 1 => a = 4, b = 25, c = 10
  Caso 2 => a = 1209, b = 1, c = 10000
  Caso 3 => a = 5, b = 0, c = 20
 */

/*
  Ejercicio: Dados dos numeros a y x determinar si a es multiplo de x
  Caso 1 => a = 5, x = 25
  Caso 2 => a = 3, x = 7
  Caso 3 => a = 21, x = 1
*/
/*
  Ejericio: Dados tres lados de un triangulo a, b, c determinar que tipo de triangulo es e imprirlo de acuerdo a las siguientes reglas:
  Equilatero: Si los tres lados son iguales
  Escaleno: Si los tres lados no son iguales

  Nota: Si el triangulo no se puede formar, imprimir 'No se puede formar un triangulo'
  Se sabe que un triangulo no se puede formar si alguno de sus lados es 0

  Caso 1 => a = 3, b = 4, c = 5
  Caso 2 => a = 2, b =2, c = 2
  Caso 3 => a = 1, b = 0, c = 20
  Caso 4 => a = 0, b = 0, c = 0
*/

/*
  Ejercicio: Calcular el area de un triangulo rectangulo, formula del area: lado por lado entre 2.
  Caso 1 => l = 1
  Caso 2 => l = 10
  Caso 3 => l = 400
 */
 
 /*
    Ejercicio: Tengo una mama y un papa como en la mayoria de las familias, y como en la mayoria de las familias cuando quiero salir a pasear con mis amigos sucede lo siguiente.
    Si alguno de mis papas dice que no entonces no puedo salir.
    Solo si ambos dicen que si entonces puedo salir.
    Caso 1 => mama dice que si papa dice que no
    Caso 2 => mama dice que no papa dice que si 
    Caso 3 => mama dice que si papa dice que si
    Caso 4 => mama dice que no papa dice que no
 */
 
 /*
    Ejercicio: Dados tres numeros: a,b,c imprimir el numero de enmedio, es decir el que no es el mayor ni el menor, bajo las siguientes condiones:
    Si los numeros son iguales, imprimir: 'no hay numero de enmdio'
    Si dos de los numeros son iguales, imprimir: 'me quieres ver la cara de estupida?'
    Si todos los numeros son 0, imprimr: 'buen intento'
    Caso 1 => a = 1, b = 5, c = 2
    Caso 2 => a = 1, b = 2, c = 3
    Caso 3 => a = 0, b = 15, c = 88788797
    Caso 4 => a = 0, b = 0, c = 1
    Caso 5 => a = 1, b = 1, c =1
 */

// https://www.udemy.com/programacion-para-principiantes/

```


