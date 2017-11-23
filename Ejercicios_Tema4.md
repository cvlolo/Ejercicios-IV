# Manuel Casado Vergara

## Ejercicios Tema 4

### 1. Instala LXC en tu versión de Linux favorita. Normalmente la versión en desarrollo, disponible tanto en GitHub como en el sitio web está bastante más avanzada; para evitar problemas sobre todo con las herramientas que vamos a ver más adelante, conviene que te instales la última versión y si es posible una igual o mayor a la 1.0.

Utilizo los siguientes comandos para instalar la última versión estable del programa:

		sudo add-apt-repository ppa:ubuntu-lxc/lxc-stable
		sudo apt-get update
		sudo apt-get install lxc

### 2. Crear y ejecutar un contenedor basado en tu distribución y otro basado en otra distribución, tal como Fedora. Nota En general, crear un contenedor basado en tu distribución y otro basado en otra que no sea la tuya.

En primer lugar creamos los dos contenedores con la orden sudo lxc-create -t fedora -n FedoraCont para crear un contenedor Fedora y la orden sudo lxc-create -t ubuntu -n UbuntuCont para el contenedor de ubuntu.  Los listamos con lxc-ls para ver que se han creado correctamente:

![img](https://github.com/cvlolo/Ejercicios-IV/blob/master/img/lxc.png)

Ahora solo tendríamos que utilizar sudo lxc-start -n nombre para ejecutarlo y sudo lxc-stop -n nombre para pararlo.

### 3. Instalar docker.

Realizado para llevar acabo [mi proyecto](https://github.com/cvlolo/IV-Proyecto)

### 4.Instalar a partir de docker una imagen alternativa de Ubuntu y alguna adicional, por ejemplo de CentOS.

Realizado para llevar acabo [mi proyecto](https://github.com/cvlolo/IV-Proyecto)

### 6.Crear a partir del contenedor anterior una imagen persistente con commit.

Realizado para llevar acabo [mi proyecto](https://github.com/cvlolo/IV-Proyecto)

### 7.Crear un Dockerfile para el servicio web que se ha venido desarrollando en el proyecto de la asignatura.

Realizado para llevar acabo [mi proyecto](https://github.com/cvlolo/IV-Proyecto)

### 8.Desplegar un contenedor en alguno de estos servicios, de prueba gratuita o gratuitos.

Realizado para llevar acabo [mi proyecto](https://github.com/cvlolo/IV-Proyecto)
