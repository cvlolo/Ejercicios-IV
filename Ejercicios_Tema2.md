# Manuel Casado Vergara

## Ejercicios Tema 2

### 1. Descargar y ejecutar las pruebas de alguno de los proyectos anteriores, y si sale todo bien, hacer un pull request a este proyecto con tests adicionales, si es que faltan (en el momento que se lea este tema).

En el repositorio [siguiente](https://github.com/cvlolo/tdd-gdg) podemos encontrar un archivo en python con diferentes funciones y tests, he añadido la siguiente función con sus correspondientes
tests:

	
	def squareRoot(a):
    if(not(type(a)is int)):
        return -1
    else:
        return math.sqrt(a);

	def testRoot(self):
		self.assertEqual(squareRoot(4), 2, "La raiz cuadrada de 4 es 2")
		self.assertEqual(squareRoot(25), 5, "La raiz cuadrada de 25 es 5")
		self.assertEqual(squareRoot(7.9), -1, "No ha introducido un numero entero")
 	
### 2. Para la aplicación que se está haciendo, escribir una serie de aserciones y probar que efectivamente no fallan. Añadir tests para una nueva funcionalidad, probar que falla y escribir el código para que no lo haga (vamos, lo que viene siendo TDD).

Se ha realizado esto tanto en el ejercicio anterior como en mi [proyecto de la asignatura](https://github.com/cvlolo/IV-Proyecto) 

### 3. Convertir los tests unitarios anteriores con assert a programas de test y ejecutarlos desde mocha, usando descripciones del test y del grupo de test de forma correcta. Si hasta ahora no has subido el código que has venido realizando a GitHub, es el momento de hacerlo, porque lo vas a necesitar un poco más adelante.

Voy a utilizar mocha en python mediante [pocha](https://github.com/rlgomes/pocha), que nos ayuda a importar la facilidad de escritura de tests de nodejs a python.

	import unittest
	import math
	from pocha import describe,it

	@describe('Tests de prueba')
	def _():
	
		def squareRoot(a):
		    if(not(type(a)is int)):
			return -1
		    else:
			return math.sqrt(a);

		class SoloTest():

			@it('testing sobre la operacion raiz cuadrada') 
			def testRoot():
				assert squareRoot(4)==2
				assert squareRoot(25)==5
				assert squareRoot(7.9)==-1

	if __name__ == '__main__':
	    unittest.main()


Al ejecutarlo mediante pocha, obtenemos lo siguiente:

![img](https://github.com/cvlolo/Ejercicios-IV/blob/master/img/pocha.png)

### 4. Instalar alguno de los entornos virtuales de node.js (o de cualquier otro lenguaje con el que se esté familiarizado) y, con ellos, instalar la última versión existente, la versión minor más actual de la 4.x y lo mismo para la 0.11 o alguna impar (de desarrollo).

Voy a instalar dos versiones diferentes de python utilizando virtualend, la 2.7 y la 3.5. 

Primero instalo virtualend con la orden `sudo apt-get install virtualenv python-virtualenv`, y una vez instalado, ejecuto las dos ordenes siguientes:

![img](https://github.com/cvlolo/Ejercicios-IV/blob/master/img/virtualenv.png)

Con esto ya tendriamos disponibles dos versiones diferentes de python.

