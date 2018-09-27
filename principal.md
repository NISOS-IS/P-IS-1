# Tutorial de Git y GitHub
### Configuración Básica

* Nombre del Administrador:
>>**`git config --global user.name "nombre_usuario"`**

* Correo Electrónico:
>>**`git config --global user.email "email_usuario@uco.es"`**

* Editor de Texto:
>>**`git config --global core.editor "nombre_editor"`**

* Color de la Interfaz:
>>**`git config --global color.ui true`**

* Listado de la Configuración:
>>**`git config --list`**

### Comandos Básicos I

Git cuente con 3 estados fundamentales:

* Directorio de Trabajo
* Área de Prueba (*Staged*)
* Directorio de Git (Repositorio)

Cuando trabajamos con Git, tenemos que seguir unos pasos básicos con nuestros proyectos. Estos pasos son:

* Iniciar repositorio en un directorio:
>>**`git init`**

* Agregar los cambios realizados en el directorio enlazado a git al área de prueba (*Staged*):
>>**`git add <nombre_archivo>`**

* Validar los cambios en el repositorio:
>>**`git commit -m "Mensaje"`**
* Hacer los dos pasos anteriores en uno:
>>**`git commit -am "Mensaje"`**

* Historial de commits:
>>**`git log`**

### Comandos Básicos II

* Ayuda del listado anterior:
>>**`git help log`**

* Listar los N commits más recientes:
>>**`git log -n N`**

>Por ejemplo, "**`git log -n 5`**" lista los 5 commits más recientes.

* Listar los commits desde una fecha:
>>**`git log --since=2018-09-18`**

* Listar los commits por autor:  
>>**`git log --autor="nombre_autor"`**

* Ver cambios en el directorio:  
>>**`git status`**

### Comandos básicos III

* Ver diferencia entre los ficheros del directorio y los del repositorio de git:  
>>**`git diff`**

* Ver diferencia entre ficheros en el *staging* y el repositorio:
>>**`git diff --staged`**

* Eliminar archivos:
>	* Primero se elimina el archivo del directorio con:
>>**`git rm archivo`**

>	* Luego se valida el cambio realizado con:
>>**`git commit -m "Mensaje"`**

* Mover o renombrar archivos:
>	* Primero se mueve o renombra el archivo con:
>>**`git mv <archivo_antiguo> <archivo_nuevo>`**

>	* Luego se valida el cambio realizado con:
>>**`git commit -m "Mensaje`**

### Comandos básicos IV

* Deshacer los cambios con git:  
>>**`git checkout -- <nombre_fichero>`**

* Retirar archivos del *staging*:  
>>**`git reset HEAD <nombre_fichero>`**



Las ramas o *branches* son la forma de separar la línea actual de desarrollo de nuestro proyecto con respecto a la principal. Estas distintas ramas representan normalmente distintas versiones del proyecto que posteriormente son integradas a la línea principal.

* Ver listado de ramas:
>>**`git branch`**

* Crear una rama:
>>**`git branch <nombre_rama>`**

* Moverse de una rama a otra:
>>**`git checkout <nombre_rama>`**

* Crear una rama y moverse a ella al mismo tiempo:
>>**`git checkout -b <nombre_rama>

* Comparar el contenido entre distintas ramas:
>>**`git diff <nombre_rama1>..<nombre_rama2>

### Comandos Ramas II

* Ver ramas idénticas a la actual:
>>**`git branch --merged`**

* Renombrar ramas:
>>**`git branch -m <nombre_antiguo> <nombre_nuevo>`**

* Eliminar ramas:
>	* Sirve para eliminar una rama, pero te pregunta si el contenido que hay en ella quieres guardarlo en otra rama o borrarla sin guardar nada.
>>**`git branch -d <nombre_rama>`**

>	* Sirve para eliminar una rama. En este caso no se te pregunta si el contenido lo quieres guardar o no, simplemente se elimina todo, perdiendo el contenido de dicha rama.
>>**`git branch -D <nombre_rama>`**

* Integrar ramas en la actual (guardar ramas en la actual):
>>**`git merge <nombre_rama>`**