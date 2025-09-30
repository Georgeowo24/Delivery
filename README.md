# Delivery
## Duración del Sprint: 1 semana (5 días hábiles).

## Planificación (Día 1 - Responsable: JTR):
  * Definición del Backlog Inicial: Definir y detallar las historias de usuario del sprint.
  * Estimación de Historias de Usuario: El equipo estimará el esfuerzo de cada historia de usuario.
  * Asignación de Tareas: Distribuir las tareas entre los miembros del equipo, considerando los roles definidos.
## Codificación (Día 1-3 - Responsable: CHB, JRCS, CMA, VMR):
  * Desarrollo del Frontend:
    - JRCS, CMA, VMR: Implementar la interfaz de usuario para añadir, listar, editar y eliminar productos utilizando React.js y Tailwind CSS.
  * Desarrollo del Backend:
    - CHB, JTR, CMA: Desarrollar las Firebase Cloud Functions para manejar la lógica de negocio de añadir, listar, editar y eliminar productos, interactuando con Cloud Firestore.
  * Control de Versiones:
    - Todos: Programación en ramas feature/ por cada funcionalidad y uso de GitHub para el control de versiones.
## Integración Continua (Día 3-4 - Responsable: CHB):
  * Pipelines en GitHub Actions:
    - Ejecución automática de pruebas unitarias y de integración para el frontend y backend.
    - Análisis de código estático con ESLint.
    - Construcción de los artefactos de producción del frontend con Vite y compilación de las Cloud Functions.
## Pruebas (Día 4 - Responsable: JTR):
  * Pruebas Automatizadas:
    - JTR: Ejecutar pruebas unitarias, de integración y end-to-end de las funcionalidades implementadas.
    - Revisión de cobertura de código.
  * Rama Tester:
    - Los cambios de la rama development se enviarán a la rama tester para que JTR y el equipo realicen las pruebas finales antes de la integración a main.
## Entrega y Despliegue Continuo (Día 5 - Responsable: CHB):
  * Despliegue a Staging:
    - Una vez que las pruebas en la rama development sean exitosas y el pull request sea aprobado, se realizará un merge a la rama tester.
    - Un pipeline de GitHub Actions se activará con el push a la rama tester para desplegar automáticamente el frontend y las Cloud Functions al entorno de staging en Firebase Hosting.
  * Validación del Product Manager:
    - CHB: Validar las funcionalidades en el entorno de staging.
  * Despliegue a Producción (si la validación es exitosa):
    - Después de la validación exitosa en staging, se realizará un merge de la rama tester a la rama main.
    - Un pipeline de GitHub Actions se activará con el push a la rama main para desplegar automáticamente el frontend y las Cloud Functions al entorno de producción en Firebase Hosting.
## Monitoreo y Retroalimentación (Día 5 - Responsable: JTR):
  * Monitoreo: JTR: Utilizar las herramientas de monitoreo de Firebase (Performance Monitoring, Crashlytics) para observar el rendimiento y detectar problemas post-despliegue en producción.
* Retroalimentación: Recopilar retroalimentación para el próximo Sprint.

##
### Aplicación de comunicación a Utilizar: Discord.
