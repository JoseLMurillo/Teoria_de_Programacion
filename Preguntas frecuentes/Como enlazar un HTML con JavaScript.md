# Como enlazar un HTML con JavaScript

En el desarrollo web, HTML (HyperText Markup Language) se utiliza para estructurar el contenido de una página, mientras que JavaScript añade interactividad y comportamiento dinámico a la misma. Para aprovechar al máximo estas tecnologías, es esencial saber cómo enlazar un archivo JavaScript con un documento HTML.

### Estructura Básica de un Documento HTML

Un archivo HTML básico podría verse de la siguiente manera:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Página Web</title>
</head>
<body>
    <h1>Bienvenido a Mi Página Web</h1>
    <p>Este es un párrafo de ejemplo.</p>
</body>
</html>
```

---
### Enlazar un Archivo JavaScript Externo
Para enlazar un archivo JavaScript externo con tu HTML, debes utilizar la etiqueta `<script>` con el atributo `src` que apunta a la ubicación del archivo JavaScript.

Supongamos que tienes un archivo JavaScript llamado `script.js`. Para enlazarlo, agrega la siguiente línea dentro de la etiqueta `<head>` o antes del cierre de la etiqueta `<body>` en tu archivo HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Página Web</title>
    <script src="script.js"></script> <!-- Enlazar JavaScript en el head -->
</head>
<body>
    <h1>Bienvenido a Mi Página Web</h1>
    <p>Este es un párrafo de ejemplo.</p>
    <!-- También puedes enlazar JavaScript aquí -->
    <!-- <script src="script.js"></script> -->
</body>
</html>
```

---
### Estructura del Archivo JavaScript
El archivo `script.js` podría contener código JavaScript para interactuar con el contenido HTML, por ejemplo:

```jsx
// Esperar a que el documento esté completamente cargado
document.addEventListener("DOMContentLoaded", function() {
    // Seleccionar el elemento <h1> y cambiar su contenido
    var header = document.querySelector("h1");
    header.textContent = "¡Bienvenido a mi sitio web interactivo!";

    // Seleccionar el párrafo y cambiar su contenido
    var paragraph = document.querySelector("p");
    paragraph.textContent = "Este contenido ha sido modificado con JavaScript.";
});
```

---
### Enlazar JavaScript Interno (No recomendado)
También puedes incluir JavaScript directamente dentro del archivo HTML utilizando la etiqueta `<script>`:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Página Web</title>
    <script>
        // Esperar a que el documento esté completamente cargado
        document.addEventListener("DOMContentLoaded", function() {
            // Seleccionar el elemento <h1> y cambiar su contenido
            var header = document.querySelector("h1");
            header.textContent = "¡Bienvenido a mi sitio web interactivo!";

            // Seleccionar el párrafo y cambiar su contenido
            var paragraph = document.querySelector("p");
            paragraph.textContent = "Este contenido ha sido modificado con JavaScript.";
        });
    </script>
</head>
<body>
    <h1>Bienvenido a Mi Página Web</h1>
    <p>Este es un párrafo de ejemplo.</p>
</body>
</html>
```

---
### Diferencias entre Enlazar en el `<head>` y antes del cierre del `<body>`
1. **Enlazar en el `<head>`:**
    - El archivo JavaScript se carga antes de que se renderice el contenido del `body`. Esto puede causar errores si el JavaScript intenta manipular elementos que aún no existen en el DOM.
    - Es recomendable usar `defer` o `async` para evitar estos problemas:
        
        ```html
        <script src="script.js" defer></script>
        
        ```
        
2. **Enlazar antes del cierre del `<body>`:**
    - El archivo JavaScript se carga después de que todo el contenido del `body` se haya renderizado. Esto asegura que el DOM esté completamente cargado antes de que se ejecute el JavaScript.
    - No se necesita `defer` o `async`.

---
# Para saber más de JavaScript

[Teoría de programación JavaScript](../Teoria/Teoría%20de%20programación%20JavaScript.md)