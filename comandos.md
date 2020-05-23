# GITHUB-COMMAND
Comandos GitHub básicos

#### Sirve para guardar el nombre con el que apareceremos al subir los archivos
-git config --global user.name "nombre"      
<br />
### Dirección de correo que nos identifica
-git config --global user.email correo@      
<br />
### Esta herramienta nos sirve para comparar diferencias entre ficheros
-git config --global diff.tool tkdiff        
<br />
### Donde voy a guardar las crendenciales de repositorios remotos
-git config --global credential.helper manager      
<br />
### Elegir editor de trabajo en este caso nano
-git config --global core.editor nano        
<br />
### Inicializar repositorio
git init 				     
<br />
### Crear fichero readme o cualquier otro
echo "#Primera línea de un fichero readme.dm" > readme.md	
<br />
### Añadir ficheros al repositorio
git add * or git add nombreFichero
<br />
### Comprobar estado del fichero
git status
<br />
### Añadir revisiones del proyecto
git commit -m "nombre del commit"
<br />
### Ver commits
git log --oneline
<br />
### Modificar un fichero de texto
less nombreFichero
<br />
### Para ignorar ficheros tenemos que crear el fichero gitignore
nano .gitignore -> Dentro de este fichero si por ejemplo tenemos archivos .tmp, dentro de ese fichero debemos de poner *.tmp
<br />
### Comparar archivos para ver las modificaciones que se han realizado a un archivo modificado
-git diff
<br />
### Comparar archivos en caso de que le hayamos hecho un git add 
-git diff --staged
<br />
### Muestra en la consola las diferencias entre los archivos
-git difftool  -> Para una mejor visualización necesitaremos la herramienta tkdiff  se almacena dentro de la ruta GIT/usr/bin
<br />
### Borrar fichero
rm nombreFichero
<br />
### Mover renombrar o mover ficheros

#### Renombrar
git mv nombreFichero nombreFichero1
<br />
#### Mover
git mv nombreFichero ruta
<br />
### Mostrar informacion en colummnas de los commits tanto el hash, el nombre, el tiempo y el nombre.
git log --pretty=format:"%h %an %ar - %s"
<br />
###Mostrar información de un commit
git show hashDelArchivo
<br /><br />
## OPCIONES GRÁFICAS DE GIT:
- Atlassian SourceTree
- GitKraken	//Mi elección
<br /><br />	 	 	 	 	 
					 
## HERRAMIENTAS INTERESANTES 
- GITLAB

