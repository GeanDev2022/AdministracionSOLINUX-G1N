<h1 align="center">Apuntes Linux</h1>

<h2 align="center">Comandos</h2>

<b>cat </b> (leer y crear archivos)<br><br>
<b>mkdir</b> (crea fichero)<br><br>
<b>rmdir</b> (eliminar fichero) <br><br>
<b>cd</b> (moverse)<br><br>
<b>vi</b> (Crear archivo)<br><br>
<b>rm</b> (remover)<br><br>
<b>rm -r</b> (borrar directorio )<br><br>
<b>rm -rf</b> (borrar directorio forzado)<br><br>
<b>alias [comando]</b> (Abreviar comando)<br><br>
<b>history</b> (historial de comandos)<br><br>
<b>mv [nombrearchivo] [nuevonombrearchivo]</b> (Cambia el nombre de archivo/carpeta)<br><br>
<b>mv [nombrearchivo] [nombrecarpeta/]</b> (Mueve el archivo a carpeta)<br><br>
<b>Recuperar contraseña:</b> (Cuando se entre y se permita seleccionar el sistema operativo o al de rescate se mueven las teclas para que no entre automaticamente al sistema operativo, posteriormente se presiona la tecla e, se para en la linea de linux, se avanza hasta el final y se cambia rhgb quiet por rd.break, posteriomente se oprime control x para guardar y continuar. Este paso me permite acceder a una consola y se presiona la tecla enter. Se realiza el comando mount para revisar las unidades que estan montadas, allí se busca la unidad sysroot. Se ejecuta el comando mount -o rw,remount /sysroot/ y se presiona enter. Se accede al directorio del root con el comando chroot /sysroot/ y se oprime enter. Para establecer las contraseñas se oprime el comando passwd se presiona enter y posterior a eso permite cambiar la contraseña. PAra que tome los cambios se utiliza el comando touch /.autorelabel, para salir de la terminal se presiona exit y luego exit de nuevo. Una vez reiniciado el pc se oprime en el incio de sesion iniciar con otra cuenta y se escribe root y la contraseña nueva.)<br><br>
<b>Editar archivo: </b>(control i para editar, una vez terminado el texto se presiona escape y se pone :qw y enter)<br><br>
<b>cat [nombreArchivo] :</b> se puede instalar nano, para leer less [nombreArchivo]<br><br>
<b>man ls :</b> para cambiar el nombre de un archivo o carpeta <br><br>
<b>mv [nombreArchivo] [nuevoNombre]</b> Comando para mover un archivo o carpeta <br><br>
<b>mv [nombreArchivo] [rutaDondeSeVaAMover]</b> <br>
<b>tar</b>(Sirve para comprimir y descomprimir archivos y directorios) <br><br>
<b>tar -cvf [nombrearchivo].tar /home/... </b> (-c: crear comprimido, -v: verbose, log, observar comportamiento, -f:el nombre del comprimido) <br><br>
<b>tar -xvf [nombrearchivo].tar </b> (-x: descomprimido, -v: verbose, log, observar comportamiento, -f:el nombre del comprimido) <br><br>
<b>tar -xvf [nombrearchivo].tar -c /home/.. </b>(para descomprimir en alguna ruta) <br><br>
<b>tar -tvf [nombrearchivo].tar</b>(listar) <br><br>
<b>tar -xvf [nombrearchivo] "file1"  "file2"</b> (Descomprimir multiples archivos)<br><br>
<b>tar -cf [nombrearchivo] bar foo</b> (Comprimir multiples archivos)<br><br>
<b>df -Th</b> (Permite saber el tamaño de los discos y particiones)<br><br>
<b>du -sh</b> (Permite saber el tamaño de los archivos) </br><br>
<b>zip [nombrenuevo].zip nombreexiste</b> (Sirve para comprimir archivos y directorios) </br><br>
<b>unzip [nombreexiste].zip</b> (Sirve descomprimir archivos y directorios)</br><br>
<b>df -Th</b> (Mirar el almacenamiento de las particiones) </br><br>
<b>uptime</b> (tiempo encendido)</br><br>
<h2>PERMISOS DE USUARIO , GRUPO U OTROS</h2> </br><br>
<b>
User: r:read(4),
w:write(2),
x:execute(1)
</b> </br><br>
<b>chmod ### [archivo o directorio]</b>(Permiso de usuario,grupo u otro) </br><br>
<b>chmod u+r,u+w,u+x</b> (Darle permiso de rwx al usuario) </br><br>
<b>chmod u=rwx</b> </br><br>
<img scr="./img/Screenshot_35.png"/>
<img src="./img/4.png"/>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>

