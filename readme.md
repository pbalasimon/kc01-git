**¿Qué comando utilizaste en el paso 11? ¿Por qué?**
git reset --hard HEAD~1. Para mover una rama a un commit anterior se hace con el comando reset. El modificador de hard es porque se pedía que se perdieran los cambios del working copy. Por defecto no elimina los archivos. También se podía haber hecho mirando el reflog y obteniendo el hash del commit anterior.


**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
Primero reflog para obtener el hash del commit anterior, y después, git reset --hard hash. Para recuperar de nuevo nuestro trabajo, con el modificador hard para que nos cambie el working copy.


**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
No, no causó ningún conflicto. De hecho, ni siquiera hubo merge, porque la rama styled ya tenia todos los commits de la rama master.


**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
Si, causo conflictos, porque ambas ramas habían modificado las mismas líneas del archivo git-nuestro.md


**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
No, no causó ningún conflicto, porque el merge fue fast-forward, y los fast-forward no pueden causar nunca conflictos. Simplemente el puntero de la rama master, avanzó hasta el puntero de la rama styled.


**¿Qué comando o comandos utilizaste en el paso 25?**
git log --graph


**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
Si, podría ser fast-forward, porque la rama master y la rama title estaban en línea.


**¿Qué comando o comandos utilizaste en el paso 27?**
git reset HEAD~1


**¿Qué comando o comandos utilizaste en el paso 28?**
git checkout -- git-nuestro.md


**¿Qué comando o comandos utilizaste en el paso 29?**
git branch -D title


**¿Qué comando o comandos utilizaste en el paso 30?**
Primero un git reflog para obtener el hash del commit donde se hizo el merge. Después git reset --hard hash


**¿Qué comando o comandos usaste en el paso 32?**
Primero un git reflog para obtener el hash del primer commit, despues un git reset --hard hash.


**¿Qué comando o comandos usaste en el punto 33?**
Primero un git reflog para obtener el hash del commit donde se añadió el titulo, después un git reset --hard hash.


