# Git-Comand
Comandos Git

git --version (Nos da la version)
git help (Ayuda de Git)
git config --global user.name "Chico Cristiano" (Establesco el nombre del programador De manera global con git)
git config --global user.email "user@gmail.com" (correo con Github)
git config --global -e (editar usario y correo a->modificar esc una vez luego :wq! write quit !rapido)
git init (Inicia el repositorio)
git status(Informacion del estado del repositorio)
git add archivo.html  (anexar archivo al directorio de manera manual individualmente)
git add . (Anexar todos los archivos del proyecto al directorio)
git commit -m "Mensaje" (Creamos la fotografia del proyecto y archivos)
git log (Muestra el estado del proyeto y commits echos por autor)
git checkout -- .(Regresa el proyecto al commit anterior)
git branch (Rama en la que se trabaja actualmente)
git branch -m master main (Cambiar el nombre de la rama actual por main)
git config --global init.defaultBranch main (Establecer rama main por default al crear un repositorio git)
git reset archivo.extension (Eliminar el achivo del respositorio)
git commit -am "mensaje" (anexando al stage y tomando la fotografia con el commit)
git add *.extension (anexar al stage todo archivo con la extension ejemplo .html)
git add js/*.js (Anexar carpeta con el nombre despues del punto) o git add carpeta/ (anexa todo)
git status --short (Informacion de estado mas breve y corta)

/// comentarios de la clase
  archivo .gitkeep

/// creacion de los alias
git config --global alias.s status --short
/// configurar el alias
git config --global -e (Si se desea editar el alias)
git log --oneline (EL ESTADO DE LOS COMMITS MAS CORTO EN UNA LINEA)
git log --oneline --decorate --all --graph (Estado de los commits corto con una decoracion)
/// alias de l curso por Fernando
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
///
git diff (Ver las diferencias de los commits)
git diff --staged (ver las diferencias en el stage si estos fueron agrgados al stage)
git commit --amend -m "Mensaje de arreglo de commit anterior" (Arregla el mensaje del commit si se mando mal escrito del anterior commit)
git reset --soft HEAD^ (Eliminar el commit anterior se puede anexar numeros para eliminar el commit que se desea despues de la flechita)
git reset --mixed HASH (se debe agregar el hash del punto que nos da el git log  para regresar a ese punto y sacar del stage todo lo anexado hasta ese punto)
git reset --HARD HASH ( regresa a ese punto y elimina todo hasta ese momento)
git reflog (Referencia en orden de todo los commits que han pasado cronologicamente si se desea regresar se usa el git reset --hard HASH de la referencia)
git mv destruir-mundo.md salvar-mundo.md (RENOMBRAR LOS ARCHIVOS.EXTENSION primernombre nombrequequeremos)
git rm salvar-mundo.md (remover archivo mediante git)
git reset --hard (reaparece archivo eliminado)

//COMENTARIOS DE LA CLASE
.gitignore (carpeta/ en el archivo creado se pone la carpeta o archivos que no queremos guardar en git)

git branch nombrerama(Crear una rama para trabajar en otra linea de tiempo)
git checkout rama(para posicionarnos em la rama que trabajaremos)
git merge rama (unir las ramas)
git branch -d rama(Eliminar rama si no tiene un uso)
git branch -d rama -f(Eliminar rama de forma forzada)
git checkout -b rama(Crear rama y moverse automaticamente a la rama creada)
git tag version(Espara lanzar la version completa funcional de un proyecto)
git tag (ver los tag que se han lanzado)
git tag -d nombre (Borrar el tag)
git tag -a version -m "Mensaje"  (hacer un tag con anotacion y mensaje)
git tag -a version hash -m "mensaje" (Hacer un tag en un commit con su respectivo hash)
git show version (ver el tag detallado escribiendo el nombre de la version del tag)
git stash (Poner el codigo funcional a salvo Completo el proyecto)
git stash list (ver lista de stash)
git stash pop (Recuperar el proyecto funcional hasta ese momento y borra el stash)
git stash clear (Limpiar todos los stash)
git stash apply "stash@{2}" (Apliacar un stash previamente visto en el git stash list)
git stash drop "stash@{0}"   (Eliminar un stash)
git stash show "stash@{1}" (ver lo que sucedio en un stash en particular)
git stash save "Mnesaje" (Guardamos el stash seguro)
git stash list --stat  (ver la lsita de los stash mas detallado)
git rebase master (crenado espacio temporal a la rama master)
git rebase -i HEAD~4 (unir los commits despues del head la cantidad de commits a unir o hash para el modo de la ventana edicion se usa squash o la s por su sigla una ves echa la modificacion esc : Wq!)
// COMENTARIOS CLASE  git rebase -i HEAD~4(NUMERO DE COMMITS A HACER CAMBIOS SE PRESIONA R DE REWORD PARA CAMBIAR EL NOMBRE DE DICHO COMMIT )
git checkout -- README.md(REGRESAR AL COMMIT ANTERIOR DE UN ARCHIVO ESPECIFICO DESPUES DE LOS -- ARCHIVO.ALGO)
git rebase --continue  ( cuando hacemos un rebase interactivo y un  edit en commits para  guardar los cambios y continuar)
///github
local mente
git push --tags (para subir los tags al repositorio)
git pull origin main (traer los datos desde el Origen en Github especificando origen y rama)
git remote -v (a donde a punta en el github con su rama)
git clone mas url (clonar repositorio por terminal)
git push /git push origin rama (hacer un push al github especigficando rama con oringin rama)
git config pull.rebase true (configuracion para resolver conflictos de git y github al hacer commits en las misma lineas)
git pull --rebase  (Resolver conflictos del git a github)
git rebase --continue (Continuar con el rebase)
git config --global pull.rebase true (Configurar el global el rebase)
git fetch (registros de commit de actualizaciones echas em github)





