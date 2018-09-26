* Hacer los dos pasos anteriores en uno:
>>**`git commit -am "Mensaje"`**

* Historial de commits:
>>**`git log`**

###Comandos Básicos II

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

###Comandos básicos III

* Ver diferencia entre los ficheros del directorio y los del repositorio de git:  
>>**`git diff`**

* Ver diferencia entre ficheros en el *staging* y el repositorio:
>>**`git diff --staged`**

* Eliminar archivos:
>	* Primero se elimina el archivo del directorio con:
>>**`git rm archivo`**

>	* Luego se valida el cambio realizado con:
>>**`git commit -m "Mensaje"**

* Mover o renombrar archivos:
>	* Primero se mueve o renombra el archivo con:
>>**`git mv <archivo_antiguo> <archivo_nuevo>`**

>	* Luego se valida el cambio realizado con:
>>**`git commit -m "Mensaje`**


