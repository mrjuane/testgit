# testgit

git config --global user.name "nombre del usuario"
git config --global user.email direccion de email
git config --global core.editor "nombre del editor --wait"

para verificar que la configuracion esta bien
git config --global -e
para configurar el salto de linea en git

windows
CR LF

linux/mac
LF

para no tener problemas hay que realizar una configuracion que elimina o agrega el CR
para windows el comando es
 git config --global core.autocrlf true
para linux/mac el comando es
 git config --global core.autocrlf input
 
 comandos de git
 ls -- lista los archivos del directorio que estamos
 pwd -- retorna el path del directorio que estamos
 cd -- se usa igual que DOS
 mkdir -- crear un directorio
 git init -- inicializa el directorio repositorio .git
 ls -a -- te muestra los archivos de la carpeta incluyendo los ocultos
 
code . -- ejecuta el editor de texto con la ruta de la carpeta en la que estamos para programar en este caso vscode que se llama code
git status -- comando que se usa para verificar los archivos que tenemos creados en la carpeta con su status

git add archivo1.txt -- agrega el archivo de nombre archivo1.txt
git add *.txt -- agrega todos los archivos con extension .txt
git add . -- agrega todos los archivos marcados en rojo en la carpeta que nos encontramos es una mala practica por agregar 
archivos que no se necesita cargar al repositorio.

git commit -m "mensa que tenga sentido para con relacion al commit"
-------------------------------------------------------------------------
para remover un archivo
rm arch2.txt-- remueve el archivo seleccionado
git rm archivo1.txt -- remueve un archivo directo y lo pone en el stageing para commit
git restore archivo1.txt -- lo recupera del stage
-------------------------------------------------------------------------
para renombrar un archivo
mv archivo1.txt archivo.txt -- para renombrar el nombre de un archivo
git add archivo1.txt archivo.txt -- completa el renombre del archivo y se cumple el mismo principio de git rm

-------------------------------------------------------------------------
 git diff -- muestra la diferencia de los archivos modificados
 git diff --staged -- muestra los cambios que estan en el staged
 ------------------------------------------------------------------------
 git log -- este comando te dice el log de los cambios generados en ese repositorio
 git log --oneline -- muestra el codigo unico de un commit y el mensaje de cada commit
  
 ------------------------------------------------------------------------
 git branch -- te muestra la rama que estamos trabajando
 git checkout -b ramab -- se utiliza para crear un branch y ramab viene siendo el nombre del ticket o de la historia de usuario que se va a trabajar y
 se usa para cambiar de branch
 ------------------------------------------------------------------------
 para hacer el merge tenemos que irnos a la rama principal y traer la rama que realizo el cambio para fusionarlas con los cambios
 git merge ramab -- este comando trae la rama de los cambios y hace el merge con la rama principal
 
