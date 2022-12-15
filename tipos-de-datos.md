En el video anterior trabajamos con variables pero únicamente guardamos un tipo de dato, el STRING, en este video vamos a ver otra serie de datos que podemos guardar en nuestras variables.

El tipo de dato que  tenemos que elegir a la hora de trabajar es el tipo de dato que defina mejor la información que vamos a guardar. Dicho esto, JS es un lenguaje de programación de tipado débil que significa que no tenemos que indicar el tipo de dato que hay que asignar a nuestra variable, pero los tenemos que conocer.

- STRING (cadena de texto)
- NUMBER (numérico)
- BOOLEAN (booleno)
- NULL (nulo)
- UNDEFINIED (no declarado / no valor)


## TIPOS DE DATO

### **STRING**

Asignación de valores de texto. Esta secuencia de texto se denomina cadena / cadena de caracteres y siempre tiene que ir entre comillas.


```jsx
let text = "Hola gente";
let message = "Bienvenidos al curso";
```


Para escribir cadenas en las que hay comillas simples o dobles, tendremos que jugar con las que utilicemos para asignarles un valor:


```jsx
let message = "Mi amigo me dijo: 'Más vale pájaro en mano...'";
```


En caso de querer mostrar comillas dobles dentro del texto jugaríamos con las simples al contrario.


### **NUMBER**

Asignación de valores numéricos. Pudiendo ser un número entero, decimal o negativo.


```jsx
let nEntero = 3;
let nDecimal = 3.5;
let nNegativo = -10;
```


Cuidado con poner números entre comillas ya que serán interpretados como una cadena de caracteres.


### **BOOLEAN**

Asignación de un valor lógico a la variable. Pudiendo ser true o false. No servirán para almacenar sobre todo información de si cumplen o no cumplen una condición, si esa es verdadera o falsa...
Tienen dos estados: **TRUE/FALSE**


```jsx
let tieneCarnet = true;     // Si es verdadero
let tieneCarnet = false;    // Si es falso
```


### **NULL**

Asignación de un valor nulo que no corresponde a dato concreto.


```jsx
let nombre = null;
```


### **UNDEFINED**

Nos indica que a una variable no se le ha dado un tipo de valor.


```jsx
let nombre;
console.log(nombre); // Devuelve undefined por que no se le ha dado ningún valor.
```


Podríamos volver a asignarle a una variable el tipo undefined una vez declarada.


```jsx
nombre = undefined;
```
 

### OBJETOS Y ARRAYS

Un objeto es una estructura de datos organizada mientras que los arrays nos sirven para agrupar diferente información que no necesita tener relación. Vemos un adelanto aunque este tipo de datos lo revisaremos en profundidad en otros videos.


```jsx
// Objeto
let simpson = {
	name:'Bart',
	surname: 'Simpson',
	age: 10
}

// List
let list = ['Edu', 5, true, 'Party'];
```


Para terminar, vamos a conocer también la función typeof que nos indicará el tipo de variable en cada momento:


```jsx
let name = typeof 'Edu'; // string
let age = typeof 31; // number
let isTeacher = typeof true; // boolean
```


Dicho esto, nosotros podríamos utilizar cualquier tipo de dato en nuestra variable, JS no nos va a exigir un tipo de dato concreto.

Para terminar combinamos tipos de datos en una variable para ver cómo actúa:


```jsx
let example1 = 'Homer'  + 10 + 5; // 'Homer105'
let example2 = 25 +5 + 'Homer'; // '30Homer'
```