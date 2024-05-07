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

Una rama tambien sirve para dividir funciones de trabajo en un desarrollo grupal.
## Conflictos
Los conflictos son problemas que aparecen al tratar de fusionar dos ramas, por ejemplo un error de espacios. En Visual Studio Code tiene una herramienta donde podemos decidir que hacer con eso y asi arreglarlo. Tambien se puede hacer desde consola

## Comandos
- ### git branch
sirve para listar las ramas:

`git branch`

tambien sirve para crear ramas y solo tiene una modificacion:

`git branch Nombrerama`

- ### git switch
sirve para cambiar de rama, aparte si añadimos -c podemos crear y movernos a la rama: 

`git switch Nombrerama`
`git switch -c Nombrerama2`

- ### git checkout
Sirve tambien para cambiar de rama pero se usa mas el switch desde 2019:

`git checkout`

- ### git merge
Este comando sirve para fusionar dos ramas, o la rama secundaria al MAIN, pero OJO tenemos una condicion, tenemos que estar "parados" en la rama que queramos que se actualice con la otra.

`git merge RamaX`

- ### git branch -d o --delete
Nos sirve para eliminar una rama cualquiera.

`git branch -d NombreRama`
`git branch --delete NombreRama`

- ### git merge header --no--ff
sirve para verlo como arbolito y te da un mensaje en consola.

- ### git log --graph --oneline

Muestra un historial de commits de manera gráfica y compacta. Cada commit se representa en una sola línea, mostrando únicamente su identificador único abreviado. El --graph agrega una representación visual de las ramas y fusiones del proyecto.

# Clase 3
## ¿Que es GitHub?
Es el proveedor de repositorios en la nube para hospedar codigo mas utilizado en la actualidad.

## Los SSH
Es un protocolo de red que permite a los usuarios acceder de forma segura a una computadora remota o servidor a través de una conexión encriptada. 

## Comandos
- ### git remote add
sirve para conectar un repositorio local con uno remoto.

`git remote add (ALIAS) (SSH o HTTPS)`

El alias puede ser cualquier nombre para referirnos al repositorio en futuras ocasiones.

- ### git remote add origin
como el anterior comando solo que usamos un https sin SSH con url.

`git remote add origin https://...`
- ### git remote -v
Solo nos da una lista detallada de repositorios remotos enlazados con el repositorio local.

- ### git clone
sirve para clonar un repositorio remoto a nuestra maquina para trabajarlo
`git clone codigoSSH`

- ### git fetch
Sirve para traer los cambios de tu repositorio remoto al local, pero no se aplicaran cambios. 

`git fetch ALIAS`
- ### git branch -a
son tokens pero con informacion personal.

- ### git push
Envia cambios al repositorio remoto, se necesita dos parametros.

- Primero el alias del repositorio remoto.
- Segundo nombre de la rama.

`git push (ALIAS) (NombreRama)`
