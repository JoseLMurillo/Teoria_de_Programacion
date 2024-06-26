# Tipos de datos
En programación, los tipos de datos son fundamentales para definir la naturaleza de los datos que se manejan en un programa. A continuación se presentan los tipos de datos más comunes, explicados de manera general:

---
## **Comentarios**
Los comentarios son secciones del código que no son ejecutadas por el intérprete de JavaScript. Son extremadamente útiles para documentar el código, explicar la lógica detrás de ciertas secciones, hacer anotaciones temporales, y mejorar la legibilidad del código para otros desarrolladores (o para ti mismo en el futuro).

ℹ️ JavaScript admite dos tipos de comentarios: comentarios de una sola línea y comentarios de múltiples líneas.

---
### Comentarios de una Sola Línea
Los comentarios de una sola línea comienzan con `//`. Todo lo que esté después de `//` en esa línea será considerado un comentario y no será ejecutado.

**Pseudocódigo**
```
# Esto es un comentario de una sola línea
variable x = 5; # Esto también es un comentario de una sola línea
```

**JavaScript**
```jsx
// Esto es un comentario de una sola línea

var x = 5; 

//let y = 3; cuando comentamos una porción de código este va a aparecer de un color mas oscuro, como se nota en esta línea de la variable en la que escribo

// Esto también es un comentario de una sola línea
```

---
### **Comentarios de Múltiples Líneas**
Los comentarios de múltiples líneas comienzan con `/*` y terminan con `*/`. Todo lo que esté entre estos delimitadores será considerado un comentario.

```jsx
/*
  Esto es un comentario de múltiples líneas.
  Puedes escribir tantas líneas como necesites.
*/
var y = 10;
```

---
## **Enteros**:
Representan **números** enteros, ya sean positivos o negativos, y cero.

**Seudo Código**
```
variable numeroPositivo = 10
variable numeroCero = 0
variable numeroNegativo = -10
```

**JavaScript**
```jsx
let numeroPositivo = 10
let numeroCero = 0
let numeroNegativo = -10
```

---
## **Flotantes o fraccionarios**:
Representan números con decimales, es decir, números que tienen una parte fraccionaria. Como el número pi.

**Seudo Código**
```
variable numeroPi = 3.14
```

**JavaScript**
```
let numeroPi = 3.14
```

---
## **Cadenas de texto o String o Chards**:
Representan caracteres individuales y secuencias de caracteres, como palabras o frases. También se pueden incluir números o otros símbolos 

**Seudo Código**
```
variable nombre = "Juan"
variable simbolos = 
```

**JavaScript**
```jsx
let nombre = "Juan"
```

---
## **Valores de Verdad o Boolean:**
Representan valores de verdad, típicamente true (verdadero) o false (falso). Estos valores serán muy útiles cuando se usen los condicionales.

**Seudo Código**
```
variable verdadero = true
variable falso = false
```

**JavaScript**
```jsx
variable verdadero = true
variable falso = false
```

---
## **Arreglos o Arrays**:
Representan una colección ordenada de elementos del mismo tipo, accesibles mediante índices.

**Seudo Código**
```
  variable arregloNumeros = [1,2,3,4]
  variable arregloCaracteres = ["a","b","c"]
```

**JavaScript**
```jsx
  let arregloNumeros = [1,2,3,4];
  let arregloCaracteres = ["a","b","c"];
```

---

ℹ️ Puedes incluso tener dentro de los arreglos otros arreglos, esto se conoce como matrices.

---

Cada elemento en un array tiene un índice, que es su posición dentro del array. Los índices en JavaScript comienzan en 0, lo que significa que el primer elemento está en el índice 0, el segundo en el índice 1, y así sucesivamente.

Puedes acceder a un valor específico del array utilizando su índice.

**Seudo Código**
```
# Acceder al primer elemento del array de números
variable primerNumero = numeros[0];

# Acceder al segundo elemento del array de frutas
variable segundaFruta = frutas[1];
```

**JavaScript**
```jsx
// Acceder al primer elemento del array de números
let primerNumero = numeros[0];

// Acceder al segundo elemento del array de frutas
let segundaFruta = frutas[1];
```

---

ℹ️ También puedes cambiar el valor de un elemento en un array asignando un nuevo valor a un índice específico.

---

**Seudo Código**
```
# Cambiar el valor del primer elemento del array de números
numeros[0] = 15;

# Cambiar el valor del segundo elemento del array de frutas
frutas[1] = "pera";
```

**JavaScript**
```jsx
// Cambiar el valor del primer elemento del array de números
numeros[0] = 15;

// Cambiar el valor del segundo elemento del array de frutas
frutas[1] = "pera";
```

### Longitud del Array
La propiedad `length` de un array devuelve el número de elementos que contiene.

**Seudo Código**
```
variable longitudNumeros = numeros.tamaño;
```

**JavaScript**
```jsx
let longitudNumeros = numeros.length;
```

---

ℹ️ Para acceder a cada elemento de un array, puedes utilizar bucles como `for`, `forEach`, `for...of`, y `map`.

---
## **Listas o Lists**:
Similar a los arreglos, pero pueden contener elementos de diferentes tipos y suelen tener métodos adicionales para la manipulación de sus elementos.

