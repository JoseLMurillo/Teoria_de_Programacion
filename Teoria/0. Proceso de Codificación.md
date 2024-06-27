# Proceso de Codificación

En  [Conocimientos Previos](Conocimientos%20Previos.md) se menciona un proceso de codificación. La sugerencia es que tengas presente siempre este proceso al momento de enfrentarte a un código porque te facilitara el desarrollo del mismo:

- **Análisis de Requisitos**: Identificación de las necesidades y expectativas del usuario.
- **Diseño del Software**: Planificación de la estructura y componentes del software.
- **Programación**: Codificación del software utilizando lenguajes de programación.
- **Pruebas**: Verificación y validación del software para asegurar su funcionamiento correcto.
- **Mantenimiento**: Actualización y mejora continua del software para corregir errores y agregar nuevas funciones.
---
## Ejemplo
Entonces hagamos un ejemplo de este proceso:
- 🤔 **Análisis de Requisitos**:
	Supongamos que el usuario necesita un programa que calcule la suma de dos números. El usuario espera poder ingresar dos números y como resultado poder ver su suma.
	
	Entonces hagamos una lista de las cosas que podemos llegar a necesitar, como ejercicio intenta pensar en los elementos que crees que se necesitan:
	
	- Informar al usuario que es lo que hace el programa.
	- Dos variables para guardar o **almacenar** los dos números.
	- Una variable para almacenar el resultado de la suma.
	- Un mensaje que muestre la suma al usuario.

- **🎨Diseño del Software:**
	Aun podemos añadir más detalle:
	- En que forma se solicita al usuario los dos números? Con el uso de un método que pida información al usuario.
	- Como vamos a mostrar la información tanto de que hace el programa como el mensaje que muestra la suma? Con el uso de un método que muestre información al usuario.

- 🎯 **Programación:**
	En este ejemplo de código vamos a usar JavaScript:
	
```jsx
//Crea una alerta que muestra información en pantalla
alert("Este programa suma dos numeros");

//Dos variables para almacenar los dos números y resultado
let primerNumero;
let segundoNumero;
let resultado;

//Solicitud de los números
primerNumero = prompt("Ingresa el primer numero");
segundoNumero = prompt("Ingresa el segundo numero");

//Crea una alerta para mostrar el resultado
alert(`La suma de ${primerNumero} y ${segundoNumero} es ${resultado}`);
```

- 🤔 **Análisis del código**:
	Si analizas el código observaras que usamos diferentes cosas:
	- **let** es una palabra clave utilizada para declarar variables en JavaScript. También se puede usar var pero no es recomendado.
	- **prompt** es una función en JavaScript que muestra un cuadro de diálogo al usuario con un mensaje y un campo de entrada para que ingrese datos.
	- **alert** es una función en JavaScript que muestra un cuadro de diálogo al usuario con un mensaje y un botón "Aceptar".
	- **${}** es una característica de los template literals, una forma más flexible y legible de concatenar (unir) texto en JavaScript. También puedes hacerlo usando el signo +.

- **🔨 Prueba:**
	Esta etapa es para observar si hay algún error en tu código o si cumple con los requisitos que observaste en tu análisis.
	
	Por ejemplo, puedes ejecutar tu código dentro de la consola de navegación o carga desde un archivo HTML que este enlazado a tu archivo de JavaScript. [Como enlazar un HTML con JavaScript](Como%20enlazar%20un%20HTML%20con%20JavaScript.md) [Plugins recomendados](Plugins%20recomendados.md)
	Observa si hay algún error en tu código y corrígelo. 

- **🔧 Mantenimiento:**
	Esta etapa es para analizar error o quieres agregan nuevas funcionalidades a tu código


Teniendo todo lo anterior en cuenta puedes entonces iniciar con la [Teoría de programación JavaScript](Teori%CC%81a%20de%20programacio%CC%81n%20JavaScript%2006c98826aae046d79ed500c5a54facfa.md) 

---

# Video Tutoriales

- Diagrama de flujo
    
    [¡MEJORA tu LÓGICA de PROGRAMACIÓN!](https://www.youtube.com/watch?v=cShOfUMT5iA)
