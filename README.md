# Recordatorio personalizado sobre el uso de Git y GitHub :octocat:

## Temario 
:pencil:
1. [Comenzando nuestra área de trabajo](#1-comenzando-nuestra-área-de-trabajo)
2. [Identificandonos](#2-identificandonos)
3. [Examinando el historial y los estados](#3-examinando-el-historial-y-los-estados-log-status-show-reflog)
   * [log](#git-log)
   * [status](#git-status)
   * [show](#git-show-v100)
   * [reflog](#git-reflog)
4. [Trabajando con Git](#4-trabajando-con-git-add-mv-reset-rm-commit)
   * [add](#git-add----)
   * [mv](#git-mv-heroeshtml-villanohtml)
   * [reset](#git-reset-xml) 
   * [rm](#git-rm-archivo)
   * [commit](#git-commit--m-nombre)
5. [Ignorando Archivos](#5-ignorando-archivos)
6. [Trabajando con Ramas](#6-trabajando-con-ramas-branch-checkout-diff-tags-rebase-merge)
   * [branch](#git-branch)
   * [checkout](#git-checkout-nombre_rama)
   * [diff](#git-diff)
   * [tags](#git-tag)
   * [rebase](#git-rebase-master-nombre_rama)
   * [merge](#git-merge-nombre_rama)
7. [Trabajando colaborativamente](#7-trabajando-colaborativamente-fetch-pull-push)
   * [fetch](#fetch)
   * [pull](#pull)
   * [push](#push)
8. [Shortcuts](#8-shortcuts-atajos)
9. [GITHUB](#9-github)

## Si estas retomando todo lo que es git o te ha ocurrido algun error, consulta la seccion de casos.

:eyes:

[Ir a Casos](https://github.com/oscar8232003/Materias/blob/master/Git/casos.md#casos)

![Diagrama explicado](https://image.ibb.co/gor8ff/Diagrama-en-blanco.png)

## 1 Comenzando nuestra área de trabajo.
#### git help 
> Sirve para ver información de ayuda en git pero general.
#### git help comando 
> Sirve para ver la información de ayuda de un comando en específico.
#### git clone  
> Clona un repositorio en una carpeta específica.
#### git init   
> Inizializa un repositorio nuevo.

[Volver al inicio](#temario)

## 2 Identificandonos
:person_with_blond_hair::woman:
#### git config --global user.name "Oscar" 
> Sirve para identificarse con un nombre.
#### git config --global user.email "correo@gmail.com" 
> Sirve para identificarse con un email.
#### grit config --global -e 
> Sirve para ver la información global de nuestro repositorio(si quieren salir es :q sin guardar y :w con guardar).

[Volver al inicio](#temario)

## 3 Examinando el historial y los estados (log, status, show, reflog)
:coffee:
#### git log 
> Muestra los commit hechos desde el último hasta el más reciente.
#### git log --oneline 
> Muestra los logs pero con commit cortos y los nombres.
#### git status 
> Muestra en qué branch estamos trabajando, si hay archivos en rojo esos están modificados o fuera del stage y si están en verde es porque ya están en el stage para poder hacer un commit.
#### git show v1.0.0 
> Muestra información de un tag.
#### git reflog 
> Sirve para ver el historial de logs, esta todo lo que se ha hecho, sirve para reestablecer versiones que no se encuentran visibles en el log. 

[Volver al inicio](#temario)

## 4 Trabajando con Git (add, mv, reset, rm, commit).
:package:
#### git add -- . 
> Agrega todos los elementos a la carpeta git con el ..
#### git add *.png 
> Agrega todos los elementos a la carpeta pero con extensión .png.
#### git add img/ 
> Agrega todos los elementos de la carpeta img.
#### git add "*.txt" 

[Volver al inicio](#temario)

## 8 Shortcuts (Atajos!).
:thumbsup:
#### git config --global alias.nombre_alias "comando" 
> Creamos un shortcut personalizado.
#### git config --global -e  
> Sirve para ver las configuraciones globales(:q para salir).
#### git config --global alias.lg “log --oneline --decorate --all --graph”  
> Crea un comando que al digitar lg es la abreviación de toda la sentencia que está entre comillas, este comando sirve para reemplazar el log.
#### git config --global alias.s “status -s -b” 

[Volver al inicio](#temario)

## 9 GITHUB.
:kissing_heart::octocat:
#### Primero hay que crear un nuevo repositorio dentro de github.
#### Aparecerán estas 2 líneas, el remote add origin es para dejar puesto las credenciales del repositorio.
#### git remote add origin https://github.com/oscar8232003/udemy-heroes.git.
#### git push -u origin master (origin es dentro del origen y master es hacia la rama master).
#### Para verificar si esta todo correcto digita.
#### git remote -v.
#### Si tienes problemas con las credenciales digita git credential-manager uninstall y desinstala el manager de credenciales e install si lo quieres volver a instalar.
#### El fork es para copiar el repositorio a tu repositorio y hacer los cambios que quieras, es como clonar un proyecto pero este lo sube automáticamente a tu repo.

#### git push --tags 
> Sirve para subir los tags.
#### git push 
> Sube todos los cambios de mi repo local al repo remoto.
#### git push :rama-eliminada 
> Se elimina la rama de git local y después se manda a el repo remoto.
#### git pull 
> Copiamos los cambios del repositorio remoto al repositorio local.
#### git pull --all 
> Si hay problemas con el pull, se le pone el --all.
#### git fetch 
> Organiza los cambios que se le hicieron al proyecto, es decir, si hay cambios en ambos repositorios, el fetch sirve para que se cree una rama con los cambios del repositorio remoto.
#### git clone https://github.com/oscar8232003/udemy-heroes.git 
> Vamos a la carpeta donde queremos poner el proyecto navegando por la terminal y ponemos el comando.
#### git clone https://github.com/oscar8232003/udemy-heroes.git demo-10 
> Vamos a la carpeta donde queremos poner el proyecto, ponemos el comando y lo pone con el nombre demo 10.
#### git push origin rama_destinataria 
> Hace un push con el contenido a la rama_destinataria.

[Volver al inicio](#temario)
