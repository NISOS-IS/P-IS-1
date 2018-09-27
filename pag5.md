* Resolver conflictos (se suele hacer manualmente):
>>**`git merge --abort`**

### Comandos Ramas III
* Almacenar cambios temporales:
>>**`git stash sabe "Mensaje"`**

* Listar cambios:
>>**`git stash list`**

* Ver contenido de un cambio temporal:  
>>**`git stash show -p <nombre_stash>`**

* Eliminar un cambio temporal:  
>>**`git stash drop <nombre_stash>`**

* Aplicar cambio del *stash*:
>	* Primero se hace:
>>**`git stash apply <nombre_stash>`**

>	* Luego se hace:
>>**`git stash pop <nombre_stash>`**  
