# GITHUB-COMMAND
Comandos GitHub básicos

## Acceder a GitHub
#### Guarda el nombre con el que apareceremos al subir los archivos
```
git config --global user.name "nombre"
```
#### Dirección de correo que nos identifica
```
git config --global user.email correo@
```

#### Esta herramienta nos sirve para comparar diferencias entre ficheros
```
git config --global diff.tool tkdiff        
```
#### Donde voy a guardar las crendenciales de repositorios remotos
```
git config --global credential.helper manager      
```
#### Elegir editor de trabajo en este caso nano
```
git config --global core.editor nano        
```
## Commits y herramientas básicas 
#### Inicializar repositorio
```
git init 				     
```
#### Crear fichero readme o cualquier otro
```
echo "#Primera línea de un fichero readme.dm" > readme.md	
```
#### Ver archivos dentro de la carpeta
```
ls -lart
ls -l
```
#### Añadir ficheros al repositorio
```
git add * or git add nombreFichero
```
#### Comprobar estado del fichero
```
git status
```

#### Añadir revisiones del proyecto
```
git commit -m "nombre del commit"
```

#### Ver commits
```
git log --oneline
```
#### Modificar un fichero de texto
```
less nombreFichero
```
#### Para ignorar ficheros tenemos que crear el fichero gitignore
```
nano .gitignore -> Dentro de este fichero si por ejemplo tenemos archivos .tmp, dentro de ese fichero debemos de poner *.tmp
```
#### Comparar archivos para ver las modificaciones que se han realizado a un archivo modificado
```
git diff
```
#### Comparar archivos en caso de que le hayamos hecho un git add 
```
-git diff --staged
```

#### Muestra en la consola las diferencias entre los archivos
```
git difftool  -> Para una mejor visualización necesitaremos la herramienta tkdiff  se almacena dentro de la ruta GIT/usr/bin
```
#### Muestra la diferencias entre los archivos almacenados en el staged changes
```
git diff --cached
```
#### Borrar fichero
```
rm nombreFichero
```
#### Mover renombrar o mover ficheros
```
git mv nombreFichero <ruta>
```
#### Renombrar
```
git mv nombreFichero nombreFichero1
```
#### Mover
```
git mv nombreFichero ruta
```
#### Mostrar informacion en colummnas de los commits tanto el hash, el nombre, el tiempo y el nombre.
```
git log --pretty=format:"%h %an %ar - %s"
```
#### Mostrar información de un commit
```
git show <hashDelArchivo>
```
#### Conectarse a un repositorio
```
git remote add origin <rutaDeElProyectoDeGit>
```
#### Recuperar archivos del repositorio
```
git fetch origin
```
#### Descargar archivos en origen master
```
git pull origin master -> Esto se descarga en tu propia rama de master
```
#### Descargar archivos en el directorio actual
```
git clone <url> .
```
#### Subir archivos 
```
git push 
```
#### Recuperar un fichero que le hemos hecho git add a su versión anterior
```
git reset HEAD <nombreDelArchivo>
```

#### Este comando combina los efectos de git checkout como el git reset en un solo comando, lo cuál hace que el fichero, el resultado es que se eliminan lo ficheros del staging area y del working directory de tal forma volvemos a los msmos contenidos que estaban presentes en el último commit
```
git reset --hard HEAD~1
```
## CHECK OUT
#### Traer archivos de la rama
```
git checkout master
```
#### Traer un archivo o un grupo de archivos de la rama master
```
git checkout --master
```
#### Traer archivos de una revisión concreta
```
git checkout HEAD fichero
```
#### Traer fichero de un commit anterior 
```
git checkout HEAD~1 fichero  En caso de que queramos traer anteriores a este debemos sustituir el 1 por 2 o 3 según nos parezca
```
#### En caso de algún problema (Borrado, modificado,etc..)
```
git checkout HEAD -- .   //Esto realmente recupera todo de la versión anterior en el directorio que estamos situados
```
#### Deshacer cambios
```
git revert <hashDelCommit>
``` 
#### Deshacer todos los cambios en una franja 
```
git revert HEAD...HEAD~2 --no-edit
```

#### No sé para que sirve pero ahí está
```
git pull origin master –allow-unrelated-histories
```

## RAMAS O BRANCH
#### Crear una nueva rama
```
git branch <nombre> master
```
#### Cambiar de rama
```
git checkout 'nombre'
```

## BLAME
#### Mostrar quién modificó un fichero
```
git blame <nombreArchivo>
```
#### Filtrar en un rango las líneas que han sido modificadas y por quien
```
git blame -L 5,9 <nombreArchivo>
```

# OPCIONES GRÁFICAS DE GIT:
- Atlassian SourceTree
- GitKraken	//Mi elección
<br /><br />	 	 	 	 	 
					 
# HERRAMIENTAS INTERESANTES 
- GITLAB

