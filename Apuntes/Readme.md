<h1 align="center">Apuntes Linux</h1>

<h2 align="center">Comandos</h2>

<b>cd</b> (moverse)<br>
<b>vi</b> (Crear archivo)<br>
<b>rm</b> (remover)<br>
<b>rm -r</b> (borrar directorio )<br>
<b>rm -rf</b> (borrar directorio forzado)<br>
<b>alias [comando]</b> (Abreviar comando)<br>
<b>history</b> (historial de comandos)<br>
<b>mv [nombrearchivo] [nuevonombrearchivo]</b> (Cambia el nombre de archivo/carpeta)<br>
<b>mv [nombrearchivo] [nombrecarpeta/]</b> (Mueve el archivo a carpeta)<br>
<b>Recuperar contraseña:</b> (Cuando se entre y se permita seleccionar el sistema operativo o al de rescate se mueven las teclas para que no entre automaticamente al sistema operativo, posteriormente se presiona la tecla e, se para en la linea de linux, se avanza hasta el final y se cambia rhgb quiet por rd.break, posteriomente se oprime control x para guardar y continuar. Este paso me permite acceder a una consola y se presiona la tecla enter. Se realiza el comando mount para revisar las unidades que estan montadas, allí se busca la unidad sysroot. Se ejecuta el comando mount -o rw,remount /sysroot/ y se presiona enter. Se accede al directorio del root con el comando chroot /sysroot/ y se oprime enter. Para establecer las contraseñas se oprime el comando passwd se presiona enter y posterior a eso permite cambiar la contraseña. PAra que tome los cambios se utiliza el comando touch /.autorelabel, para salir de la terminal se presiona exit y luego exit de nuevo. Una vez reiniciado el pc se oprime en el incio de sesion iniciar con otra cuenta y se escribe root y la contraseña nueva.)<br>
<b>Editar archivo: </b>(control i para editar, una vez terminado el texto se presiona escape y se pone :qw y enter)<br>
<b>cat [nombreArchivo] :</b>  se puede instalar nano, para leer less [nombreArchivo]<br>
<b>man ls :</b> para cambiar el nombre de un archivo o carpeta  <br>
<b>mv [nombreArchivo] [nuevoNombre]</b> Comando para mover un archivo o carpeta <br>
<b>mv [nombreArchivo] [rutaDondeSeVaAMover]</b> Comando para copiar con todos los permisos cp -a [nombreArchivo] [nombreCopiaArchivo] <br>
<b></b>  <br>
<b></b>  <br>



CONSULTAR

QUE ES Y COMO INSTALAR UNA VPN
