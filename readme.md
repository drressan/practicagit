-¿Qué comando utilizaste en el paso 11? ¿Por qué? 

 Use el comando git reset –hard HEAD~1
Este comando mueve el HEAD a un commit anterior y el –hard borra los cambios en working copy

-¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 

Utilicé los comandos git reflog y git reset –hard IDdecommit
Con reflog sigo los pasos realizados hasta el momento y ubico el último commit que borré, utilizando el log de referencia, una vez ubicado el reset –hard #idcommit me devuelve el HEAD y restablece el working copy al commit deseado

 
-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 

El merge del paso 13 ya está actualizado, no causó conflicto porque la rama styled ya contenía ese commit

-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

El merge causo conflicto por el contenido de un archivo con el mismo nombre pero distinto contenido
 
-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?  

El merge no causó conflicto por que el contenido en era menor por lo que se borraron las líneas “sobrantes”

-¿Qué comando o comandos utilizaste en el paso 25?  

Utilicé el comando git config alias.graph “log --graph --decorate --pretty=oneline” para asignar alias a la palabra graph y luego usarlo en git graph para ”dibujar el diagrama

-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

El merge podría ser fast forward si se solucionan los conflictos ya que se añaden y quitan líneas

-¿Qué comando o comandos utilizaste en el paso 27? 

Utilicé el comando git reset HEAD~1 para deshacer el merge sin modificar el working copy

-¿Qué comando o comandos utilizaste en el paso 28? 

Para cancelar los cambios realizados se usa git restore git-nuestro.md

-¿Qué comando o comandos utilizaste en el paso 29? 

Para eliminar la rama title utilicé git branch -D title

-¿Qué comando o comandos utilizaste en el paso 30? 

Para rehacer el merge con title, utilicé git reflog para identificar el id del merge anterior,
git checkout idmerge para llegar a merge master absorbe title

-¿Qué comando o comandos usaste en el paso 32? 

Utilicé el comando git reflog para ubicar el id del commit donde se creó el poema y 
Me moví a él con git checkout #idiniciopoema

-¿Qué comando o comandos usaste en el punto 33? 
Utilicé el comando git reflog para ubicar el id del commit donde se añadió el titulo del poema y me moví a él con git checkout #idcommitcontitulo