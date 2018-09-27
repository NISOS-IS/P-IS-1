# Tutorial de Git y GitHub
###Configuración Básica

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

###Comandos Básicos I

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
