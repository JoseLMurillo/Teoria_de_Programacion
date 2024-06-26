# Variables
Las variables son contenedores que almacenan datos, es decir, espacios en memoria donde se guarda información. Cada variable tiene un nombre y puede contener diferentes tipos de datos, como números, cadenas de texto, o valores booleanos.

Imagina tus contactos de teléfono como variables, estos estarían representados con un nombre y un número que los identifica.

---

⛔ Como recomendación evitar usar tildes o espacios dentro de los nombres de las variables. Además de el uso de camelCase que es poner mayúsculas a palabras combinadas, por ejemplo: *variableSolicitada, nombrePersona, cuentaBancaria*.

---

**Pseudocódigo**
```
//variable pedro = +00 123456789
```

**JavaScript**
```jsx
let pedro = 00 1234567890
```

- **Declaración de Variables:**
	ℹ️ Las variables, como su nombre lo dice; pueden variar en el tiempo, es decir, que puedes cambiar su valor. Existe un tipo de contenedor de memoria que no varía y se conoce como constantes. A las constantes solo se les puede asignar un valor inicial.
    
	Cambiar el valor de una variable es útil si se almacenan datos que cambian en el tiempo. Para cambiar el valor contenido en una variable puedes hacerlo de la siguiente manera:
    
    **Pseudocódigo**
   ```
    # ALMACENA EDAD
    variable edad = 18
    
    # RESULTADO POR CONSOLA
    Mostrar edad
    
    # Reasigna edad
    edad = 20
    
    # El resultado que mostraria es 20
    Muestra edad
    ```
    
    **JavaScript**
    ```jsx
    //ALMACENA EDAD
    let edad = 18;
    
    //RESULTADO POR CONSOLA
    console.log(edad);
    
    //Reasigna edad
    edad = 20;
    
    # El resultado que mostraria es 20
    console.log(edad);
    ```
	
	ℹ️ Note se que no se vuelve a usar la palabra **let** al reasignar edad porque la variable edad ya existe, ocupa un espacio en memoria y no es necesario volver a crear otro espacio para almacenar ese dato.
	
    **Pseudocódigo**
    ```
    # VARIABLE TIPO TEXTO
    variable nombre = "Juan"
    
    # VARIABLE TPO NUMERO
    variable edad = 25
    
    # VARIABLE TPO NUMERO FRACCIONARIO
    variable numeroPi = 3.141592
    
    # VARIABLE TIPO BOOLEANO
    variable verdadero = true
    
    variabel falso = false
    ```
    
    **JavaScript**
    ```jsx
    //VARIABLE TIPO TEXTO
    let nombre = "Juan";
    
    //VARIABLE TPO NUMERO
    let edad = 25;
    
    //VARIABLE TPO NUMERO FRACCIONARIO
    let numeroPi = 3.141592
    
    //VARIABLE TIPO BOOLEANO
    let verdadero = true;
    
    let verdadero = false;
    ```

Si eres observador te has dado cuenta de que existen varios y diferentes tipos de datos, aquí puedes profundizar en ellos:

[Tipos de datos](Tipos%20de%20datos.md)