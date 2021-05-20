# Desafío

# Hola Octano!
En este documento se describe como ejecutar contenedor asociado a desafio indicado.
Lo primero que debemos hacer es descargar y/o conectar el repositorio para obtener los archivos Dockerfile y index.html
Con ellos se podra ejecutar crear imagen y luego se podra ejecutar container "Dockerizado" con webserver. Ademas, el codigo contiene linea para poder copiar el archivo index adjunto, para que este logra mostrar el codigo en base 64.
A continuacion, se detalla los pasos a seguir para la correcta ejecucion del contenedor
# Paso 1
Debemos conectar el repositorio https://github.com/rodxcharm/DesafioOctano y/o descargar los archivos alojados en la carpeta data.
# Paso 2
Una vez conectado el repositorio y/o descargados los archivos, debemos ejecutar el comando "docker build -t nombreimagen ." en su WSL o Linux OS cargado en su equipo.
# Paso 3
Una vez ejecutada correctamente la creacion de la imagen, procedemos a la ejecucion del contenedor, a partir de la imagen creada. Para ello, debemos ejecutar el comando
"docker run -dit --name nombre_contenedor -p 80:80 nombre_imagen
# Paso 4
Una vez ejecutado correctamente el comando anterior, ya tendremos en ejecucion nuestro contenedor. Para validar su ejecución, podemos ejecutar el comando "docker ps" el cual nos mostrara el estado de ejecucion del contenedor y otros datos, tal como lo muestra la siguiente imagen:
![image](https://user-images.githubusercontent.com/84494491/118931345-e062fc00-b914-11eb-94e6-18163eeae3a0.png)
# Paso 5
En este paso, procederemos a validar la correcta operacion de nuestro webserver Apache montado en el contenedor creado. Para ello debemos abrir el navegador de su gusto e ingresar a http://localhost, los cual nos mostrara nuestro codigo en base 64, tal como muestra la siguiente imagen:
![image](https://user-images.githubusercontent.com/84494491/118931932-7bf46c80-b915-11eb-9333-8c9be23e8c6b.png)

Siguiendo estos pasos, podremos tener operativo nuestro webserver alojado en contenedor.
¡Muchas gracias por el desafío!

NOTA: me tomo aproximadamente 5 horas lograr el objetivo.
