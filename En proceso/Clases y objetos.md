# Clases y objetos

La programación orientada a objetos (OOP) organiza el código en clases y objetos. Una clase es una plantilla para crear objetos, que son instancias de la clase.

- **Ejemplo de Clase y Objeto:**
    ```
    clase Persona
        propiedad nombre
        propiedad edad
    
        función inicializar(nombre, edad)
            esta.nombre = nombre
            esta.edad = edad
        fin_función
    
        función describir()
            retornar "Nombre: " + esta.nombre + ", Edad: " + esta.edad
        fin_función
    fin_clase
    
    objeto persona1 = nuevo Persona("Juan", 25)
    imprimir persona1.describir()
    
    ```