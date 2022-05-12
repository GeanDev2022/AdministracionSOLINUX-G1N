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
<h2><strong>Permisos</strong></h2>

Lectura: r = 4</br><br>
Escritura: w = 2</br><br>
Ejecución: x = 1</br><br>

Grupos</br><br>
Pueden tener diferentes permisos de acuerdo a cada grupo</br><br>
User: rwx = 421 = 7</br><br>
Group: rwx = 421 = 7</br><br>
Others: rwx = 421 = 7</br><br>

Para dar permisos a un directorio se toma el el total de cada grupo</br><br>
Por ejemplo, para darle todos los permisos a un archivo seria = 777

Para asignar el permiso se utiliza el comando <strong>chmod 777 [archivo o directorio]</strong>

Comando para agregar usuario: <strong>adduser [nombreUsuario]</strong></br><br>
Comando para añadir contraseña al usuario: <strong>passwd [nombreUsuario]</strong></br><br>
Comando para quitarle los archivos a un usuario: <strong>chown [usuario][usuario] [archivos o directorios]</strong></br><br>
Comando para crear un comando sin bash o sin acceso al sistema: useradd [nombreUsuario] -s /sbin/nologin </br><br>
Comando para darle otra vez permisos al usuario: usermod [nombreUsuario] -s /bin/bash </br><br>
Comando para eliminar un usuario: userdel [nombreUsuario] v
Comando para crear grupo: groupadd [nombreGrupo] v
Comando para ver los grupos: cat /etc/group </br><br>
<b>top</b>  para mirar los procesos que esta corriendo en el servidor, es mas administrativo</br><br>
<b>yum install httpd</b> Instalar servidor web</br><br>
<b>systemctl start,restart,enable,stop</b> permite depeniendo la bandera ya sea la ejecucion, restart... </br><br>
<b>ps</b> para ver los procesos que se estan ejecutando en nuestro sistema</br><br>
<b>kill -9 </b> Esta bandera sirve para matar de forma adecuada un proceso `(PREGUNTA DE PARCIAL)`</br><br>
<b>df -h</b> Espacio en las particiones </br><br>
<b>xfs</b> Aumentar en caliente las particiones pero no disminuir</br><br>
<b>ext4</b> Aumentar las partiiones y dismunuir, pero no en caliente</br><br>
<b>du -sh [directorio]</b> </br><br>
<b>htop</b> (ver procesos con grafica) </br><br>
<b>jobs</b>control c: salir control z: mandar a segundo plano (Para ver procesos que se ejecutan en segundo plano)</br><br>
<b>fg %#procesos</b> para regresar el procesos detenido de sleep tiempo</br><br>
<b>nice -n [valor] [nombreproceso]</b> (valor menos es mas favorable y mas valor es menos favorable)</br><br>
<b>-g</b> grupo primario</br><br>
<b>-G</b> grupo secundario</br><br>
<h1> Redirecciones y tuberias</h1>
<b> `>` Cambia el contenido del archivo texto </b> </br><br>
<b> `>>` Agrega y mantiene el contenido anterior  </b> </br><br>
<b> 0: stdin  salida estandar
    1: stdout salida buena
    2: sterr  salida con error
    find / -type f -user geandev > todo.txt 2>&1
</b> </br><br>    
<img src="./img/Screenshot_3.png"/></br><br>
<b> ps fea | grep ssh</b> la salida del comando ps lo envia a grep y filtra todo lo que tenga ssh </br><br>
<b>ps fea | grep ssh 2> ssh.txt</b> </br><br>
<h1>Scripts</h1>
<b>
#!/bin/bash </br>
- instruccion 1
- instruccion 2
- var param_1 = $1
- var param_2 = $2
- .....
- var param_10 = ${10}
</b> </br><br>
<b>vi [nombrescripts].sh (parametros)</b> Realiza todas las instrucciones que nosotros le digamos</br><br>
<b>chmod +x [nombrescript]</b> </br><br>
<b>mkdir script, cd script, vi deploy_web.sh, i, 
#!/bin/bash
<img src="./img/Screenshot_4.png"/></br><br>
luego ./deploy_web.sh Gean
<img src="./img/Screenshot_5.png"/></br><br>

</b> </br><br>
<b>usr/share/nginx/html</b> </br><br>

<h1>20 ABRIL 2022</h1>
<b>Firewall</b> (firewall-cmd --list-all)</br><br>
<b>DNS</b> (cat /etc/resolve.conf)</br><br>
<b>Gateway</b> (route -n) </br><br>
<b>Selinux</b>  (cat /etc/selinux)</br><br>
<b>route -n</b> sirve para verificar si un servidor tiene internet mediante el gateway (ping [ip])</br><br>
<b>cat /etc/selinux/config   </b> </br><br>
<b>getenforce</b> consultar el enforce actual </br><br>
<b>setenforce 0/1</b>  0:permisivo 1:enforcing</br><br>
<b>sudo firewall-cmd --zone=public ---permanent --add-port=3306/tcp</b> </br><br>

<h1>Crear particiones</h1></br><br>
<b>lsblk
sudo su</br>
parted /dev/sda1 unit MB print free</br>
fdisk /dev/sdb</br>
n</br>
p</br>
1</br>
enter</br>
+2GB</br>
p</br>
w</br>
partprobe -s</br>
lsblk</br>
mkfs.ext3 /dev/sdb1</br>
mkdir /mnt/disconuevo</br>
mount /dev/sdb1 /mnt/disconuevo/</br>
mount</br>
df -Th</br>
cd /mnt/disconuevo</br>
ls</br>
touch prueba</br>
echo "escribir" > prueba</br>
cat prueba</br>
cd ..</br>
vi /etc/fstab</br>
i</br>
/dev/sdb1 /mnt/disconuevo ext3 defaults 0 0</br>
esc</br>
:wq</br>
systemctl reboot</br>
</b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>
<b></b> </br><br>

