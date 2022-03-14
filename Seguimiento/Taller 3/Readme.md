<h1 align="center">Taller III (Linux 1)</h1>
_Gean Carlo Cortes Mayorga 11-03-2022_

<h2 align="center"> 1. Comprimir el directorio Bisabuelo y Bisabuela </h2>

Para comprimir cada uno de los directorios usamos el comando 
`tar -cvf nombrenuevo.tar nombredirectorio`

<img src="./img/Screenshot_1.png"/>
<img src="./img/Screenshot_2.png"/>




<h2 align="center"> 2. Comprimir el directorio Bisabuelo y Bisabuela en formato tar.gz y bz2</h2>

Para comprimir cada uno de los directorios usamos el comando 
`tar -cvf nombrenuevo.tar.gz nombredirectorio`

tar.gz:
<img src="./img/Screenshot_3.png"/>
<img src="./img/Screenshot_4.png"/>

bz2:

<img src="./img/Screenshot_9.png"/>
<img src="./img/Screenshot_10.png"/>



<h2 align="center"> 3. Listar los archivos comprimidos</h2>

Para listar cada uno de los directorios comprimidos usamos el comando `tar -tvf nombrearchivo.{formato}`


<img src="./img/Screenshot_5.png"/>
<img src="./img/Screenshot_6.png"/>
<img src="./img/Screenshot_7.png"/>
<img src="./img/Screenshot_8.png"/>
<img src="./img/Screenshot_11.png"/>
<img src="./img/Screenshot_12.png"/>


<h2 align="center"> 4. Descomprimir los directorios /Bisabuelo en las siguientes rutas: </h2>

Para descomprimir cada uno de los directorios usamos el comando `tar -xvf nombrenuevo.{formato} -C  ../../..`

`/tmp`
Ejemplo con Bisabuelo.tar ../../tmp/ (estando en /home/geandev)
<img src="./img/Screenshot_13.png"/>
<img src="./img/Screenshot_14.png"/>


`/root`
Ejemplo con Bisabuelo.tar ../../root/ (estando en /home/geandev)
<img src="./img/Screenshot_15.png"/>
<img src="./img/Screenshot_16.png"/>




<h2 align="center"> 5. Comprimir los directorios usando la herramienta o paquete (zip, unzip)</h2>

<img src="./img/Screenshot_.png"/>
<img src="./img/Screenshot_.png"/>



<h2 align="center"> 6. Reto: Realizar un script en bash shell que haga la copia de seguridad del directorio /etc. A las 24h todos los dias.</h2>


<img src="./img/Screenshot_.png"/>
<img src="./img/Screenshot_.png"/>
