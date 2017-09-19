
# Manuel Casado Vergara

## Ejercicios Tema 1

1. Consultar en el catálogo de alguna tienda de informática el precio de un ordenador tipo servidor y calcular su coste de amortización a cuatro y siete años. 
   Consultar este artículo en Infoautónomos sobre el tema.

 * Para ello voy a utilizar el servidor [Dell-Poweredge-t630](http://www.pcexpansion.es/dell-poweredge-t630-pet63003b.php):

	- EL precio con IVA del producto es de 2013,22 €, por tanto, su precio sin el IVA sería de 1590,4438 €

	- Para su amortización a los 4 años, tenemos en cuenta que cada año la amortización es del 25%:
		- 1590,4438 € x 0,25= 397,6 € cada uno de esos 4 años.

	- Para su amortización a los 7 años, se haría de la siguiente forma:
		- Los primeros dos años la amortización es del 25%, 1590,4438 € x 0,25= 397,6 € x 2 años = 795,2 €
		- El tercer y cuarto año la amortización es del 15%, 1590,4438 € x 0,15= 238,56 € x 2 años = 477,13 € 
		- El quinto año la amortización será del 10%, 1590,4438 € x 0,10= 159,04 €
		- El sexto y séptimo año la amortización será del 5%, 1590,4438 € x 0,05= 79,52 € x 2 años = 159,04 €
		- Tras esto, el producto queda amortizado.



2. Usando las tablas de precios de servicios de alojamiento en Internet “clásicos”, es decir, que ofrezcan Virtual Private Servers o servidores físicos, y de proveedores de servicios en la nube, comparar el coste durante un año de un ordenador con un procesador estándar (escogerlo de forma que sea el mismo tipo de procesador en los dos vendedores) y con el resto de las características similares (tamaño de disco duro equivalente a transferencia de disco duro) en el caso de que la infraestructura comprada se usa sólo el 1% o el 10% del tiempo.


	Servidor dedicado utilizado: [Arsys servidor dedicado](https://www.arsys.es/servidores/dedicados?s=cpc&c=121342803&a=6571030683&gclid=Cj0KCQjwgIPOBRDnARIsAHA1X3QrdSZAjoOFexMCXkpU8SqOeaGgWVcDH-o9VzPfCaBqDvpgj8YpNKoaAsfPEALw_wcB)
	Servidor en la nube: [Arsys cloud server](https://www.arsys.es/servidores/cloud)

	*Características:*
		Cloud Procesador: 8 vCPU Xeon - Dedicado Procesador: Intel Xeon E5-2630 8 Core HyperThreading
		Cloud RAM: 16 GB  - Dedicado RAM: 16 GB
		Cloud Almacenamiento: 200 GB SSD - Dedicado Almacenamiento: 5 SATA 1 TB RAID5 + 2 SSD 200GB RAID1
		Cloud Precio: 150 €/mes -> 1800€/año - Dedicado Precio: 225 €/mes -> 2700€/año
		
	-Uso al 1%
		El servidor dedicado tiene que utilizarse siempre el 100%, el virtual usándolo solo el 1% del tiempo sale a 1800 x 0,01= 18€/año.
	-Uso al 10%
		El servidor dedicado tiene que utilizarse siempre el 100%, el virtual usándolo solo el 10% del tiempo sale a 1800 x 0,1= 180€/año.
	
		


