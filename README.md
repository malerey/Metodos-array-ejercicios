# Metodos de arrays: ejercicios


## Map

### 1

* Tenemos un array en una variable `numeros` con números al azar.
* Usá la función `map` para crear un nuevo array incrementando cada valor del array en 10, y guardarlo en la variable `numerosMasDiez`
* Mostrar por consola el array original y el nuevo

```js
const numeros = [1, 2, 3, 4, 5];

let numerosMasDiez;

// codear acá la solución del ejercicio


console.log(numeros); // [1, 2, 3, 4, 5]
console.log(numerosMasDiez); // [11, 12, 13, 14, 15]
```

### 2
* Tenemos un array en una variable `numeros` con números al azar.
* Usar la función `map` para crear un nuevo array multiplicando cada valor del array por 2, y guardarlo en la variable `dobles`
* Mostrar por consola el array original y el nuevo

```js
const numeros = [3, 7, 13, 99];

// codear acá la solución del ejercicio


console.log(numeros); // [3, 7, 13, 99]
console.log(dobles); // [6, 14, 26, 198]
```

### 3

* Tenemos un array en una variable `frases` con frases al azar.
* Usar la función `map` para crear un nuevo array donde cada frase empiece y termine con signo de exclamación.
* Mostrar por consola el array original y el nuevo

```js
const frases = ['Labore sea dolor.', 'Justo rebum dolor.', 'Stet lorem amet.'];

// codear acá la solución del ejercicio


console.log(frases); // ['Labore sea dolor.', 'Justo rebum dolor.', 'Stet lorem amet.']
console.log(frasesExclamadas); // [ '¡Labore sea dolor.!', '¡Justo rebum dolor.!', '¡Stet lorem amet.!' ]
```

### 4

* Tenemos un array en una variable `libros` con libros para leer sobre Javascript.
* Usar la función `map` para crear un nuevo array donde cada titulo de los libros esté encerrado en una etiqueta `<li></li>`.
* Mostrar por consola el array nuevo, encerrándolo entre `<ul></ul>`

```js
const librosDeJS = [
  'JavaScript for Kids: A Playful Introduction to Programming',
  'Composing Software',
  'Eloquent JavaScript: A Modern Introduction to Programming',
  'JavaScript: The Good Parts',
  'Programming JavaScript Applications: Robust Web Architecture with Node, HTML5, and Moderns JS Libraries',
  'Effective JavaScript: 68 Specific Ways to Harness the Power of JavaScript',
  'JavaScript: The Definitive Guide',
  'You Don’t Know JS',
  'JavaScript Allongé: The Six Edition'
];

// codear acá la solución del ejercicio



// el resultado final debería ser
// <ul><li>JavaScript for Kids: A Playful Introduction to Programming</li><li>Composing Software</li><li>Eloquent JavaScript: A Modern Introduction to Programming</li><li>JavaScript: The Good Parts</li><li>Programming JavaScript Applications: Robust Web Architecture with Node, HTML5, and Moderns JS Libraries</li><li>Effective JavaScript: 68 Specific Ways to Harness the Power of JavaScript</li><li>JavaScript: The Definitive Guide</li><li>You Don’t Know JS</li><li>JavaScript Allongé: The Six Edition</li></ul>
```

### 5

* Tenemos un array en una variable `frases` con frases al azar.
* Usar la función `map` para crear un nuevo array que contenga la longitud de cada palabra.
* Mostrar por consola el array original y el nuevo.

```js
const frases = ['Labore sea dolor.', 'Justo rebum dolor.', 'Stet lorem amet.'];

// codear acá la solución del ejercicio


console.log(frases); // ['Labore sea dolor.', 'Justo rebum dolor.', 'Stet lorem amet.']
console.log(longitudes); // [ 17, 18, 16 ]
```

### 6

* Tenemos un array en una variable `playlist` con una lista de canciones de un disco.
* Usar la función `map` para agregar a cada título de la canción el número de posición en la que está dentro del array.

```js
const playlist = ['Everlong', 'The Pretender', 'Learn to Fly'];

/// completá acá el código



// RESULTADO ESPERADO
// [ '0 - Everlong', '1 - The Pretender', '2 - Learn to Fly' ]
```

### 7

* Tenemos un array en una variable `costos` con números que representan costos de diferentes productos.
* Completar el siguiente código para llegar al resultado esperado
* A un costo primero se le agrega la ganancia y después el IVA

