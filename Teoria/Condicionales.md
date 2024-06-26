# Condicionales
Las estructuras condicionales permiten ejecutar diferentes bloques de código según ciertas condiciones. Si se cumplen las condiciones retorna verdadero, de lo contrario retorna falso.

Podemos pensar los condiciones como una pregunta que si se cumple genera una respuesta.

- **Ejemplo de Condicional:**
    ```
    si (edad >= 18) entonces
        imprimir "Eres mayor de edad"
    sino
        imprimir "Eres menor de edad"
    fin_si
    ```
    
	Si observas el ejemplo usamos signos para preguntar si la edad es mayor o igual a 18, esto se llama comparadores. Existen diferentes comparadores, los más conocidos son:
    
    - > : Compara si un valor es mayor que otro y retorna verdadero si cumple.
    
    ```
    variable edad = 19
    si edad > 18 entonces
       imprimir "Eres mayor"
    ```
    
    - < : Compara si un valor es menor que otro y retorna verdadero si cumple.
        
        ```
        variable edad = 17
        si edad < 18 entonces
           imprimir "Eres menor"
        ```
        
    - == : Compara si un valor es igual a otro y retorna verdadero si cumple.
        
        ```
        variable edad = 18
        si edad == 18 entonces
           imprimir "Eres mayor"
        ```
        
    - === : Compara tanto el valor como el tipo de dato y retorna verdadero si cumple.
        
        ```
        variable edad = 18
        si edad === 18 entonces
           imprimir "Eres mayor"
        ```
        
    - ! = : Compara si un valor es diferente a otro y retorna verdadero si cumple.
        
        ```
        variable edad = 18
        si edad != 18 entonces
           imprimir "Eres mayor"
        ```
        
		También existe la combinación de los mayores menores con el igual
    
    - > =
    - < =

---

[Condicionales](Condicionales.md)
