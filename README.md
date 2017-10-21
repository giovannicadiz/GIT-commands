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
