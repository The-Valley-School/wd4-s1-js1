Existen unas serie de métodos que nos van a ayudar a trabajar con estos tipos de datos y nos van a dar funcionalidad añadida


### STRING


```jsx
// LENGTH: Devuelve la longitud de la cadena
let simpson = 'Homer';
console.log(simpson.length)

// INCLUDES(): Nos dice si un caracter o cadena se encuentra dentro de un string
let message = 'Hola soy Homer';
let simpson = 'Homer'
console.log(message.includes(simpson));

// REPEAT(): Devuelve un string con el número de copias que estemos aplicando
let simpson = 'Homer'
console.log(simpson.repeat(2));

// REPLACE(): Sustituye
let movie = "The Simpson"
console.log(movie.replace('Simpson','GodFather'));

// REPLACEALL(): Sustituye todos los que se encuentre
let message = "Hola soy Edu, feliz navidad. Hola soy Edu, feliz navidad."
console.log(message.replaceAll('Edu','Fran'));

// SLICE(): Genera un string con la porción que cojamos
let message = 'Hola soy Homer';
console.log(message.slice(2,4));

// SPLIT(): Genera un array separando los elementos en función del separador
let message = 'Hola soy Homer';
console.log(movie.split(" "));

// CHARAT():Devuelve el elemento en la posición 1 empezando desde 0
let simpson = 'Homer';
console.log(simpson.charAt(1));

// TOUPPERCASE(): Devuelve el elemento en mayúsculas
let simpson = 'Homer';
console.log(simpson.toUpperCase());

// TOLOWERCASE(): Devuelve el elemento en minúsculas
let simpson = 'Homer';
console.log(simpson.toLowerCase());

// TRIM(): Elimina los espacios si los hubiese en nuestra cadena
let simpson = 'Homer';
console.log(simpson.trim());
```
 

### NUMBER


```jsx
// ISNAN(): Determina si el valor es number (not a number)
let seasons = 21;
console.log(isNaN(seasons));

// NUMBER.ISINTEGER(): Determina si el valor es número entero 
let seasons = 21;
console.log(Number.isInteger(seasons));

// PARSEINT(): Convierte strings a números enteros o decimales
let seasons = '21';
console.log(parseInt(seasons));

// TOSTRING(): Pasa valor númerico a string
let seasons = 21;
console.log(seasons.toString());
```


## BOOLEAN
 

```jsx
// TOSTRING(): Pasa valor númerico a string
let isFriday = true;
console.log(isFriday.toString());
```
