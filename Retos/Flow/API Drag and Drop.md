## Documentación Técnica para la API

En esta documentación se explicarán la API web fundamental para crear aplicaciones interactivas y dinámicas: Drag and Drop

#### API Drag and Drop
La API Drag and Drop de HTML5 permite a los usuarios arrastrar y soltar elementos HTML entre diferentes partes de una página web o incluso entre diferentes aplicaciones. Esto ofrece una forma intuitiva e interactiva de manipular datos y realizar acciones.

**Eventos principales:**
- **dragstart:** Se produce cuando el usuario comienza a arrastrar un elemento.
- **drag:** Se produce continuamente mientras el usuario arrastra el elemento.
- **dragenter:** Se produce cuando el elemento que se arrastra entra en la zona de destino (el elemento sobre el que se puede soltar).
- **dragover:** Se produce mientras el elemento que se arrastra está sobre la zona de destino.
- **dragleave:** Se produce cuando el elemento que se arrastra sale de la zona de destino.
- **drop:** Se produce cuando el usuario suelta el elemento que se arrastra sobre la zona de destino.

**Métodos principales:**
- **setDataTransfer():** Establece los datos que se transferirán al soltar el elemento.
- **getDataTransfer():** Recupera los datos transferidos al soltar el elemento.

**Ejemplo de uso:**

```html
<div id="draggable" draggable="true">Elemento draggable</div>

<div id="dropzone" ondrop="handleDrop(event)" ondragover="preventDefault()">Zona de destino</div>

```

```js
<script>
function handleDrop(event) {
  event.preventDefault();
  const data = event.dataTransfer.getData("text");
  const dropzone = document.getElementById("dropzone");
  dropzone.textContent = data;
}
</script>
```

