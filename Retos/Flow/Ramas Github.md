## Ramas Comunes para Desarrollar y Desplegar
1. **Rama Principal**
   - **main**: Rama principal donde se mantiene el código en producción.

2. **Ramas de Desarrollo**
   - **develop**: Rama de desarrollo donde se integran las funcionalidades antes de ser fusionadas a la rama `main`.
   - **feature/[nombre_funcionalidad]**: Ramas para el desarrollo de nuevas funcionalidades específicas.
     - Ejemplo: `feature/crear-tablero`

3. **Ramas de Hotfix**
   - **hotfix/[nombre_fallo]**: Ramas para corregir errores críticos en producción.
     - Ejemplo: `hotfix/corregir-error-login`

4. **Ramas de Release**
   - **release/[version]**: Ramas para preparar una nueva versión de la aplicación.
     - Ejemplo: `release/v1.0.0`

5. **Flujo de Trabajo**
   - Crear una nueva rama desde `develop` para trabajar en una nueva funcionalidad o corrección.
   - Realizar un pull request a `develop` una vez completada la funcionalidad.
   - Fusionar `develop` a `main` después de que todas las funcionalidades del sprint estén completas y probadas.
