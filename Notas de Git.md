# Sintaxis y escritura Markdown
Referencia:
[GitHub Pages](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
Para crear un encabezado, agrega entre uno y seis símbolos # antes del encabezado del texto. El número de # que use determinará el tamaño del encabezado.

* Autor: Javier Morrón
* Contacto: [Moneytoday.es](https://moneytoday.es/contacto)

```
# The largest heading
## The second largest heading
###### The smallest heading
```
# The largest heading
## The second largest heading
###### The smallest heading

Para formatear código o texto en su propio bloque distintivo, usa comillas triples.
Some basic Git commands are:
```
git status
git add
git commit
```
## Estilos de texto
Texto en negrita
```
**texto en negrita**
````
**Esto es un texto en negrita**
texto en cursiva
```
*Texto en cursiva*
```
*Esto es un texto en culsiba*
Tachado
```
~~texto tachado~~
```
~~Esto es un texto tachado~~
Cursiva en negrita y anidada
```
**Este texto es _extremadamente_ importante** 
```
**Este texto es _extremadamente_ importante**
Todo en negrita y cursiva
```
***Todo este texto es importante***
```
***Todo este texto es importante***
Subscript
```
<sub>Se trata de un texto de subíndice</sub>
```
<sub>Se trata de un texto de subíndice</sub>

# Entrecomillado de texto
```
> Cita de texto
```
> Es mejor hecho que pefecto :ok_hand:
---
## Emojis en Markdown :smiley: :thumbsup: :star: :star::star::star::star:
**Lista completa de emojis en Markdown con sus respectivos shortcodes**
Refrencia:
[tutorialmarkdown](https://tutorialmarkdown.com/emojis).

## Clonar repositorio remoto ![Referencia:Remoto](https://git-scm.com/book/es/v2/Fundamentos-de-Git-Trabajar-con-Remotos)

Para ver los remotos que tienes configurados, debes ejecutar el comando git remote. Mostrará los nombres de cada uno de los remotos que tienes especificados. Si has clonado tu repositorio, deberías ver al menos origin (origen, en inglés) - este es el nombre que por defecto Git le da al servidor del que has clonado:
```
git clone https://github.com/schacon/ticgit

```
También puedes pasar la opción -v, la cual muestra las URLs que Git ha asociado al nombre y que serán usadas al leer y escribir en ese remoto:
```
$ git remote -v
origin	https://github.com/schacon/ticgit (fetch)
origin	https://github.com/schacon/ticgit (push)
```
***Añadir Repositorios Remotos***

git remote add [nombre] [url]:

Ejemplo:
```
git remote add pb https://github.com/paulboone/ticgit

# Para cambiar de repositorio remoto 
git remote set-url origen https://github.com/paulboone/ticgit


```


# Comandos de Git
```
git init                                                            # Crea un nuevo repositorio de Git

git status                                                          # Muestra el estado actual de la working directory y de la staging area

git status -s -b                                                    # Muestra con detalles el estado de nuestro directorio y las ramas 

git log                                                             # Para ver todo los cambias que hemos hecho

git log --oneline                                                   # información del registro de commit más clara

git log --oneline --decorate --all --graph                          # información de los commit y las ramas

git checkout -- .                                                   # Nos va permitir recuperar el último commit
 
git add mi_fichero.txt                                              # Adiciona el fichero con el nombre.txt

git add .                                                           # Sube todos los fichero al repositorios de git 

git add -u                                                          # Altualiza el directorio

git add "*.md"                                                      # agreda al repositorio todos los fiche md sin importal la ubicación

git commit -m "Fiche de ejemplo de vim"                             # Para relizar un comentario 

git commit --amend -m "Cambia la descricion de commit"              # Para cambiar la descrición de commit

git checkout -- .                                                   # Recupera el último commit

git  push                                                           # Cargar contenido del repositorio local a un repositorio remoto

git  pull                                                           # Extraer y descargar contenido desde un repositorio remoto y actualizar al instante                                        
```
## Trabajo con ramas

El comando **git branch** tiene más funciones que las de crear y borrar ramas. Si lo lanzas sin parámetros, obtienes una lista de las ramas presentes en tu proyecto:
```
$ git branch
  iss53
* master
  testing
```
Para crear una **nueva rama** y saltar a ella, en un solo paso, puedes utilizar el comando **git checkout con la opción -b:**
```
$ git checkout -b iss53
Switched to a new branch "iss53"
Esto es un atajo para:
$ git branch iss53
$ git checkout iss53
```
Refeencia:


![Procedimientos Básicos para Ramificar y Fusionar](https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Procedimientos-B%C3%A1sicos-para-Ramificar-y-Fusionar).



![Gestión de Ramas](https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Gesti%C3%B3n-de-Ramas).









