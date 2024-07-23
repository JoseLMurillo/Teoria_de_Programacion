## Documentación Técnica: Programación Orientada a Objetos (POO) para el Proyecto Similar a Trello

La Programación Orientada a Objetos (POO) es una metodología de diseño de software que permite modelar el comportamiento y las características de los objetos en un sistema. En este proyecto, la POO ayudará a organizar el código de manera más modular y reutilizable. A continuación, se presenta cómo aplicar la POO en la creación de nuestra aplicación similar a Trello.

### Conceptos Básicos de POO
1. **Clases y Objetos**
   - **Clase**: Es un plano o plantilla que define las características y comportamientos que los objetos de esa clase pueden tener.
   - **Objeto**: Es una instancia de una clase.

   ```javascript
   class person {
	   //INICIALIZA LOS VALORES DE UN OBJETO | UNA CLASE PUEDE NO TENER UN CONSTRUCTOR
       constructor(name) {
           this.name = name;
       }
   }

	let pepe = new person('pepe');
   ```

2. **Encapsulamiento**
   - Es el concepto de ocultar los detalles internos de un objeto y exponer solo lo necesario a través de métodos públicos.

   ```javascript
   class person {
       constructor(name) {
           this.name = name;
           this.contacts = [];
       }

       get name() {
           return this.name;
       }

       set name(name) {
           this.name = name;
       }

       addContacts(contact) {
           this.contacts.push(contact);
       }

       removeFirstContact(contact) {
           this.contacts = this.contacts.pop();
       }

       get contacts() {
           return this.contacts;
       }
   }
   ```

3. **Herencia**
   - Permite crear nuevas clases basadas en clases existentes, inherente sus propiedades y métodos.

   ```javascript
   class person {
       constructor(name) {
           this.name = name;
           this.contacts = [];
       }

       get name() {
           return this.name;
       }

       set name(name) {
           this.name = name;
       }

       addContacts(contact) {
           this.contacts.push(contact);
       }

       removeFirstContact(contact) {
           this.contacts = this.contacts.pop();
       }

       get contacts() {
           return this.contacts;
       }
   }

   class engineer extends person {
       constructor(name, contacts, career) {
           super(name, contacts);
           this.name = name;
           this.conctact = contacts;
       }

       displayInfo() {
           console.log(`El ingeniero ${this.name} hizo la carrera de ${career}`);
       }
   }

	let pepe = new engineer('pepe', [123,456], 'Ciencias de datos.');

   ```

4. **Polimorfismo**
   - Permite a métodos con el mismo nombre comportarse de manera diferente según el objeto que los invoque.

   ```javascript
class Persona {
  constructor(nombre) {
    this.nombre = nombre;
  }

  presentarse() {
    console.log(`Hola, soy ${this.nombre}`);
  }
}

class Ingeniero extends Persona {
  constructor(nombre, especialidad) {
    super(nombre);
    this.especialidad = especialidad;
  }

  presentarse() {
    console.log(`Hola, soy ${this.nombre}, ingeniero de ${this.especialidad}`);
  }
}

const persona = new Persona('Juan');
const ingeniero = new Ingeniero('Maria', 'Software');

persona.presentarse();
ingeniero.presentarse();
   ```

**Clases Abstractas**

- Una clase abstracta no puede ser instanciada y está destinada a ser una base para otras clases. Puede contener métodos abstractos que deben ser implementados por las clases derivadas.

```js
class AbstractPersona {
  constructor(nombre) {
    if (new.target === AbstractPersona) {
      throw new TypeError("No se puede crear instancias directamente de AbstractPersona");
    }
    this.nombre = nombre;
  }

  presentarse() {
    throw new Error("Se debe sobreescribir el método presentarse()");
  }
}

class PersonaBasica extends AbstractPersona {
  constructor(nombre) {
    super(nombre);
  }

  presentarse() {
    console.log(`Hola, soy ${this.nombre}`);
  }
}

const persona = new PersonaBasica('Juan');
persona.presentarse();

```

#### Consideraciones Adicionales

- **Modularidad**: Mantener las clases y sus métodos en módulos separados para mejorar la organización y mantenibilidad del código.
- **Interfaz de Usuario**: Asegurarse de que la interfaz de usuario interactúe correctamente con las clases y el localStorage.

La implementación de la Programación Orientada a Objetos en nuestro proyecto similar a Trello permite una estructura clara y mantenible. Al encapsular la lógica en clases y aprovechar la persistencia con localStorage, podemos construir una aplicación robusta y fácil de mantener.
