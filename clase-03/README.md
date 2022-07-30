# Clase 03

## GIT PULL
Me sirve para traerme los cambios (Los nuevos commits) de la rama que seleccione.

    git pull <rama-remota> <rama-local>

## GIT FETCH
Me sirve para traerme la metadata (Me actualiza la carpeta .git con los cambios que sufrieron las ramas remotas)

    git fetch <rama-remota> <rama-local>
    git fetch --all

## GIT CHERRY PICK
Me permite seleccionar un commit o varios y llevarlos a la rama que necesite.
** Importante: ** Estando en la rama que espero traerme los commits. O sea si quiero traerme a master los commits, tengo que estar posicionado en la rama master

> Me llevo a otra rama el commit 

    git cherry-pick <hash>

> Me llevo a otra rama los commits seleccionados

    git cherry-pick <hash> <hash> <hash>

> Me llevo a otra rama rangos de commits

    git cherry-pick <hash>^..<hash>
    git cherry-pick 57f7d4b^..e061800

> Sin el sobrerito. Descarta los commit de los bordes

    git cherry-pick <hash>..<hash>
    git cherry-pick 57f7d4b..e061800