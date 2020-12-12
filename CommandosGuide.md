# Sistemas Operativos

###  :speech_balloon: Repositorio Comandos :speech_balloon:

##### - sudo apt install
Permite instalar aplicaciones disponibles en el repositorio (se debe tener el nombre exacto de la aplicacion en el repositorio)

##### - ps -aux
Permite ver los procesos activos en el sistema

##### - top
Muestra los procesos de Linux

##### - htop
Muestra los procesos con mayor uso de interfaz

##### - sudo apt install openssh-server
Comando para instalar Open SSH Server desde la terminal

##### - ip addr
Muestra la direccion IP en uso

##### - clear
Limipa la pantalla de la terminal

##### - Q
Permite salir del comando actual

##### - sudo su
Muestra el root

##### - exit
Permite salir del path actual, cerrar la terminal

##### - whoami
Muestra el usuario actual

##### - man + comando
Muestra una ayuda o inforacion del comando que se consulta

##### - cat /path/
Ver el contenido de un archivo

##### - tail -10 /path/
Mostrar los ultimos diez contenidos del path (el numero es variable de acuerdo a lo que necesite)

##### - head -10 /path/
Mostrar los primeros diez contenidos del path (el numero es variable de acuerdo a lo que necesite)

##### - cat /path/ | more 
Ver el contenido de un archivo, pero lo limita por paginas

##### - ls
Muestra el contenido/carpetas disponibles a accesar en este nivel del directorio

##### - cd carpeta
Accede a la carpeta indicada dentro del directorio

##### - cd ..
Regresa a la carpeta anterior del directorio

##### - cp /path origen/ /path nuevo/ 
Copia de un directiorio a otro directorio nuevo (se puede agregar **-R** para que copie todo el contenido recursivamente y no solo un folder o archivo en especifico)

##### - mv /path origen/ /path nuevo/
Mueve archivo de un directorio a otro (se puede agregar **-t** para que mueva el contenido completo del directorio)

##### - mv /path origen/ /path origen/
Renombra el archivo

##### - rm /path/
Elimina el archivo indicado, solo si estamos en el directorio en donde se encuentra dicho archivo

##### - rm /path/nombre de archivo
Elimina el archivo indicado

##### - rm /path/ -R
Elimina el contenido del directorio de manera recursiva, es decir todo su contenido :boom: USAR CON CUIDADO :boom:

##### - passwd
Se usa para cambiar el password del usuario en uso, excpeto el super usario que puede cambiar el password para cualquier cuenta de usuario.

##### - history
Muestra el historial de los comandos ejecutados en la sesion de consola

##### - sudo apt install 'pack'
Instala el paquete indicado

##### - add-apt-repository ppa:numix/ppa -y
Agrega un repositorio extra en el servidor/computador, en este caso se agrega el repositorio de **numix**

##### - sudo apt update
Actualiza los repositorios

##### - sudo 'pckg'
Instala un paquete o aplicacion que se haya bajado y se encuentre en Downloads

##### - sudo telnet towel.blinkenlights.nl 
Ver peli de Star Wars ![StarWars](Darth-Vader.png)

##### - sudo apt update && sudo apt upgrade
Actualiza el Sistema Operativo

##### - nano 'nombre del archivo'
Crear un archivo nuevo, abre un mini editor en la consola que permite agregar contenido al archivo

##### - ls -la
Muestra el contenido del directorio en forma de lista

##### - chmod 777 /path/
Le da todos los permisos a todos los grupos para el directorio o archivo indicado

##### - chmod 000 /path/
Le quita todos los permisos a todos los grupos para el directorio o archivo indicado

##### - chown root 'nombre de archivo'
Modifica el propietario del archivo indicado

##### - du -h 'nombre de archivo'
Muestra el peso del archivo indicado

##### - stat 'nombre de archivo'
Muestra informacion/detalles del archivo indicado

##### - file 'nombre de archivo'
Muestra el tipo de archivo que es el archivo indicado

##### - kill -9 'pid'
Mata un proceso desde la terminal, se requiere el pid (Process ID) para poder ejecutarlo

