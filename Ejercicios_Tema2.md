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
 	

