### **DEFINICIÓN DE OBJETOS**

Tras aprender los tipos de datos primitivos y los arrays, vamos ahora a aprender que son los **OBJETOS.**

Tenemos que entender los objetos en JS como podríamos entender los objetos en la vida real. 

Una silla es un objeto con propiedades, tiene un diseño, un color, está fabricada de un material…

En JS de igual manera, tenemos objetos que tienen propiedades.

Estas propiedades son variables asociadas a un objeto, igual que las variables que hemos estado viendo, lo único que están ligadas a un objeto en si:


```jsx
silla.color; //objeto.propiedad
```


Vamos a ver como definir un objeto, por ejemplo unas zapatillas de una tienda online.


```jsx
let zapatilla = new Object();
zapatilla.marca = "Nike";
zapatilla.modelo = "Air Max";
zapatilla.talla = 45;
zapatilla.precio = 100;
```


Podríamos también definir un objeto (y es la que os recomendamos) usando un indicador objeto, mediante una lista con los nombres de la propiedad y el valor:


```jsx
let zapatilla = {
	marca: "Nike",
	modelo: "Air Max",
	talla: 45,
	precio: 100
};
```


Todas las propiedades no asignadas son de tipo UNDEFINED.


```jsx
zapatilla.color; //undefined
```


### **ACCESO A OBJETOS**

Para acceder al valor de una propiedad de un objeto tendríamos la siguiente sintaxis:


```jsx
NOMBREOBJETO["PROPIEDAD"]; 
```


Por ejemplo:

```jsx
let zapatilla = {
	marca: "Nike",
	modelo: "Air Max",
	talla: 45,
	precio: 100
};

let marcaZapatilla = zapatilla["marca"];
// let marcaZapatilla = zapatilla.marca también valdría

console.log(marcaZapatilla);//"Nike"
```


### **MODIFICACIÓN DE OBJETOS**

De igual manera, para modificar una propiedad de un objeto, podríamos hacer lo siguiente. 


```jsx
let zapatilla = {
	marca: "Nike",
	modelo: "Air Max",
	talla: 45,
	precio: 100
};

zapatilla["talla"] = 38;
//zapatilla.talla = 38 también valdría

console.log(zapatilla.talla);//38
```


Cualquier propiedad no definida nos devolverá undefined. De todas maneras, podemos añadir propiedades siempre que lo consideremos necesario:


```jsx
let zapatilla = {
	marca: "Nike",
	modelo: "Air Max",
	talla: 45,
	precio: 100
};
console.log(zapatilla["color"]); // Nos devolverá undefined

zapatilla["color"] = "Blanco";
//zapatilla.color = "Blanco" también valdría

console.log(zapatilla); // Ya tendríamos la propiedad incluida en el objeto
```


### RECORRER OBJETOS

Tenemos dos formas de recorrer objetos:


```jsx
let zapatilla = {
	marca: "Nike",
	modelo: "Air Max",
	talla: 45,
	precio: 100
};

// Opción de bucles

for (let clave in zapatilla) {
    console.log("Zapatilla tiene la clave " + clave + " con valor: " + zapatilla[clave]);
}

// Opción conocer las claves

let keys = Object.keys(zapatilla);
console.log(keys);
```


Seguiremos ampliando conocimiento de los objetos cuando trabajemos con POO (Programación Orienada a objetos) en siguientes sesiones.

 