<aside>
⚠️ Todas las características de los arreglos se transfieren a las listas.

</aside>

**Seudo Código**
```
variable lista = [1,"abc",3.0,true]
```

**JavaScript**
```jsx
let lista = [1,"abc",3.0,true];
```

---

ℹ️ Puedes incluso tener dentro de las listas otras listas y arreglos, esto se conoce como matrices.

---
## **Estructuras, objetos, Structs o Records**:
En JavaScript, los objetos son estructuras de datos que permiten almacenar colecciones de valores mediante pares clave-valor. Los objetos pueden contener otros objetos, arrays y valores primitivos como números y cadenas de texto.

**Seudo Código**
```
variable persona = {
   nombre: "Ana",
   edad: 30,
   esEstudiante: false
   contactos: ["Juan", "Luis"]
   mascota: {
     nombre: "pepe",
     edad: 2
     sexo: "M"
   } 
}
```

**JavaScript**
```jsx
let persona = {
   nombre:"Ana",
   edad: 30,
   esEstudiante: false
   contactos: ["Juan", "Luis"]
   mascota:{
     nombre: "pepe",
     edad: 2
     sexo: "M"
   } 
}
```

La notación de punto es una forma común y fácil de acceder a los valores de un objeto.

**Seudo Código*
```
# Acceder al nombre de la persona
variable nombre = persona.nombre;

# Acceder a la edad de la persona
variable edad = persona.edad;

# Acceder al estado de estudiante de la persona
variable esEstudiante = persona.esEstudiante;
```

**JavaScript**
```jsx
// Acceder al nombre de la persona
let nombre = persona.nombre;

// Acceder a la edad de la persona
let edad = persona.edad;

// Acceder al estado de estudiante de la persona
let esEstudiante = persona.esEstudiante;
```

La notación de corchetes permite acceder a las propiedades del objeto utilizando una cadena de texto.

**Seudo Código**
```
# Acceder al nombre de la persona
variable nombre = persona["nombre"];

# Acceder a la edad de la persona
variable edad = persona["edad"];

# Acceder al estado de estudiante de la persona
variable esEstudiante = persona["esEstudiante"];
```

**JavaScript**
```jsx
// Acceder al nombre de la persona
let nombre = persona["nombre"];

// Acceder a la edad de la persona
let edad = persona["edad"];

// Acceder al estado de estudiante de la persona
let esEstudiante = persona["esEstudiante"];
```

---
### Acceder a Arrays dentro de un Objeto
El objeto `persona` contiene un array llamado `contactos`. Puedes acceder a los elementos de este array utilizando su índice.

**Seudo Código**
```
# Acceder al primer contacto
variable primerContacto = persona.contactos[0];

# Acceder al segundo contacto
variable segundoContacto = persona.contactos[1];
```

**JavaScript**
```jsx
// Acceder al primer contacto
let primerContacto = persona.contactos[0];

// Acceder al segundo contacto
let segundoContacto = persona.contactos[1];
```

### Acceder a Objetos Anidados
ℹ️ El objeto `persona` también contiene otro objeto llamado `mascota`. Puedes acceder a sus propiedades utilizando la notación de punto o la notación de corchetes.

**Seudo Código**
```
# Acceder al nombre de la mascota
variable nombreMascota = persona.mascota.nombre;

# Acceder a la edad de la mascota
variable edadMascota = persona.mascota.edad;

# Acceder al sexo de la mascota
variable sexoMascota = persona.mascota.sexo;
```

**JavaScript**
```jsx
// Acceder al nombre de la mascota
let nombreMascota = persona.mascota.nombre;

// Acceder a la edad de la mascota
let edadMascota = persona.mascota.edad;

// Acceder al sexo de la mascota
let sexoMascota = persona.mascota.sexo;
```

---
### Acceso con Notación de Corchetes
**Seudo Código**

```
# Acceder al nombre de la mascota
variable nombreMascota = persona["mascota"]["nombre"];

# Acceder a la edad de la mascota
variable edadMascota = persona["mascota"]["edad"];

# Acceder al sexo de la mascota
variable sexoMascota = persona["mascota"]["sexo"];
```

**JavaScript**
```jsx
// Acceder al nombre de la mascota
let nombreMascota = persona["mascota"]["nombre"];

// Acceder a la edad de la mascota
let edadMascota = persona["mascota"]["edad"];

// Acceder al sexo de la mascota
let sexoMascota = persona["mascota"]["sexo"];
```

### Modificar Valores en el Objeto
Puedes modificar los valores de las propiedades del objeto utilizando la notación de punto o la notación de corchetes.

**Seudo Código**
```
# Modificar el nombre de la persona
persona.nombre = "Ana María";

# Modificar la edad de la mascota
persona.mascota.edad = 3;

# Modificar el primer contacto
persona.contactos[0] = "Carlos";
```

**JavaScript**
```jsx
//Modificar el nombre de la persona
persona.nombre = "Ana María";

// Modificar la edad de la mascota
persona.mascota.edad = 3;

// Modificar el primer contacto
persona.contactos[0] = "Carlos";
```

ℹ️ Puedes usar un bucle `for...in` para recorrer todas las propiedades de un objeto.