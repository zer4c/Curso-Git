# CURSO GIT
# CLASE 1
## Primeros pasos con git y Markdown
para iniciar el curso tenemos que instalar el programa de **GIT**, que es un controlador de versiones en un repositorio.
### Repositorio
Un repositorio es un tipo de almacenamiento centralizado para administrar cambios de codigo fuente.
## COMANDOS:
- ### git init
Sirve para iniciar un nuevo repositorio local, teniendo en cuenta que la carpeta esta vacia y estemos en la raiz del directorio:

`git init`

si no tenemos una carpeta creada simplemente hacemos:

`git init Nombre_Repositorio`
- ### git add
Sirve para que git movilice un archivos o varios al area temporal (Stage area).

`git add archivo.x`
- ### git status
Sirve para ver en que estado estan los ficheros actualmente.

`git status`
- ### git commit
Guarda un fichero al repositorio local, hace un ***commit*** que es como un punto de guardado y te pedira añadir un mensaje describiendo los cambios realizados.

`git commit archivo.x`

>Tambien podemos poner el mensaje directamente desde consola con:  
`git commit -m "Descripcion"`
- ### git log
Sirve para mostrar el historial de los commits realizados.

`git log`
## Markdown
Es un lenguaje de marcado que usan varias aplicaciones y entre ellas GitHub; su extension es md. Referencias de sintaxis.
- [Sintaxis Markdown](https://tutorialmarkdown.com/sintaxis)

- [Guia de Markdown de GitHub](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
# Clase 2
## ¿Que es una rama?
Son una snapshot de la division del estado del codigo, es un nuevo apuntador hacia una de las confirmaciones. Sirven para un desarrollo en equipo mas eficiente.

Se puede crear la rama de la siguiente manera: 

`git branch NombreRama`

Una buena practica es poner de nombre la funcion que se esta desarrollando.
## Comandos
### git branch
sirve para listar las ramas:

`git branch`
### git switch
sirve para cambiar de rama: 

`git swtich Nombrerama`

### git checkout
Sirve para cambiar de rama:
crear -b homepage
`git checkout`
### git merge
### git branch -d o --delete
### git merge header --no--ff
sirve para verlo como arbolito y te da un mensaje
### git log --graph --oneline
## fusionar ramas
## conflictos
investigar si tienen los mismos ID por la creacion de ramas
# Clase 3
## ¿Que es GitHub?
### perfil
### colaboradores
solo dura un mes
###
## Comandos
### git remote add origin
solo https sin ssh con url
### git remote -v
### ls -al -/ssh
### 
## los SSh
### git prune origin main
### git clone
### git fetch
### git branch -a
son tokens pero con informacion personal.

