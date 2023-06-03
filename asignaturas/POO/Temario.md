## UD 1. Fundamentos de POO

### 1. Objetos y clases (Cap. 1)
- Objetos
	- Instancia
	- Campos
		- Tipo
	- Estado
- Clases
	- Definición
	- Campos
	- Métodos
- Métodos
	- Mutadores
	- Selectores
	- Tipo de retorno
		- void
	- Signatura
	- Parámetros
		- Tipo
- Compilador
- Código fuente

### 2. Definiciones de clases (Cap. 2)
- Definición de clase
	- Campos
	- Constructores
	- Métodos
		- tipos de métodos
			- Selector
			- Mutador
		- partes
			- cabecera
			- cuerpo
		- Parámetros
			- parámetro real
			- parámetro formal
		- Instrucción return
			- Tipo de retorno
			- void
- Variables
	- tipos de variables
		- locales
		- de instancia
	- declaración
	- ámbito
	- tiempo de vida
- Instrucciones
	- Asignación
	- condicional
- Expresiones
	- Operadores
		- operadores de asignación compuestos (+=, -=)
- Código
	- Comentario
	- Bloque


### 3. Interacción de objetos (Cap. 3)
- Abstracción
- Modularización
- Creación de objetos
	- new
- Diagramas 
	- de clases
	- de objetos
- llamadas a métodos
	- notación con punto
	- llamada a método interno
		- this
	- llamada a método externo
- depuradores
	- punto de interrupción
- tipos
	- tipo primitivo
		- int
		- boolean
		- char
		- double
		- long
	- clases como tipos
	- cadena
		- concatenación de cadenas
- operadores
	- operadores lógicos
	- módulo
- referencia
- sobrecarga


### 4. Agrupación de objetos (Cap. 4)
- colecciones
	- tipos
		- ArrayList
		- arreglos (arrays)
	- declaración de tipos de colección
		- ArrayList\<String\>
	- índice
- iteradores
	- Iterator
- ciclos
	- while
	- for
	- for-each
- objetos anónimos
- null
- operadores
	- ++
- biblioteca de clases de Java
	- paquetes
	- import


### 5. Comportamientos más sofisticados (Cap. 6)
- uso de clases de biblioteca
	- String
	- ArrayList
	- Random
	- HashMap
	- HashSet
	- Iterator
	- Arrays
- documentación
	- lectura y escritura de documentación
		- documentación de una clase
			- nombre
			- propósito general y características
			- número de versión
				- @version
			- autor(es)
				- @author
			- documentación de cada constructor y método
				- nombre
				- tipo de retorno
					- @return
				- nombres y tipos de parámetros
					- @param
				- propósito y función del método
				- descripción de cada parámetro
				- descripción del valor de retorno
	- javadoc
- variable de clase
	- static
- constante
- final: 
	- indica que el valor de la variable no se puede modificar
	- si se aplica a un método, significa que no se puede sobreescribir
- interfaz
	- implementación
- mapa
	- pares clave/valor
	- HashMap
- conjunto
	- HashSet
- modificador de acceso
- ocultamiento de la información (encapsulación)
- acoplamiento
- objeto inmutable

### 6. Colecciones de tamaño fijo: matrices (Cap. 7)
- matrices
	- unidimensionales
		- tamaño fijo y conocido con antelación
- ArrayList
	- flexible
- bucle for
- operadores
	- ++
	- condicional
	- ternario ? :
- tabla de búsqueda



## UD 2. Estructuras de las aplicaciones

### 7. Diseño de clases (Cap. 8)
- aspectos no funcionales
	- acoplamiento
		- interconesxiones entre clases
	- cohesión
		- modularización en unidades apropiadas
- buen diseño
	- bajo acoplamiento
	- alta cohesión
- diseño dirigido por responsabilidades
- encapsulamiento
- duplicación de código
- refactorización
- estructuras
	- switch
	- enumerado
- método de clase


### 8. Objetos con buen comportamiento (Cap. 9)

#### Pruebas
Las pruebas son la actividad consistente en averiguar si un fragmento de código (un método, una clase o un probrama) presenta el comportamiento deseado.

