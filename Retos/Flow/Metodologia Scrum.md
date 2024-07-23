## Metodología Scrum
1. **Roles del Equipo**
   - **Product Owner**: Responsable de definir las características y prioridades del producto.
   - **Scrum Master**: Facilita el proceso Scrum y asegura que el equipo sigue las prácticas ágiles correctamente.
   - **Equipo de Desarrollo**: Compuesto por tres personas que realizan el desarrollo y pruebas del proyecto.

2. **Historias de Usuario**
   - Se manejaran las funcionalidades con la estructura de historias de usuario y criterios de aceptación. La estructura de historias de usuario es la siguiente:
     Como `PERSONA INTERESADA`, quiero `FUNCIONALIDAD` para `MOTIVO DE LA HISTORIA`.
 
3. **Sprint Planning y Duración**
   - **Sprint Planning**: Definir las historias de usuario y las tareas específicas que se completarán en cada sprint.
   - **Duración del Sprint**: 

4. **Reuniones Diarias**
   - **Daily Standup**: Reunión diaria de 15 minutos para discutir el progreso, impedimentos y plan del día.

5. **Revisión y Retrospectiva**
   - **Sprint Review**: Demostración del trabajo completado al final de cada sprint.
   - **Sprint Retrospective**: Evaluación de lo que funcionó bien y qué puede mejorarse para el siguiente sprint.

### Historias de Usuario

#### Gestión de Tableros

1. **Crear Tablero**
   - **Historia de Usuario**: Como usuario, quiero crear un nuevo tablero para organizar mis proyectos.
   - **Criterios de Aceptación**:
     - El sistema debe proporcionar un botón para crear un nuevo tablero.
     - El usuario debe poder ingresar un nombre para el tablero.
     - El tablero debe aparecer en la lista de tableros después de ser creado.

2. **Editar Tablero**
   - **Historia de Usuario**: Como usuario, quiero editar el nombre de un tablero existente para actualizar su información.
   - **Criterios de Aceptación**:
     - Debe haber una opción para editar el nombre del tablero.
     - El usuario debe poder guardar los cambios realizados.
     - El nombre del tablero debe actualizarse en la lista de tableros.

3. **Eliminar Tablero**
   - **Historia de Usuario**: Como usuario, quiero eliminar un tablero que ya no necesito.
   - **Criterios de Aceptación**:
     - Debe haber una opción para eliminar un tablero.
     - El sistema debe solicitar confirmación antes de eliminar el tablero.
     - El tablero debe desaparecer de la lista de tableros tras ser eliminado.

#### Gestión de Listas

4. **Añadir Lista**
   - **Historia de Usuario**: Como usuario, quiero añadir una nueva lista a un tablero para categorizar mis tareas.
   - **Criterios de Aceptación**:
     - Debe haber un botón para añadir una nueva lista.
     - El usuario debe poder ingresar un nombre para la lista.
     - La lista debe aparecer en el tablero después de ser creada.

5. **Editar Lista**
   - **Historia de Usuario**: Como usuario, quiero editar el nombre de una lista existente para actualizar su información.
   - **Criterios de Aceptación**:
     - Debe haber una opción para editar el nombre de la lista.
     - El usuario debe poder guardar los cambios realizados.
     - El nombre de la lista debe actualizarse en el tablero.

6. **Eliminar Lista**
   - **Historia de Usuario**: Como usuario, quiero eliminar una lista que ya no necesito.
   - **Criterios de Aceptación**:
     - Debe haber una opción para eliminar una lista.
     - El sistema debe solicitar confirmación antes de eliminar la lista.
     - La lista debe desaparecer del tablero tras ser eliminada.

7. **Ordenar Listas**
    - **Historia de Usuario**: Como usuario, quiero ordenar las listas arrastrándolas y soltándolas para reorganizar mi tablero.
    - **Criterios de Aceptación**:
      - El usuario debe poder arrastrar una lista y soltarla en una nueva posición.
      - Las listas deben cambiar de posición en el tablero tras ser soltadas.

#### Gestión de Tarjetas

8. **Añadir Tarjeta**
    - **Historia de Usuario**: Como usuario, quiero añadir una nueva tarjeta a una lista para detallar mis tareas.
    - **Criterios de Aceptación**:
      - Debe haber un botón para añadir una nueva tarjeta dentro de una lista.
      - El usuario debe poder ingresar un nombre y descripción para la tarjeta.
      - La tarjeta debe aparecer en la lista después de ser creada.

