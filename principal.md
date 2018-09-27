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

* Complementar Último commit:>>**`git commit --amed -m "Mensaje"`*** Recuperar versión de un fichero de commit antiguo:>>**`git checkout <id_commit> -- <nombre_archivo>`*** Revertir un commit:>>**`git revert <id_commit>`**### Comandos Básicos V* Deshacer múltiples cambios en el repositorio:>>**`git reset --soft <id_commit>`**>>**`git reset --mixed <id_commit>`**>>**`git reset --hard <id_commit>`*** Listar archivos que git no controla:>>**`git clean -n`*** Eliminar archivos que git no controla:>>**`git clean -g`*** Ignorar archivos en el repositorio: .gitignore### Comandos Básicos VI>>**`git ls-tree master`**   >>**`git ls-tree master^^^`**   >>**`git ls-tree master ̃ 3`*** Log en una línea:>>**`git log --oneline`*** Log con los tres últimos commits en una línea:>>**`git log -oneline -3`*** Para más opciones consultar documentación de git### Comandos Básicos VII* Examinar contenido de un commit: >>**`git show <id>`*** Comparar un commit con el actual:>>**`git diff <id> <nombre_archivo>`*** Comparar dos commits:>>**`git diff <id>..<id> <nombre_archivo>`**