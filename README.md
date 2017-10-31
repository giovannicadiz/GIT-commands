 ![Logo Git](https://github.com/giovannicadiz/GIT-commands/blob/master/img/logo-git.png)

Basic commands in [Git](https://es.wikipedia.org/wiki/Git)
===============

## INSTALAR GIT

### CONFIGURAR HERRAMIENTAS
#### Configura la información para todos los repositorios locales.

* Establece el nombre que desea esté anexado a sus transaccionesde commit:
```[git]
git config --global user.name "[name]"
```

* Establece el e-mail que desea esté anexado a sus transacciones de commit:
```[git]
git config --global user.name "[name]"
```

* Habilita la útil colorización del producto de línea de comando:
```[git]
git config --global color.ui.auto
```

### CREAR REPOSITORIOS
#### Inicia un nuevo repositorio u obtiene uno de una URL existente

* Crea un nuevo repositorio local con el nombre especificado:
```[git]
git init [project-name]
```

* Descarga un proyecto y toda su historia de versión:
```[git]
git clone [url-project]
```

### EFECTUAR CAMBIOS
#### Revisa las ediciones y elabora una transacción de commit

* Enumera todos los archivos nuevos o modificados que se deben confirmar:
```[git]
git status
```

* Muestra las diferencias de archivos que no se han enviado aún al área de espera:
```[git]
git diff
```

* Toma una instantánea del archivo para preparar la versión
```[git]
git add [name fiele]
```

* Muestra las diferencias del archivo entre el área de espera y la última versión del archivo
```[git]
git diff --staged
```

* Mueve el archivo del área de espera, pero preserva su contenido
```[git]
git reset [name file]
```

* Registra las instantáneas del archivo permanentemente en el historial de versión:
```[git]
git commit -m "[descriptive message]"
```

### CAMBIOS GRUPALES
#### Nombra una serie de commits y combina esfuerzos ya culminados

* Enumera todas las ramas en el repositorio actual:
```[git]
git branch
```

* Crea una nueva rama:
```[git]
git branch [branch name]
```

* Cambia a la rama especificada y actualiza el directorio activo:
```[git]
git checkout [branch-name]
```

* Combina el historial de la rama especificada con la rama actual:
```[git]
git merge [branch]
```

* Borra la rama especificada:
```[git]
git branch -d [branch-name]
```


### NOMBRES DEL ARCHIVO DE REFACTORIZACIÓN
#### Reubica y retira los archivos con versión

* Borra el archivo del directorio y pone en el área de espera el archivo borrado.
```[git]
git rm [file]
```

* Retira el archivo del control de versiones, pero preserva el archivo a nivel local.
```[git]
git rm --cached[file]
```

* Cambia el nombre del archivo y lo prepara para commit
```[git]
git mv [file-original]file-renamed[]
```

### SUPRIMIR TRACKING
#### Excluye los archivos temporales y las rutas

```[git]
*.log
build/
temp-*
```
* Un archivo de texto llamado **gitignore** suprime la creación accidental de versiones de archivos y rutas que concuerdan con los patrones especificados

* Enumera a todos los archivos ignorados en este proyecto
```[git]
git ls-files --other --ignored --exclude-standard
```

### GUARDAR FRAGMENTOS
#### Almacena y restaura cambios incompletos

* Almacena temporalmente todos los archivos tracket modificados
```[git]
git stash
```

* Restaura los archivos guardados más recientemente
```[git]
git stash pop
```

* Enumera todos los sets de cambios en guardado rápido
```[git]
git stash list
```

* Elimina el set de cambios en guardado rápido más reciente
```[git]
git stash drop
```

### REPASAR HISTORIAL
#### Navega e inspeciona la evolución de los archivos de proyecto

* Enumera el historial de la versión para la rama actual
```[git]
git log
````

* Enumera el historial de versión para el archivo, incluidos los cambios
```[git]
git log --follow[file]
```

* Mustra las diferencias de contenido entre dos ramas.
```[git]
git diff[first-branch] ... [second-branch]
```

* Produce metadatos y cambios de contenido del commit especificado
```[git]
git show [commit]
```

### REHACER COMMITS
#### Borrar errores y elabora historial de reemplazo

* Deshace todos los commits después de **[commit]** ,preservando los cambios localmente
```[git]
git reset [commit]
```

* Desecha todo el historial y regresa el commit especificado
```[git]
git reset --hard [commit]
```

### SINCRONIZAR CAMBIOS
#### Registra un marcador de repositorio e intercambiar historial de versión

* Descarga todo el historial de marcador del repositorio
```[git]
git fetch [bookmark]
```

* Combina la rama del marcador con la rama actual
```[git]
git merge [bookmark]/[branch]
```

* Carga todos los commit de la rama local GitHub
```[git]
git push [alias][branch]
```

* Descarga el historial del marcador e incorpora cambios
```[git]
git pull
```
