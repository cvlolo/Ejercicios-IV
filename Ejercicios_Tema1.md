
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

Características:
	
 	Cloud Procesador: 8 vCPU Xeon - Dedicado Procesador: Intel Xeon E5-2630 8 Core HyperThreading
	Cloud RAM: 16 GB  - Dedicado RAM: 16 GB
  	Cloud Almacenamiento: 200 GB SSD - Dedicado Almacenamiento: 5 SATA 1 TB RAID5 + 2 SSD 200GB RAID1
  	Cloud Precio: 150 €/mes -> 1800€/año - Dedicado Precio: 225 €/mes -> 2700€/año
		
Uso al 1%
	
 * El servidor dedicado tiene que utilizarse siempre el 100%, el virtual usándolo solo el 1% del tiempo sale a 1800 x 0,01= 18€/año.
		
Uso al 10%
	
 * El servidor dedicado tiene que utilizarse siempre el 100%, el virtual usándolo solo el 10% del tiempo sale a 1800 x 0,1= 180€/año.
	
		
3. En general, cualquier ordenador con menos de 5 o 6 años tendrá estos flags. ¿Qué modelo de procesador es? ¿Qué aparece como salida de esa orden? Si usas una máquina virtual, ¿qué resultado da? ¿Y en una Raspberry Pi o, si tienes acceso, el procesador del móvil?

El modelo de mi procesador sería el siguiente:
	
	lolo@Lolo-PC:~$ cat /proc/cpuinfo 
	model name	: Intel(R) Core(TM) i7-4510U CPU @ 2.00GHz

Ahora obtenemos sus flags correspondientes:

	lolo@Lolo-PC:~$ egrep '^flags.*(vmx|svm)' /proc/cpuinfo
	flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon 		pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf eagerfpu pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 movbe popcnt tsc_deadline_timer 		aes xsave avx f16c rdrand lahf_lm abm epb tpr_shadow vnmi flexpriority ept vpid fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid xsaveopt dtherm ida arat pln pts

Para una raspberry pi:

	pi@raspberrypi:~ $ cat /proc/cpuinfo
	model name	: ARMv7 Processor rev 4 (v7l)

En máquina virtual:

	lolo@lolo-VirtualBox:~$ cat /proc/cpuinfo 
	model name	: Intel(R) Core(TM) i7-4510U CPU @ 2.00GHz
	lolo@Lolo-PC:~$ egrep '^flags.*(vmx|svm)' /proc/cpuinfo
	No sale nada

4.  Comprobar si el núcleo instalado en tu ordenador contiene este módulo del kernel usando la orden kvm-ok.
    Instalar un hipervisor para gestionar máquinas virtuales, que más adelante se podrá usar en pruebas y ejercicios.

Ejecuto la orden kvm-ok:

	lolo@Lolo-PC:~/Ejercicios-IV$ kvm-ok
	INFO: /dev/kvm exists
	KVM acceleration can be used

Como hipervisor he instalado VirtualBox.

	






		


