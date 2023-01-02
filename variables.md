Vamos con las variables. Como vimos en el prework y también nos ha tocado ver en las sesiones de CSS, podemos entender una variable como un ‘cajón’ donde guardamos cierta información o dato, pudiendo acceder a la información de ese cajón cuando queramos además de poder cambiar la información que tenemos en el cajón. El poder utilizar esta información a lo largo de nuestro proyecto agiliza mucho el desarrollo.


## DECLARACIÓN DE VARIABLES

Para declarar una variable usamos la palabra **'var'** o **'let'** y a continuación el nombre que le queramos dar.


```jsx
var cajon; // Este es nuestro cajón (opción no recomendada)
let cajon; // Este es nuestro cajón (opción recomendada)
```


Recomendamos el uso de 'let' en vez de 'var'.


## ASIGNACIÓN DE VALOR

Ahora mismo nuestra variable no tiene ningún contenido, para asignarle un valor vamos a utilizar el operador **‘=’**


```jsx
let cajon;
cajon = 'calcetín'; 

// Podemos también declarar e inicializar el valor en una única línea
let cajon = 'calcetín';

// Podemos declarar e inicializar todas las variables que queramos en una línea, si separamos por comas.
let cajon = 'calcetín', armario = 'camisa', comoda = 'jersey';

// Nosotros recomendamos siempre declararlas en diferentes líneas para que visualmente sea más sencillo identificarlas.
let cajon = 'calcetín';
let armario = 'camisa';
let comoda = 'jersey';

// A la hora de declarar, es importante saber que no podemos usar el mismo nombre para declarar dos variables.
let cajon = 'calcetín';
let cajon = 'calzoncillo'; // JS no permite esto
```
  

## MODIFICACIÓN DEL VALOR

El valor de las variables puede cambiar, imagina que donde tenía un calcetín pase a ser un cinturón (Así las veces que quieras).


```jsx
//Inicializo y declaro
let cajon = 'calcetín';

//Cambio de valor
cajon = 'cinturón'; 

```


Para rizar un poco el rizo, podemos asignar una variable a otra variable.


```jsx
//Inicializo y declaro la primera variable
let miPrendaFavorita = 'calcetín';

//Inicializo y declaro la segunda variable que hace referencia a la primera
let buscoEstaPrenda = miPrendaFavorita; 

```


## NOMBRAR VARIABLES

- Utilizaremos siempre una palabra descriptiva de lo que vaya a contener.


```jsx
let manzana;    // Mal nombre para una variable si queremos indicar el título de una serie
let a;          // Mal nombre para una variable si queremos indicar el título de una serie
let serie;      // Buen nombre para una variable si queremos indicar el título de una serie
```


- Utilizaremos  nomenclatura lowerCamelCase. Cuando declaramos variables con más de una palabra estas se unen quitando los espacios, y empezando la palabra siguiente en mayúsculas.


```jsx
let Actor Principal;    // Mala forma de declarar si queremos indicar el actor principal
let ActorPrincipal;     // Mala forma de declarar si queremos indicar el actor principal
let actorPrincipal;     // Buena forma de declarar si queremos indicar el actor principal
```


- Como los equipos de desarrollo son cada vez más internacionales, es recomendable que nombremos las variables en inglés.
- Es muy importante también que el nombre de la variable sea único para impedir que se produzcan errores en el código.



## ¿EN QUÉ PARTE DEL CÓDIGO LAS DECLARAMOS?

Tenemos la opción de declarar las variables fuera de cualquier función. Estas variables tienen el nombre de VARIABLES GLOBALES y son accesibles desde cualquier parte del proyecto.

El enfoque que tenemos actualmente es intentar reducir al máximo estas variables e intentar que todas estén en sus funciones, aunque es cierto que a veces es necesario y útil tener cierta variable global que almacene datos genéricos.

Ls **variables locales**, una vez declaradas dentro de su función, solo podrán ser accesibles dentro de la misma.


```jsx
function showSimpson() {
	let simpson = "Homer";
	console.log( simpson );
}

showSimpson(); // Homer
console.log( simpson ); // Error
```


```jsx
let simpson = "Homer";

function showSimpson() {
	console.log( simpson );
}

showSimpson(); // Homer
console.log( simpson ); // Homer
```


```jsx
let simpson = "Homer";

function showSimpson() {
	let simpson = "Marge";
	console.log( simpson );
}

showSimpson(); // Marge
console.log( simpson ); // Homer
```
