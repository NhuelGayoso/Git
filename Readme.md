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

 * UNTRACKED: Significa que el archivo no esta siendo seguido por GIT, sabe que existe pero no tiene ideade lo que pasa dentro del archivo . No lo controla Git 
 * STAGED o index: 
 * UNMODIFIED:
 * MODIFIED:

## Zona/area virtual  de git

 * Working Directory (WD)
 * Staging Area (SA)
 * Local Repo (LR)

## GIT STATUS
¿Que hace? Controla en que estado estan los archivos y en que zona o area de la estructura virtual estan los archivos

```sh
git status
```