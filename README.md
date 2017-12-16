# MIS COMANDOS GIT #

Este es un documento para llevar documentado los commandos git que voy aprendiendo a lo largo de los proyectos.


### Que vamos a encontrar en este repositorio ? ###

* Breve resumen
* Version

### Contribuciones a esta guia ###

* Proyectos
* Revision de código de otros repositorios
* Otras guias


### Add y commit ### 

Registrando cambios de directorio de trabajo al Storage (index) => add
Incluir los cambios en el HEAD local => commit
Enviar los cambios al repositorio remoto => push

>
> git add .
> git add <nombre de archivo>

Omitiendo add
>
> git commit -am "comentario"

> git push origin master
> git push origin <nombre del branch>


### Actualizar repositorio ##
git pull

$cuando tienes cambios locales y necesitas actualizr el repo con archivos remotos
git stash
git pull
git stash pop

### Comados GIT para Ramas ###

$Crear una nueva rama
> git branch <nombre de la nueva rama>
> git checkout -t origin/feature/otra
Realizar cambios

>
> git add .
> git commit -m "mesnaje"
> gui push origin feature/otra

$Ver ramas locales
git branch

$Ver ramas remotas
git branch -a

$Obtener Ramas remotas
git pull
git remote show origin
git checkout --track origin/serverfix
git checkout -t origin/serverfix
$Otro ejemplo
git checkout --track se featuring/seleccion origin/featuring/seleccion

$Cambiando de rama
git checkout master

### TAG ###

$Verificando Tags
git tag

$Añadiendo un nuevo TAG
git tag -a V1.0 -m "la primera version 1.0"

$Veindo un TAG en especifico
git show 1.0

$Publicando el tag en el repo remoto
git push origin v1.0

