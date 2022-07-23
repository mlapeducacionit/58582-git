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

## GIT MERGE: Funsión de ramas

**IMPORTANTE:** Tengo que estar en la rama en al cual quiero traerme los cambios. Si quiero traerme lo rama-branches. Tengo que estar en master y ejecutar el git merge.

    git merge <rama-que-me-quiero-traer>
    git merge rama-branches

## GIT LOG

    git log --help

    git log --oneline --decorate --all --graph