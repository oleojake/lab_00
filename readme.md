# Laboratorio de Git
Este laboratorio tiene como objetivo que practiques los comandos básicos de Git. Para ello, deberás crear un repositorio en local y subirlo a GitHub. Luego, deberás crear una rama, hacer un merge y resolver los conflictos que se presenten si fuera el caso.

## Entrega
La entrega del laboratorio se realizará pegando abajo de está página el enlace correspondiente a tu repositorio de GitHub.

**IMPORTANTE: El repositorio debe contener un archivo README.md con la descripción de lo qué se ha realizado en el laboratorio, si quieres puedes añadir capturas de pantalla para explicar cómo has realizado el laboratorio.**

## Requisitos
Tener instalado Git en tu computadora.
Tener una cuenta en GitHub.

## Objetivos
### 1. Crear un repositorio en local
* Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
* Crea una carpeta con el nombre del repositorio.
* Ingresa a la carpeta que acabas de crear.
* Inicializa el repositorio de Git.

<h3 style="color:orange">✔️ Pasos ejecutados</h3>

```
git init
```

### 2. Subir el repositorio a GitHub
* Crea un nuevo repositorio en GitHub.
* Copia el URL del repositorio que acabas de crear en GitHub
* Conecta tu repositorio local con el repositorio en GitHub.
* Verifica que la conexión se haya establecido correctamente.

<h3 style="color:orange">✔️ Pasos ejecutados</h3>

```
git remote add origin git@github.com:oleojake/lab_00_git.git
git branch -M main
git push -u origin main
```

### 3. Hacer un commit y un push
* Crea un archivo en la carpeta del repositorio.
* Añade el archivo al staging.
* Crea un commit con un mensaje descriptivo.
* Sube los cambios al repositorio en GitHub.

<h3 style="color:orange">✔️ Pasos ejecutados</h3>

```
git add .
git commit -m "first commit"
git push
```

### 4. Crear una rama
* Crea una rama nueva llamada "development".
* Cambia a la nueva rama.
* Realiza algunos cambios en el archivo que creaste.
* Añade y haz un commit con los cambios en la rama "development".
* Sube los cambios a Github.

<h3 style="color:orange">✔️ Pasos ejecutados</h3>

```
git branch development
git checkout development
git commit -am "modificando el fichero index"
```

### 5. Hacer un merge
Vuelve a la rama "main".
Haz un merge de la rama "development" a la rama "main".
Si no hay conflictos, los cambios realizados en la rama "development" se incorporarán a la rama "main".
Hax un push de los cambios al repositorio en GitHub.
*La rama principal de nuestro repositorio puede ser "main" o "master" según la hayamos nombrado.*

<h3 style="color:orange">✔️ Pasos ejecutados</h3>

```
git checkout main
git merge development
git push
```