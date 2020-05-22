# GITHUB-COMMAND
Comandos GitHub básicos

//Sirve para guardar el nombre con el que apareceremos al subir los archivos

-git config --global user.name "nombre"      

//Dirección de correo que nos identifica

-git config --global user.email correo@      

//Esta herramienta nos sirve para comparar diferencias entre ficheros

-git config --global diff.tool tkdiff        

//Donde voy a guardar las crendenciales de repositorios remotos

-git config --global credential.helper manager      

//Elegir editor de trabajo en este caso nano

-git config --global core.editor nano        

//Inicializar repositorio

git init 				     

//Crear fichero readme o cualquier otro

echo "#Primera línea de un fichero readme.dm" > readme.md	

//Añadir ficheros al repositorio

git add * or git add nombreFichero

//Comprobar estado del fichero

git status

//Añadir revisiones del proyecto

git commit -m "nombre del commit"

//Ver commits

git log --oneline

//Modificar un fichero de texto

less nombreFichero

//Para ignorar ficheros tenemos que crear el fichero gitignore

nano .gitignore -> Dentro de este fichero si por ejemplo tenemos archivos .tmp, dentro de ese fichero debemos de poner *.tmp

//Comparar archivos para ver las modificaciones que se han realizado a un archivo modificado

-git diff

//Muestra en la consola las diferencias entre los archivos

-git difftool  -> Para una mejor visualización necesitaremos la herramienta tkdiff  se almacena dentro de la ruta GIT/usr/bin

//Borrar fichero

rm nombreFichero

//Mover renombrar o mover ficheros

//Renombrar

git mv nombreFichero nombreFichero1

//Mover

git mv nombreFichero ruta


OPCIONES GRÁFICAS DE GIT:
- Atlassian SourceTree
- GitKraken																	//Mi elección
	 	 	 	 	 
					 
HERRAMIENTAS INTERESANTES 
- GITLAB

