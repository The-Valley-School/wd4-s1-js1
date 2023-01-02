Existen unas serie de métodos que nos van a ayudar a trabajar con estos tipos de datos y nos van a dar funcionalidad añadida.


### STRING


```jsx
// length(): Devuelve la longitud de la cadena
let simpson = 'Homer';
console.log(simpson.length)

// includes(): Nos dice si un caracter o cadena se encuentra dentro de un string
let message = 'Hola soy Homer';
let simpson = 'Homer'
console.log(message.includes(simpson));

// repeat(): Devuelve un string con el número de copias que estemos aplicando
let simpson = 'Homer'
console.log(simpson.repeat(2));

// replace(): Sustituye
let movie = "The Simpson"
console.log(movie.replace('Simpson','GodFather'));

// replaceAll(): Sustituye todos los que se encuentre
let message = "Hola soy Edu, feliz navidad. Hola soy Edu, feliz navidad."
console.log(message.replaceAll('Edu','Fran'));

// slice(): Genera un string con la porción que cojamos
let message = 'Hola soy Homer';
console.log(message.slice(2,4));

// split(): Genera un array separando los elementos en función del separador
let message = 'Hola soy Homer';
console.log(movie.split(" "));

// chartAt():Devuelve el elemento en la posición que indiquemos empezando desde 0
let simpson = 'Homer';
console.log(simpson.charAt(1));

// toUpperCase(): Devuelve el elemento en mayúsculas
let simpson = 'Homer';
console.log(simpson.toUpperCase());

// toLowerCase(): Devuelve el elemento en minúsculas
let simpson = 'Homer';
console.log(simpson.toLowerCase());

// Trim(): Elimina los espacios iniciales y finales de la cadena
let simpson = 'Homer';
console.log(simpson.trim());
```
 

### NUMBER


```jsx
// isNaN(): Determina si el valor no es un número
let seasons = 21;
console.log(isNaN(seasons));

// Number.isInteger(): Determina si el valor es un número entero 
let seasons = 21;
console.log(Number.isInteger(seasons));

// parseInt(): Convierte strings a números enteros o decimales
let seasons = '21';
console.log(parseInt(seasons));

// toString(): Pasa el valor númerico a string
let seasons = 21;
console.log(seasons.toString());
```


## BOOLEAN
 

```jsx
// toString(): Pasa el valor númerico a string
let isFriday = true;
console.log(isFriday.toString());
```
