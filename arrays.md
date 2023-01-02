## **DEFINICIÓN DE ARRAYS**

Tras ver los tipos de datos primitivos, vamos ahora a ver otro tipo de datos que son los arrays. Vamos a profundizar en ellos.

Un array, como ya sabemos, es un conjunto de datos, un listado de datos (strings, numbers...) que irán entre corchetes y separados por comas. La sintaxis es la siguiente:


```jsx
[ elemento1, elemento2, ..., elementoN]
```


Podemos tener listados de todo tipo: numéricos, de strings, mixtos…


```jsx
let numerosPremiados = [3, 5, 43, 18, 27];
let listaCompra = ["Manzanas", "Peras", "Carne", "Papel de cocina"];
let varios = [3, "Manzanas", null, 18, true];
```


### **ACCEDER A LOS ELEMENTOS DE UN ARRAY**

Para acceder a los elementos de un array tenemos que entender el mismo como un listado, que empieza en el índice 0. Al igual que cuando hemos trabajado con los caracteres de un string.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];
let personaje = familiaSimpson[0];
console.log(personaje); //Mostrará por consola a Homer
```


Homer es la **posición 0** del array, Marge sería la **posición 4.**


### **PROPIEDAD LENGTH**

Para conocer el número de elementos de un array se puede consultar con la propiedad length. El método length nos va a venir muy bien a la hora de iterar sobre los elementos de un Array.


```jsx
familiaSimpson.length;
```

```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];
for (let i = 0; i < familiaSimpson.length; i++){
    console.log(familiaSimpson[i]);
}
```


## **MANIPULAR EL ARRAY ( Métodos que  modifican la matriz )**

Podemos también modificar un elemento concreto del array si indicamos su posición.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson[1] = "Mou"; //Estamos cambiando a Bart por Mou
console.log(familiaSimpson);
```


### **POP Y PUSH**

Pop y push son dos métodos con los cuales podemos eliminar y añadir elemento al final del array.

POP (elimina el último elemento)


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson.pop();
console.log(familiaSimpson); //Mostrará el listado sin Maggie

familiaSimpson.pop();
console.log(familiaSimpson); //Mostrará el listado sin Maggie y sin Marge
```


PUSH (añade al final del array).


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson.push("Bola de Nieve");
console.log(familiaSimpson); //Mostrará el listado añadiendo al final a Bola de Nieve

familiaSimpson.pop("Ayudante de Santa Claus", "Abe");
console.log(familiaSimpson); //Mostrará el listado añadiendo al final a Ayudante de Santa Claus y a Abe
```


### REVERSE

Invierte el orden del array.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson.reverse();
console.log(familiaSimpson); //Mostrará el listado al revés

```


### SHIFT

Funciona como el **pop()**  pero extraemos el primer elemento en vez del último.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson.shift();
console.log(familiaSimpson); //Desaparaece Homer
```
 

### SORT

Ordena los elementos de un array. Para hacer la ordenación pasa todos los elementos a strings y los ordena en orden alfabético.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

familiaSimpson.sort();
console.log(familiaSimpson); // Orden alfabético
```


### SPLICE

Acorta el array según los parámetros que le pasemos.


```jsx
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];

familiaSimpson.splice(2,2); // a partir de la posición 2(incluída) quita 2 elementos
console.log(familiaSimpson); // ['Homer', 'Bart', 'Maggie']

familiaSimpson.splice(2,2,'Moe'); // a partir de la posición 2 quita 2 elementos y añade a 'Moe'
```


## **MANIPULAR EL ARRAY ( Métodos que  no modifican la matriz )**

### CONCAT

Para concatenar un segundo array al primero.


```jsx
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];
let familiaFlanders = [ "Ned", "Todd", "Rod" ];

console.log(familiaSimpson.concat(familiaFlanders)); //['Homer', 'Bart', 'Lisa', 'Marge', 'Maggie', 'Ned', 'Todd', 'Rod']
```


### SLICE

Extrae una copia de la sección específica que decidamos.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

console.log(familiaSimpson.slice(2,4)); //['Lisa', 'Marge'] (Posición que inicia incluída, posición que para no incluída)
```


### **TOSTRING**

Convierte el array en un string.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

console.log(familiaSimpson.toString()); // 'Homer,Bart,Lisa,Marge,Maggie'
```


## **LOCALIZAR VALORES EN ARRAYS**

### INDEXOF

Devolverá el índice del primer elemento que coincida con el parámetro proporcionado, en caso contrario devolverá -1. 


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

console.log(familiaSimson.indexOf('Bart')) // 1
```
 

### LASTINDEXOF

Devolverá el índice del último elemento que coincida con el parámetro proporcionado, en caso contrario devolverá -1.


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Bart", "Marge", "Maggie"];

console.log(familiaSimson.lastIndexOf('Bart')) // 3
```


### **INCLUDES**

Devolverá `true` en caso de encontrar el elemento buscado, `false` si no lo encuentra


```jsx
let familiaSimpson = ["Homer", "Bart", "Lisa", "Marge", "Maggie"];

console.log(familiaSimson.includes('Lisa')) // true
```