##### - tar -cvf 'nombre de archivo' 'archivo o path que se desea comprimir'
Comprime el archivo o directorios indicados en un nuevo archivo de tipo .tar

##### - tar -xvf 'nombre de archivo.tar'
Descomprime el archivo de tipo .tar en el directorio actual

##### - reboot
Reinicia el equipo inmediatamente

##### - shutdown
Apaga el equipo 

##### - shutdown now
Apaga el equipo de manera inmediata

##### - hostname
Muestra el nombre del equipo o host

##### - wget 'URL'
Descarga lo que se encuentre en la URL indicada

##### - sudo apt insall curl
Instala CURL

##### - curl -X GET -L /path/  (script.google.com/macros/s/AKfycbztjXtmKGK6nSZ2jyqwKvvFWrsT0qEmyxKvr15SjFCVQzy83TQ/exec?data=$nombre)
Agrega informacion a una hoja de calculo de google, mediante API

##### - chmod +x 'nombre del archivo'
Agrega permiso de ejecucion al archivo indicado

##### - sudo passwd root
Permite cambiar el password de un usuario especifico

##### - mkdir
Permite crear un directorio nuevo

##### - pwd
Muestra el path actual

##### - ip -s -c -h a (s= statistics c=color h a= human address)
Muestra la ip con los detalles indicados

##### - crontab -e
crea un archvio crontab para el usuario

##### - grep -r "palabra"
Busca recursivamente en directorios y subdirectorios por la palabra indicada
 - con -l solo busca en el directorio, no sub-directorios.
 - con -w busca la palabra completa, es case sensitive


#### - ZENITY

##### - zenity --info --text="Esta es una prueba"
Muesta una ventana pop up de tipo informacion o alerta con el mensaje indicado

##### - zenity --info --text="Esta es una prueba"
Muestra una ventana pop up, que permite ingresar informacio y en la variable "nombre" guarda lo que se le escribe

##### - echo $nombre
Muestra el contenido de la variable (previamente ingresado)

##### - zenity --password
Guarda una contrasena mediante una ventana pop up

##### - zenity --question
Muestra una ventana pop up con una pregunta

##### - zenity --list --title="Comandos" --column="Comando" --text="Seleccione un comando de la lista" "ls -la" "ps -aux"
Muestra una ventana pop up con una lista que incluye varias columnas con el resultado de los procesos de todos los usuarios


#### - DOCKER

##### - docker images
Muestra las imagenes/contenedores disponibles (se debe instalar docker previamente)

##### - sudo docker run -it 'nombre de la imagen'
Inicializa y ejecuta la imagen indicada

##### - cat /etc/os-release
Muestra la imagen en la que se encuentra el usuaio actualmente

##### - docker ps-a
Muestra los estados de las contenedores creados y otros detalles

##### - docker start 'contained id'
Inicia el contenedor indicado sin ingresar a el

##### - nmap
Muestra los puertos que estan abiertos de un servidor

##### - free
Muestra la memoria disponible

##### - docker commit -m 'instalacion x' 'containerID' nombre/nombreimagen
Salva la imagen

##### - docker login -u 'username'
Permite loguear la cuenta de dockerhub y poder subir las imagenes salvadas (crear cuenta previamente en la pagina de dockerhub)

##### - docker push 'nombre de la imagen'
Sube la imagen indicada al repositorio de dockerhub (se debe loguear previamente a la cuenta)


#### - ARCH LINUX

##### - sudo pacman -Syuu
instala actualizaciones del sistema - paquetes

##### - sudo pacman -S unrar zip unzip p7zip gzip bzip2
Instala paquetes para comprimir/descomprimir

##### - sudo pacman -S yay
Incluye el repositorio AUR

##### - yay -octopi
Insatala la aplicacion Octopi

##### - sudo pacman -S base-devel
Instala Fakeroot

##### - sudo useradd -m nombredeusuario -G wheel -p passworddelusuario
Permite crear nuevos usuarios



# - </END>