```js
const costos = [ 12.5, 56, 98, 45.75 ];

const agregarIVA = function (costo) {
  return costo * 1.21;
}

const sumarGanancia = function (costo) {
  return costo * 1.5;
}

// codear acá la solución del ejercicio


console.log(preciosFinales);
// deberia mostrar
// [ 22.6875, 101.64, 177.87, 83.03625 ]
```

### 8

* Tenemos un array en una variable `costos` con números que representan costos de diferentes productos.
* También tenemos un array en una variable `productos` con los nombres de cada producto.
* Completar el siguiente código para llegar al resultado esperado
* A un costo primero se le agrega la ganancia y después el IVA
* El nombre de un producto en una posición, se corresponde con el precio que está en la misma posición. Por ejemplo: el producto que está en la posición **1** tiene un costo igual al elemento en la posición **1** del array `costos`

```js
const productos = [ 'celular', 'notebook', 'monitor' ];
const costos = [ 12.5, 56, 98 ];

const agregarIVA = function (costo) {
  return costo * 1.21;
}

const sumarGanancia = function (costo) {
  return costo * 1.5;
}

// codear acá la solución del ejercicio


console.log(preciosFinales);
// deberia mostrar
// [ "celular 22.6875", "notebook 101.64", "monitor 177.87" ]
```

## Filter

### 1 

* Tenemos un array en una variable `costos` con números que representan costos de diferentes productos.
* Usando `filter`, crear un nuevo array con los precios más caros (mayores a 50) y guardarlo en la variable `losMasCaros`
* Mostrar el array original y el filtrado

```js
const costos = [ 39, 53, 17, 99, 7, 9, 6, 68, 54, 97, 27, 90, 92, 75, 26, 86, 22, 42, 20, 14 ];
// codear acá la solución del ejercicio


console.log(costos);
console.log(losMasCaros);
// deberia mostrar
// [ 39, 53, 17, 99, 7, 9, 6, 68, 54, 97, 27, 90, 92, 75, 26, 86, 22, 42, 20, 14 ]
// [ 53, 99, 68, 54, 97, 90, 92, 75, 86 ]
```

### 2 
* Tenemos un array en una variable `numeros` con números al azar.
* También tenemos dos arrays vacios en las dos variables `numerosPares` y `numerosImpares`.
* Utilizando `filter` crear un nuevo array con todos los números pares y guardalo en la variable `numerosPares`
* Utilizando `filter` crear un nuevo array con todos los números impares y guardalo en la variable `numerosImpares`

```js
const masNumeros = [ 43, 11, 18, 46, 44, 37, 42, 29, 9, 3, 37, 0, 40, 10, 38, 34, 25, 40, 4, 32 ];

// codea acá tu solución
const numerosPares = ;
const numerosImpares = ;

console.log("pares: ", numerosPares);
console.log("impares: ", numerosImpares);
// deberias tener como resultado
// pares: [18, 46, 44, 42, 0, 40, 10, 38, 34, 40, 4, 32]
// impares: [43, 11, 37, 29, 9, 3, 37, 25]
```

### 3

* Tenemos un array en una variable `mix` con varios elementos, de distintos tipos de datos.
* Usando `filter`, crear un nuevo array con todos los elementos que sean strings y guardalo en la variable `soloStrings`.
* Ayuda: para saber si algo es un string en javascript, podés usar typeof [ver más](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Operadores/typeof)
* Mostrar el array resultante

```js
const mix = [
  'Ut vero.',
  2,
  function () { console.log('hola mundo!') },
  56,
  'Diam rebum nonumy et.',
  true,
  false,
  'Kasd stet.',
  'Sit et dolor.',
  null,
  null,
  [ 1, 2, 3],
  'Dolore.'
];

// codear acá la solución del ejercicio

console.log(soloStrings);
// deberia mostrar
// [ 'Ut vero.', 'Diam rebum nonumy et.', 'Kasd stet.', 'Sit et dolor.', 'Dolore.' ]
```

### 4

* Tenemos un array `playlist` con canciones seleccionadas al azar por spotify para reproducir.
* Tenemos otro array `playlistEscuchada` que tiene canciones que ya escuchamos anteriormente.
* Usando `filter`, queremos crear una nueva lista que solo contenga aquellas canciones guardadas en `playlist` que no están en `playlistEscuchada`
* Guarda el resultado en la variable `playlistSinEscuchar`

