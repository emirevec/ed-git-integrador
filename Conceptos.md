## Conceptos generales

### Git

Software de control de versiones diseñado por Linus Torvalds.

### Areas de Git

- #### Working directory
- #### Stagin area
- #### Repository (Local/Remote)

### Flujos de trabajo

- #### Long-Running Branch

Se crean varios branches (Ramas) que siempre estén abiertos y que utilizamos para diferentes etapas de su ciclo de desarrollo. Podemos fusionar las ramas regularmente unas con otras.

- #### Topic branch

Se crea una rama de corta duración que se usa para una característica particular o trabajo relacionado. El trabajo está separado en silos donde todos los cambios en esa rama tienen que ver con ese tema, es más fácil ver lo que sucedió durante la revisión del código.

- #### Administrador de integración

Incluye un *repositorio canónico* que representa el proyecto "oficial". A su vez cada desarrollador tiene acceso de escritura a su propio repositorio público y acceso de lectura a todos los  demás. El desarrollador envía una solicitud al responsable del proyecto principal para que realice sus cambios.

- #### Dictador y tenientes

Modalidad utilizada en grandes proyectos con cientos de colaboradores. Varios gerentes de integración están a cargo de ciertas partes del repositorio; se llaman *tenientes*. Todos los tenientes tienen un administrador de integración conocido como el *dictador benevolente*. El dictador benevolente hace push desde su
directorio a un repositorio de referencia del que todos los colaboradores deben hacer pull.

- #### Gitflow

Define un modelo de ramificación estricto diseñado en torno al lanzamiento del proyecto. Ideal para proyectos que tienen un ciclo de lanzamiento programado. Se utiliza dos ramas para registrar el historial del proyecto. La *rama maestra* almacena el historial de
lanzamiento oficial, y la *rama de desarrollo* sirve como una rama de integración de características. También es conveniente etiquetar todos los commits en la rama maestra con un número de
versión. Las *ramas de mantenimiento* "hotfix"se utilizan para parchear rápidamente las versiones de producción.