# Clase 01

## Markdown

# H1
## H2
### H3
#### H4
##### H5
###### H6

---

### Negrita

**Soy un texto en negrita**

### Cursiva

*Soy un texto en cursiva*

---

### Lista ordenadas

1. Item
2. Item
3. Item

### Lista desordenada

* Item
* Item
* Item

--- 

    git --version #esto me muestra la versión

```bash
    git --version #esto me muestra la versión
```

```php
$variable = "Hola
```

```js
function sumar(a, b) {
    return a + b
}
```

backtick = ALT + 96
https://elcodigoascii.com.ar/

--- 

## COMANDOS CONSOLA

* ls : Listar directorios
* cd : Cambiar directorios
* cd .. : Volver para atrás un directorio
* cd ../.. : Vuelve 2 directorios para atrás
* touch : Creo archivos vacios
* mkdir : Creo directorios

---

## GIT

    git --version

## Hacer la configuración global de GIT

    git config --global user.name "Maximiliano Principe"
    git config --global user.email "mlapeducacionit@gmail.com"

## Para visualizar las configuraciones

    git config --get-regexp user

## Crear un repositorio

    git init

## Areas en GIT

* Working Directory (WD): Vamos a tener todos los archivos de proyecto

* Staging Area (SA): Area intermedia de confirmación de cambios

* Local REPO - Cajita de Fotos - Commits: Los commits que voy haciendo

## Para saber el estado de los archivos en WD y SA

    git status

## ¿Cómo sacamos la foto (Commmit)?
Una vez confirmados los cambios (Los archivos están en el SA)

    git commit -m "Mensaje"

## Para ver las diferencias entre el WD y el Local Repo

    git diff

## Para ver las fotos o commits del repositorio

    git log
    git log --online