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

> Sin el sobrerito (acento circunflejo). Descarta los commit de los bordes

    git cherry-pick <hash>..<hash>
    git cherry-pick 57f7d4b..e061800

# GIT RESET

Hay 3 tipos de resets

## GIT RESET SOFT
Al ejecutar el comando lo que hace git reset soft es eliminar los commits pero me deja los cambios que tienen dentro en el staging area (Index). Area de confirmación.

    git reset --soft <hash>

## GIT RESET MIXED (POR DEFECTO)
Al ejecutar el comando lo que hace git reset mixed es eliminar los commits pero me deja los cambios que tienen dentro commits en el working directory. Area de trabajo.

    git reset <hash>
    git reset --mixed <hash>

## GIT RESET HARD (MUY PELIGROSO)
Lo que hace es eliminar los commits y descartar su contenido. O sea pierdo la información dentro de los commits reseteados.

    git reset --hard <hash>

# GIT STASH

## Creo un stash

    git stash

## Listar stash

    git stash list

## Recuperar el ùltimo stash

    git stash pop

## Recuperar un stash en particular

```sh
    git stash apply # último stash
    git stash apply stash@{1}
```
## Borro un stash en particular

```sh
    git stash drop # último stash
    git stash apply stash@{1}
```

## Aplico un stash en nueva rama

    git stash branch <nombre-rama>
