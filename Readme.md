# Curso Git: Desarrollo Colaborativo

# Configurando Git

> Agrego el usuario
```sh
git config --global user.name "Nahuel Gayoso" # Global para todos los repositorios con mi usuario de windows

git config --local user.name "Nahuel Gayoso" # Local (este comando se tiene que ejecutar cuando ya tengo un repositorio de git)
```

> Agrego el mail
```sh
git config --global user.email "gayosonahuel@hotmail.com" # Global para todos los repositorios creados con mi usuario de windows

git config --local user.email "gayosonahuel@hotmail.com" # Local para este unico repositorio (Este comando se tiene que ejecutar cuando ya tengo un repositorio de git)
```

> Para verificar las configuraciones hechas

```sh
git config --global --get-regexp user
```

## Inicializar un repositorio GIT

```sh
git init # Va crear en la carperta del proyecto una carpeta '.git'en el directorio (carpeta)
```

**IMPORTANTE**: No hay que borrar ni alterar manualmente los archivos dentro de la carpeta '.git'. Solo trabaja git sobre esa carpeta, no nosotros

```sh
clear # limpia consola (ctrl + L)
```

## Estados de los archivos
Los archivos en git pueden tener diferentes estados.

 * UNTRACKED: Significa que el archivo no esta siendo seguido por GIT, sabe que existe pero no tiene ideade lo que pasa dentro del archivo . No lo controla Git.
   
 * STAGED o index: (Prefoto) Archivos que estan preparados para un commit (sacar la foto) el snapshot y perservar los cambios hechos de mi codigo fuente.
  
 * UNMODIFIED:
  
 * MODIFIED:

## Zona/area virtual  de git

 * Working Directory (WD): Area de trabajo donde se van agregando  o quitando  los archivos  de mi proyecto
  
 * Staging Area (SA): (Pre foto): Area  de control de cambio , se agregan los cambios  para darle seguiendo.

 * Local Repo (LR): (foto) Area de validacion de cambios , donde se registran  las modificaciones realizadas dentro del proyecto.

## GIT STATUS
¿Que hace? Controla en que estado estan los archivos y en que zona o area de la estructura virtual estan los archivos

```sh
git status
```

## GIT ADD
Me permite marcar los archivos(pre foto) que considero listos para crear(foto) el commit(snapshot)

```sh
git add <nombre-archivo1> <nombre-archivo2> <nombre-archivo3> 
git add Readme.md

# Agrega todo a la zona/area de (SA)
git add .   
```

## GIT LOG
Me muestra la lista de commit (la timeline de fotos que tengo). Cada commit tiene un hash (el dni del commit (foto))

> Version larga
```sh
git log    
```

> Version corta
```sh
git log --oneline
```