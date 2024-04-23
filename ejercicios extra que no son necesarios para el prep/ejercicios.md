# *Que es* JSON.stringify()

JSON.stringify() es un método en JavaScript que se utiliza para convertir un objeto JavaScript en una cadena JSON. Esta cadena JSON puede ser enviada a un servidor, almacenada en un archivo o transmitida a través de una red.

La función toma un objeto o valor de JavaScript como argumento y devuelve una cadena JSON que representa ese objeto o valor. Por ejemplo:

``` javascript
const objeto = { "nombre": "Juan", "edad": 30 };
const cadenaJSON = JSON.stringify(objeto);
console.log(cadenaJSON);
/* Resultado: {"nombre":"Juan","edad":30} */
```



## *metodos variantes de* JSON.stringify()

1. JSON.stringify(value): Esta es la forma más básica de usar JSON.stringify(). Toma un valor y lo convierte en una cadena JSON.

2. JSON.stringify(value, replacer): Permite especificar un reemplazo, que puede ser una función o un array, para controlar qué valores se incluyen en la cadena JSON resultante.

3. JSON.stringify(value, replacer, space): Además del reemplazo, también permite especificar un espacio, que puede ser un número o una cadena, para agregar sangría y espacios en blanco a la cadena JSON resultante.

4. JSON.stringify(value, replacer): Utilizado sin espacio, solo con un reemplazo. Es útil cuando solo necesitas modificar qué propiedades se incluyen en la cadena JSON, pero no necesitas cambiar el formato.

5. JSON.stringify(value, null, space): Utilizado con null como segundo argumento, solo con espacio. Esto aplica solo el formato sin filtrar o modificar el valor.

6. JSON.stringify(value, replacer, 0): Utilizado con 0 como tercer argumento, puede ser útil si solo deseas filtrar propiedades sin agregar sangría o espacios en blanco.

## *Ejercicios*

##### 1: Serialización de datos de un objeto simple: Crea un objeto JavaScript simple con algunas propiedades y luego utiliza JSON.stringify() para convertirlo en una cadena JSON.

##### 2: Serialización de un array de objetos: Crea un array que contenga varios objetos y utiliza JSON.stringify() para convertirlo en una cadena JSON.

##### 3: Serialización con opciones de formato: Utiliza JSON.stringify() con el argumento de espacio para agregar sangría y espacios en blanco a la cadena JSON resultante.

##### 4: Serialización con funciones de reemplazo: Utiliza JSON.stringify() con una función de reemplazo para personalizar qué propiedades se incluyen en la cadena JSON.

##### 5: Serialización con manejo de referencias circulares: Crea un objeto con referencias circulares (por ejemplo, un objeto que se referencia a sí mismo) y utiliza una variante como flatted.stringify() para serializarlo.

##### 6: Serialización con manejo de objetos no estándar: Crea un objeto con propiedades no estándar, como funciones o valores no primitivos, y observa cómo se manejan al usar JSON.stringify().

##### 7: Serialización de datos con comentarios: Utiliza una variante como JSON5.stringify() para serializar datos que contienen comentarios y observa cómo se manejan los comentarios en la cadena JSON resultante.

##### 8: Deserialización de una cadena JSON: Utiliza JSON.parse() para convertir una cadena JSON en un objeto o array de JavaScript.

##### 9: Deserialización con manejo de errores: Intenta deserializar una cadena JSON no válida y maneja adecuadamente los errores que puedan ocurrir.