9. **Editar Tarjeta**
    - **Historia de Usuario**: Como usuario, quiero editar el contenido de una tarjeta existente para actualizar su información.
    - **Criterios de Aceptación**:
      - Debe haber una opción para editar el contenido de la tarjeta.
      - El usuario debe poder guardar los cambios realizados.
      - La tarjeta debe actualizarse en la lista con la nueva información.

10. **Eliminar Tarjeta**
    - **Historia de Usuario**: Como usuario, quiero eliminar una tarjeta que ya no necesito.
    - **Criterios de Aceptación**:
      - Debe haber una opción para eliminar una tarjeta.
      - El sistema debe solicitar confirmación antes de eliminar la tarjeta.
      - La tarjeta debe desaparecer de la lista tras ser eliminada.

11. **Mover Tarjetas**
    - **Historia de Usuario**: Como usuario, quiero mover tarjetas entre listas arrastrándolas y soltándolas para reorganizar mis tareas.
    - **Criterios de Aceptación**:
      - El usuario debe poder arrastrar una tarjeta y soltarla en otra lista.
      - La tarjeta debe cambiar de lista tras ser soltada.

12. **Marcar Tarjeta como Completada**
    - **Historia de Usuario**: Como usuario, quiero marcar una tarjeta como completada para indicar que la tarea ha sido finalizada.
    - **Criterios de Aceptación**:
      - Debe haber una opción para marcar una tarjeta como completada.
      - La tarjeta debe mostrar un indicador visual que denote su estado completado.

#### Interfaz de Usuario

13. **Diseño Responsivo**
    - **Historia de Usuario**: Como usuario, quiero que la aplicación sea responsiva para poder usarla en diferentes dispositivos.
    - **Criterios de Aceptación**:
      - La interfaz debe adaptarse correctamente a diferentes tamaños de pantalla (desktop, tablet, móvil).
      - Los elementos deben reorganizarse adecuadamente en función del dispositivo.

14. **Notificaciones Visuales**
    - **Historia de Usuario**: Como usuario, quiero recibir notificaciones visuales para confirmar las acciones realizadas, como crear, editar o eliminar elementos.
    - **Criterios de Aceptación**:
      - Debe haber notificaciones visuales (por ejemplo, mensajes de toast) que confirmen las acciones del usuario.
      - Las notificaciones deben desaparecer automáticamente después de unos segundos.

Estas historias de usuario cubren las funcionalidades principales necesarias para desarrollar un MVP de la aplicación. Cada historia de usuario debe ser implementada y probada en el transcurso de los sprints planificados según la metodología Scrum.

#### Visual Story Map para la Aplicación Similar a Trello

A continuación, se presenta un visual story map organizado en una tabla para ordenar las historias de usuario en diferentes releases.

| **Épica**               | **Historia de Usuario**        | **Release 1** | **Release 2** | **Release 3** | **Release 4** |
| ----------------------- | ------------------------------ | ------------- | ------------- | ------------- | ------------- |
| **Gestión de Tableros** | Crear Tablero                  | X             |               |               |               |
|                         | Editar Tablero                 | X             |               |               |               |
|                         | Eliminar Tablero               | X             |               |               |               |
| **Gestión de Listas**   | Añadir Lista                   |               | X             |               |               |
|                         | Editar Lista                   |               | X             |               |               |
|                         | Eliminar Lista                 |               | X             |               |               |
|                         | Ordenar Listas                 |               |               |               | X             |
| **Gestión de Tarjetas** | Añadir Tarjeta                 |               |               | X             |               |
|                         | Editar Tarjeta                 |               |               | X             |               |
|                         | Eliminar Tarjeta               |               |               | X             |               |
|                         | Mover Tarjetas                 |               |               |               | X             |
|                         | Marcar Tarjeta como Completada |               |               | X             |               |
| **Interfaz de Usuario** | Diseño Responsivo              |               |               |               | X             |
|                         | Notificaciones Visuales        |               |               |               | X             |

Este visual story map organiza las historias de usuario en diferentes releases para facilitar el desarrollo incremental del proyecto y asegurar que se entreguen funcionalidades de valor en cada iteración.