```js
const playlist = ['Smells Like Teen Spirit', 'Everlong', 'Come As You Are', 'The Pretender', 'Heart-Shaped Box', 'Learn to Fly', 'Lithium'];
var playlistEscuchada = ['The Pretender', 'Lithium', 'Come As You Are']

/// codea aca tu solución


console.log(playlistSinEscuchar);
// deberia mostrar
// [ 'Smells Like Teen Spirit', 'Everlong', 'Heart-Shaped Box', 'Learn to Fly' ]
```

## Reduce

### 1

 Tenemos un array llamado `numbers` con números enteros al azar.
* Utilizando `reduce`, queremos calcular la suma de todos los números que están en el array.
* Por ejemplo: Si tenemos `[1, 2, 3]`, la suma de todos los números es **6**

```js
const numbers = [6, 1, 34, 94, 3, 17];

// codea debajo de este comentario la solucion al ejercicio

// deberia mostrar 155
```

### 2

* Tenemos un array llamado `numbers` con números enteros al azar.
* Utilizando `reduce`, queremos calcular la multiplicación de todos los números que están en el array.
* Por ejemplo: Si tenemos `[1, 2, 3, 4]`, la suma de todos los números es **24**

```js
const numbers = [6, 1, 34, 94, 3, 17];

// codea debajo de este comentario la solucion al ejercicio

// deberia mostrar 977976
```

### 3
* Tenemos un array llamado `notasDeTPs` con números del 1 al 10, que representan las notas de los distintos trabajos prácticos entregados por Grace Hopper en el curso de Ada.
* Usando `reduce`, queremos calcular la nota promedio final de trabajos prácticos _(el promedio se calcula sumando todas las notas y dividiéndolo por la cantidad de notas)_.
* Por ejemplo: Si tenemos `[7, 8, 9, 10]`, la nota final es **8.5**

```js
const notasDeTPs = [4, 7, 8, 5, 10];

// codea debajo de este comentario la solucion al ejercicio

// deberia mostrar 6.8
```

### 4
* Tenemos un array en una variable `libros` con libros para leer sobre Javascript.
* Usar la función `reduce` para crear un string con todos los titulos de los libros encerrados en una etiqueta `<li></li>`.
* Mostrar por consola el array nuevo
* Ayuda: ojo con el valor de comienzo

```js
const librosDeJS = [
  'JavaScript for Kids: A Playful Introduction to Programming',
  'Composing Software',
  'Eloquent JavaScript: A Modern Introduction to Programming',
  'JavaScript: The Good Parts',
  'Programming JavaScript Applications: Robust Web Architecture with Node, HTML5, and Moderns JS Libraries',
  'Effective JavaScript: 68 Specific Ways to Harness the Power of JavaScript',
  'JavaScript: The Definitive Guide',
  'You Don’t Know JS',
  'JavaScript Allongé: The Six Edition'
];

// codear acá la solución del ejercicio



// el resultado final debería ser
// <li>JavaScript for Kids: A Playful Introduction to Programming</li><li>Composing Software</li><li>Eloquent JavaScript: A Modern Introduction to Programming</li><li>JavaScript: The Good Parts</li><li>Programming JavaScript Applications: Robust Web Architecture with Node, HTML5, and Moderns JS Libraries</li><li>Effective JavaScript: 68 Specific Ways to Harness the Power of JavaScript</li><li>JavaScript: The Definitive Guide</li><li>You Don’t Know JS</li><li>JavaScript Allongé: The Six Edition</li>
```

### 5 

 Tenemos un array de objetos llamado `personas` con personas y edades .
* Utilizando `reduce`, queremos calcular la suma de todas las edades que están en el array.
* Ayuda: ojo con el valor de comienzo 

```js
const personas = [
    {nombre: "Grace", 
    edad: 6
    }, 
    {nombre: "Ada", 
    edad: 19
    },
    {nombre: "Hedy", 
    edad: 34
    }
  ];

// codea debajo de este comentario la solucion al ejercicio

// deberia mostrar 59
```

### integrador de todos los metodos

* Tenemos un array en una variable `datos` con números al azar, que pueden ser tanto positivos como negativos
* Queremos eliminar todos los números negativos
* Con los números restantes, obtener el doble de cada uno
* Finalmente, obtener la suma de todos los números que obtuvimos

```js
const datos = [2, -4, 6, 0, 5, -1];

// codear acá la solución del ejercicio
const total = ;

```
