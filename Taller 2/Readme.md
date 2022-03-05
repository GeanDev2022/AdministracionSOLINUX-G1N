<h1 align="center">Taller II (Linux 1)</h1>
_Gean Carlo Cortes Mayorga 25-02-2022_

<h2 align="center"> 1. Recuperar la contraseña del usuario Root.</h2>

Inicialmente, cuando se inicia el sistema, presionamos la tecla `ESC` donde ingresaremos al sistema interno.

<img src="./img/punto1/1.png"/>

Luego reemplazamos la palabra `rhgb quiet` por `rd.break`

<img src="./img/punto1/2.png"/>
<img src="./img/punto1/3.png"/>

Presionamos enter y escribimos el comando `mount`

<img src="./img/punto1/4.png"/>
<img src="./img/punto1/5.png"/>

Luego, escribimos el comando `mount -o rw, remount /sysroot/`

<img src="./img/punto1/6.png"/>

Siguiendo el proceso, debemos escribir `chroot /sysroot` seguido de `passwd` para renovar la contraseña del usuario root

<img src="./img/punto1/7.png"/>

Luego presionamos `touch /.autorelabel`

<img src="./img/punto1/8.png"/>

Finalizamos usando el comando `exit` dos veces

<img src="./img/punto1/9.png"/>

Esperamos a que se reinicie el sistema e ingresamos con el usuario `root` y escribimos la contraseña propuesta en el proceso

<img src="./img/punto1/10.png"/>
<img src="./img/punto1/11.png"/>

Y finalmente podremos ingresar a la interfaz y sistema con los privilegios

<img src="./img/punto1/12.png"/>

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<h2 align="center">2. Practicar el movimiento de archivos y directorios. Ademas renombrar archivos</h2>

Damos inicio creamos dos carpetas con los nombres de `Bisabuelo` y `Bisabuela`

<img src="./img/punto2/1.png"/>

Luego vamos a mover las carpetas `Abuelo`  a la carpeta `Bisabuela` y `Abuela` a la carpeta `Bisabuelo` 

<img src="./img/punto2/2.png"/>
<img src="./img/punto2/3.png"/>

Tenemos esta estructura

<img src="./img/punto2/tree1.png"/>

Posteriormente vamos a pasar los archivos que estan contenidos en cada una de las carpetas de `Bisabuelo` a `Bisabuela`respectivamente.

<!-- AQUI EMPIEZA LA PARTE DE BISABUELO A BISABUELA -->
<h2 align="center"> Bisabuelo --> Bisabuela </h2>

Abuela --> Abuelo

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/4.png"/>
<img src="./img/punto2/5.png"/>

Mama --> Papa

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/6.png"/>
<img src="./img/punto2/7.png"/>

Hija --> Hijo

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/8.png"/>
<img src="./img/punto2/9.png"/>

<!-- AQUI EMPIEZA LA PARTE DE BISABUELA A BISABUELO -->
<h2 align="center"> Bisabuela --> Bisabuelo </h2>

Abuelo --> Abuela

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/10.png"/>
<img src="./img/punto2/11.png"/>

Papa --> Mama

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/12.png"/>
<img src="./img/punto2/13.png"/>

Hijo --> Hija

Empezamos buscando el archivo moviendonos con el comando `cd` y luego verificando que el archivo se escuentre con `ls`, posteriormente hacemos uso del comando `vm` para mover el archivo: 

<img src="./img/punto2/14.png"/>
<img src="./img/punto2/15.png"/>

Finalmente podemos corroborar mediante el uso del comando `tree` el proceso que se acabo de realizar

<img src="./img/punto2/tree2.png"/>

El proximo proceso que se realizara sera el de crear dos carpetas `Nieto/Bisnieto` y `Nieta/Bisnieta` contenidas en cada carpeta de `Bisabuelo` y `Bisabuela` respectivamente

<img src="./img/punto2/16.png"/>

Empezamos creando la carpeta Nieto con el comando `mkdir`

<img src="./img/punto2/17.png"/>

Creamos el archivo con la informacion del Nieto con el comando `vi` y luego con `i` para editar, luego `ESC` : wq para guardar

<img src="./img/punto2/18.png"/>

Luego creando la carpeta Bisnieto con el comando `mkdir`

<img src="./img/punto2/19.png"/>

Creamos el archivo con la informacion del Bisnieto con el comando `vi` y luego con `i` para editar, luego `ESC` : wq para guardar

<img src="./img/punto2/20.png"/>

