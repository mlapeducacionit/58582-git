# CLASE 02

## .gitignore
Es un archivo. Me permite descartar archivos. Qué git ignore el archivo.
Se crea normalmente en el directorio raíz del proyecto

## .gitkeep
Le permite a git ver carpetas vacías y versionarlas

## GIT BRANCH (RAMAS)

### Crear rama

    git branch <nombre-rama>
    git branch rama-dev
### Listar ramas

    git branch

### Cambiarme de rama

    git switch <nombre-rama>
    git switch rama-dev

### Borramos una rama

    git branch -d <nombre-rama>
    git branch -d rama-dev

## GIT MERGE: Funsión de ramas

**IMPORTANTE:** Tengo que estar en la rama en al cual quiero traerme los cambios. Si quiero traerme lo rama-branches. Tengo que estar en master y ejecutar el git merge.

    git merge <rama-que-me-quiero-traer>
    git merge rama-branches

### TIPO DE FUSIONES (MERGE)

Fast-forward: (La fusión va a ser automática) No hay conflicto
Recursiva: (Unión automática) No hay conflicto
Manual: (No va poder resolver en forma automática) O sea hay conflictos. 

## GIT LOG

    git log --help

    git log --oneline --decorate --all --graph

