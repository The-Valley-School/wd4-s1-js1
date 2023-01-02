Vamos ahora a trabajar con operadores. Son símbolos matemáticos que nos van a permitir trabajar sobre dos valores para conseguir un resultado.


## **OPERADORES ARITMÉTICOS**

El primer grupo de operadores que vamos a ver son los aritméticos.
Nos van a permitir realizar operaciones matemáticas. Utilizamos los signos que conocemos de sobra:

- `=` Asignación
- `-`, `/`, `*` Resta, división y multiplicación
- `+` Suma, concatenación


### **ASIGNACIÓN**

Lo utilizamos para asignarle un valor a nuestra variable.


```jsx
let a = 3;
let b = 10;
```


## **RESTA, DIVISIÓN, MULTIPLICACIÓN**

Para realizar las operaciones necesarias sobre las variables.


```jsx
let resultadoResta = a - b;
let resultadoDivisión = a / b;
let resultadoMultiplicacion = a * b;
let resultadoEcuacion = (a - b) * a / b;
```


## **SUMA Y CONCATENACIÓN**

Para realizar operaciones numéricas o concatenación de cadenas de caracteres.


```jsx
let resultadoSuma = a + b;                  // Suma numérica, resultado 13
let frase = "Hola me llamo" + " " + "Edu";  //Concatenación, el resultado sería la cadena 'Hola me llamo Edu'
let resultadoSuma2 = "3" + "10";            //Se trataría de una concatenación, el resultado sería 310
let resultadoSuma3 = "3" + 10;              //Javascript lo seguiría interpretando como cadena, resultado 310
```


## **OPERADORES DE OPERACIÓN Y ASIGNACIÓN**

A la hora de trabajar en Javascript podemos operar y asignar de manera simultánea para poder conservar ciertos valores. Estos operadores serían:

- `+=` Suma y asignación
- `-=` Resta y asignación
- `*=` Multiplicación y asignación
- `/=` División y asignación


```jsx
let a = 3;
let b = 10;

a += b; // a = a + b
a -= b; // a = a - b
a /= b; // a = a / b
a *= b; // a = a * b

let frase1 = "Hola me llamo ";
let frase2 = "Eduardo";

frase1 += frase2; // frase1 = frase1 + frase2, resultado 'Hola me llamo Eduardo'
```
 

## **OPERADORES LÓGICOS**

Como su propio nombre indica, los operadores lógicos nos sirven para poder realizar operaciones lógicas con nuestras variables. Tenemos los siguientes:

- OR `||`: Se debe cumplir al menos una de las dos condiciones.
- AND `&&`: Deben cumplirse las dos condiciones.
- NOT `!`: Negamos el valor resultando el opuesto.


**OR**

Nos devuelve `true` en caso de que alguna de las variables de la comparativa sea `true`, en caso contrario, `false`.


```jsx
let tengoNetflix = true;
let tengoHBO = true;
let puedoVerSerie = tengoNetflix || tengoHBO;
```


**AND**

Nos devuelve true en caso de que se cumplan todas las condiciones, en caso contrario, false.


```jsx
let soyMayorDeEdad = true;
let tengoCarnet = true;
let puedoConducir = soyMayorDeEdad && tengoCarnet;
```


**NOT**

Nos devuelve el valor contrario al expuesto.


```jsx
let noVerdadero = !true; // false
let noFalso = !false; // true
```


## **OPERADORES DE COMPARACIÓN**

Utilizando los operadores de comparación vamos a poder comparar también variables.


- `==` : Igual
- `!=` : Distinto
- `===` : Estrictamente igual
- `!==` : Estrictamente distinto
- `<`  : Menor
- `<=` : Menor igual
- `>`  : Mayor
- `>=` : Mayor igual

Con `==` y `!=` comparamos variables sin tener en cuenta valor y el tipo de la variable.


```jsx
    3 == 3      //True
    3 == "3"    //True
    3 == 4      //False
    3 != 4      //True
    3 != "3"    //False
```


Con `===` y `!==` comparamos estrictamente incluyendo el valor y tipo de la variable


```jsx
    3 === 3      //True
    3 === "3"    //False
    3 === 4      //False
    3 !== 4      //True
    3 !== "3"    //True
```


Los símbolos `<`, `>`, `<=` , `>=` sirven para comparar valores numéricos


```jsx
    3 < 3      //False
    3 <= 3     //True
    3 > 4      //False
    10 >= 4    //True
```


## OPERADORES CONDICIONALES


```jsx
(condition) ? valor1 : valor2;
```


Si condition es true, el operador tiene el valor de valor1. De lo contrario, tiene el valor de valor2. Puedes utilizar el operador condicional en cualquier lugar donde normalmente utilizas un operador estándar. 


```jsx
let puedoConducir = (age >= 18) ? true : false;
```
