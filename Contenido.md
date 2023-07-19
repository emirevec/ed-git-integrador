## Comandos Git aplicados

Comandos aplicados al momento:

### git config

Permite obtener y configurar variables que controlan aspectos de cómo Git se va a ver y cómo va a operar.

> Niveles de configurarción:
> - Local. 
> - Global. 
> - System.

### git init

Inicia el control de versiones, crea en el directorio ejecutado el subdirectorio llamado ".git".  

> Estados de los archivos de un repositorio:
> - Committed. 
> - Modified. 
> - Staged.

### git status

Nos indica el estado de los archivos.

### git add

Incluye y da seguimiento a un archivo.

> Cambia el estado de **Untracked** a **Staged**.

### git commit

Confirma los cambios e incluye al archivo en una nueva versión del repositorio.

### git log

Lista los commits hechos en un repositorio en orden cronológico inverso.

### git remote 

Agrega un nuevo remoto a nuestro repositorio Git.

> Se vale de las propiedades "add <alias> <link_al_repositorio_remoto>".

### git push

Envía al repositorio remoto el historial de confirmaciones.

### git branch

Crea un nuevo apuntador móvil a una confirmación de cambios, *commit*.

> **HEAD** es el apuntador a la rama local en la que estés en ese momento.

### git checkout

Mueve el apuntador *HEAD* a la rama especificada.

### git merge

- *fast forward* mueve el apuntador hacia adelante, ya que la confirmación apuntada en la rama donde has fusionado estaba directamente arriba respecto a la confirmación actual.

- *fusión confirmada* crea una nueva versión del repositorio a tres bandas con su correspondiente confirmación de cambios, *commit*, que apunta este último.

### git clone

Obtiene una copia de un repositorio Git existente.

> Se vale de las propiedades "< url > < nombre_del_directorio_nuevo >".

### git fork

Crea una copia entera del proyecto en nuestra cuenta de usuario que quedará almacenada en nuestro espacio.

### git rebase

Abandona las confirmaciones de cambio ya creadas y crea nuevas, aplica los cambios confirmados de un branch sobre otro en vez de fusionar a tres bandas.

### git cherry-pick

Agrega una confirmación de cambios específica de otra rama.

### git stash

Toma las modificaciones de archivos en seguimiento y cambios ya listos que forman parte del stage area, y los guarda en una pila de cambios sin terminar.

### git bisect

Permite “automatizar” el trabajo de verificación de commits y realizar una búsqueda binaria sobre nuestro historial de cambios.  

### git tag

Crea una referencia al hash de un commit.

- *Anotados*, son referencias ideales para establecer lanzamientos oficiales de una aplicación, ya que se pueden subir al repositorio remoto.

- *No anotados*, no son enviados al momento de sincronización con el repositorio remoto.  

### git revert

Crea una referencia al hash de un commit.

- *Anotados*, son referencias ideales para establecer lanzamientos oficiales de una aplicación, ya que se pueden subir al repositorio remoto.

- *No anotados*, no son enviados al momento de sincronización con el repositorio remoto.  

### git reset

Ordena nuestro historial de cambios y borra aquellos commits que estuvieron de más, en los casos en que el repositorio local no se haya sincronizado con el repositorio remoto.

Flags que pueden utilizarse:

- *--soft* para que los cambios que hemos intentado resetear aún se mantengan visibles, pero ya no formen parte de ningún commit en nuestro branch.

- *--mixed* para que los cambios también se sigan manteniendo visibles en nuestros archivos pero sin formar parte del stage area.

- *--hard* para que todos los cambios que se hayan hecho durante ese tiempo no solo no formen parte del Stage Area sino que no puedan a verse tampoco en los archivos actuales, es decir nuestro Working Area.

