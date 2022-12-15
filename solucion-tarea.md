Vamos a practicar ahora con una serie de ejercicios que nos van a ayudar a asentar todos estos conocimientos 😀

### EJERCICIO 1

```jsx
/*
    Completar el código de la función para que 
    devuelva la frase recibida sin vocales.
*/

let sentence = 'Hola soy Edu Feliz Navidad';

function noVowels(str){
    return str.replaceAll(/[aeiouAEIOU]/g,'');
}

console.log(noVowels(sentence));
```

 

### EJERCICIO 2

```jsx
/*
   Completar la función para que, recibida una palabra,
   devuelva el caracter que está en el medio. Si la palabra
   es par, devuelve los dos caracteres.

   Ejemplo: camión => mi

*/

let word = "camión";

function middleCharacter(str){
    return (str.length % 2 === 0) ? str[(str.length / 2) - 1] +  str[str.length / 2] : str[parseInt(str.length/2)];
}

console.log(middleCharacter(word));

```

### **EJERCICIO 3**

```jsx
/*
    Completar el código de la función para que 
    devuelva la frase recibida sin el primer y último parámetro.

*/

let sentence = 'Hola Don Pepito, hola Don José';

function deleteFirsLast(str){
    return str.slice(1,str.length-1);
}

console.log(deleteFirsLast(sentence));

```

### EJERCICIO 4

```jsx
/*
    Completar el código de la función para que 
    devuelva la suma de los elementos del array.
*/

let numberList = [1,2,-1,3,5,7];

function deleteFirsLast(list){
    let suma = 0;
    list.forEach(element => {
        suma += element;
    });
    return suma;
}

console.log(deleteFirsLast(numberList));
```

### EJERCICIO 5

```scss
/*
    Completar el código de la función para que 
    devuelva la el ganador del balón de oro, siendo 
		el que más puntuación tenga
*/

let numberList = [1,2,-1,3,5,7];

function deleteFirsLast(list){
    let suma = 0;
    list.forEach(element => {
        suma += element;
    });
    return suma;
}

console.log(deleteFirsLast(numberList));
```

### EJERCICIO 6

```jsx
/*
		Completar el código de la función para que 
    devuelva la suma de los elementos del array.
*/

let playerList = [
    {name:'Cristiano', score:300},
    {name:'Messi', score:250},
    {name:'Benzema', score:500}
];

function winner(list){
    list.sort((x, y) => y.score - x.score);
    console.log(list);
    return list[0].name;
}

console.log(winner(playerList));
```

### EJERCICIO 7

```jsx
/*
¡Se nos han mezclado los rebaños!
Tenemos 2 rebaños de ovejas(o) y vacas(v) mezclados y necesitamos ayuda.
Completar el código de la función para que, dado dos rebaños mezclados,
devuelva un objeto con el número de ovejas y número de vacas totales.

Ejemplo: 
    Rebaño 1 -> ["o","v","v","v","o","o","o","o","o","o","v","v","v","o"]
    Rebaño 2 -> ["o","o","o","v","o","v","o","o","v","o","v","o"]
    Resultado -> {nOvejas: 16, nVacas: 10}
*/

let rebano1 = ["o","v","v","v","o","o","o","o","o","o","v","v","v","o"];
let rebano2 = ["o","o","o","v","o","v","o","o","v","o","v","o"];

function counter(list1, list2){
    let list = list1.concat(list2).sort();
    return { nOvejas: list.lastIndexOf('o') + 1  , nVacas: list.length - list.indexOf('v') };
}

console.log(counter(rebano1,rebano2));
```

  

¡A por ello!