##### Prueba unitaria
La prueba unitaria se refiere a las pruebas de las partes individuales de una aplicación, como los métodos y las clases.

##### Banco de pruebas
Un banco de pruebas es un conjunto de objetos en un estado definido que sirven como base para realizar pruebas de unidades.

##### Prueba positiva
Una prueba positiva es la prueba de un caso que se espera que funcione correctamente.

##### Prueba negativa
Una prueba negativa es la prueba de un caso que se espera que falle.

##### Automatización de pruebas
La automatización de pruebas simplifica el proceso de pruebas de regresión

##### Pruebas de regresión
Las prubas de regresión implican volver a ejecutar pruebas que ya se pasaron anteriormente con éxito, para garantizar que la nueva versión sigue superándolas.

##### Otros conceptos
- pruebas con BlueJ
- fixture

#### Depuración
La depuración es el intento de localizar y corregir el origen de un error.

##### Recorrido manual
Un recorrido manual es la actividad consistente en analizar un segmento de código línea a línea mientras que se observan los cambios de estado y otros comportamientos de la aplicación.

##### Secuencia de llamadas

#### Errores
- error de sintaxis
- error de lógica

#### Aserción
Una aserción es una expresión que establece una condición que esperamos que sea cierta. Si la condición es falsa, decimos que la aserción ha fallado. Esto indica que hay algún error en nuestro programa.


### 9. Mejora de la estructura mediante la herencia (Cap. 10)
- herencia
	- jerarquía de herencia
	- relación es-un
- superclase (padre)
	- constructor de superclase
- subclase, subtipo (hijo)
	- subclase -> especialización de superclase
	- heredan campos y métodos de superclase
- clase abstracta
- variables polimórficas
	- sustitución
- extends
- super
- enmascaramiento
- clase Object
- autoboxing
- clase envoltorio
- evitar duplicación de código
- reutilización
- mantenibilidad y extendibilidad
- pérdida de tipo

### 10. Más sobre la herencia (Cap. 11)

#### Método polimórfico

#### Tipo estático y tipo dinámico
##### Tipo estático
El tipo estático de una variable v es el tipo tal como está declarado en el código fuente, en la instrucción de declaración de la variable.

##### Tipo dinámico
El tipo dinámico de una variable v es el tipo del objeto que está almacenado actualmente en v.

#### Sobrescritura
 - sobreescritura de métodos

#### Redefinición
#### Método de búsqueda dinámica
#### Despacho de método
#### Método polimórfico
#### Super (métodos)
	- invoca a la versión del método de la superclase
#### toString
#### protected
	- sublcase tiene permitido acceso pero resto de clases no

### 11. Técnicas de abstracción adicionales (Cap. 12)
- clase abstracta
	- abstract
	- no se instancia
	- superclase de otras clases
	- método abstracto
		- subclases deben implementarlos
	- puede tener métodos implementados
- clase concreta
- interfaz
	- interface
	- implements
	- no puede tener métodos implementados (todos abstractos)
	- especificación de una clase
- herencia múltiple
	- sólo de interfaces
- instanceof

### 12. Tratamiento de errores (Cap. 14)
#### Programación defensiva

#### Informe de errores

#### Lanzamiento y manejo de excepciones

#### Procesamiento simple dea rchivos

#### Estructuras de datos

##### TreeMap

##### TreeSet

##### SortedMap

#### Aserción

##### Assert

#### Excepción
Una excepción es un objeto que representa los detalles de un fallo del programa. La excepción se genera para indicar que se ha producido un fallo.

##### Comprobada
Una excepción comprobada es un tipo de excepción cuyo uso requiere comprobaciones adicionales por parte del compilador. En particular, las excepciones comprobadas en Java requieren que se usen cláusulas *throws* e instrucciones *try*.

##### No comprobada
Una excepción no comprobada es un tipo de excepción cuyo uso no requiere ninguna comprobación por parte del compilador.

##### Manejador de excepciones

#### throw

#### throws

#### try

#### catch

#### FileReader

#### FileWriter

#### Scanner

#### Flujo

#### Serialización