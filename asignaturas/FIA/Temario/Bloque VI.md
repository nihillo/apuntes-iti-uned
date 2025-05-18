# Redes Semánticas y Marcos

Cap. 4 libro
## Introducción
## Redes semánticas
### Representación de conocimiento
### Representación de predicados no binarios
### Representación de acciones
### Representación de conocimiento disjunto
## Inferencia de conocimiento en redes semánticas
### Equiparación
### Herencia de propiedades
## Marcos
### Representación de conocimiento
- Marcos
- Relaciones
- Propiedades
- Facetas
#### Representación de conceptos e instancias
- Marcos clase
- Marcos instancia
#### Representación de relaciones entre conceptos
- Relaciones estándar
- Relaciones no estándar
#### Representación de las propiedades de los conceptos
- Propiedades de clase
- Propiedades de instancia
#### Representación de facetas de propiedades
- Facetas que definen propiedades de clase, de instancia y relaciones
- Facetas comunes a las propiedades de clase y relaciones - propiedad general
- Facetas que definen propiedades de instancia
### Criterios de diseño
## Inferencia de conocimiento en SBM
### Equiparación
- Clasificación: encontrar los marcos clase (uno o varios) de la BC que describen más consistentemente al marco pregunta, en base a un conjunto de propiedades de este con valores conocidos
- Ejemplos: clasificación de bacterias según taxonomía, sistema de diagnóstico médico, sistema de clasificación de fallos en entorno industrial
- Inconvenientes: 
	- Propiedades distribuidas por varios marcos de la BC
	- Conjunto pequeño de valores conocidos del marco pregunta
	- Valores pueden ser inciertos (grado de seguridad)
	- Información aportada por cada propiedad diferente
	- Valores por omision no siempre válidos: puede haber excepciones
- Etapas:
	- Selección de marcos candidatos
		- Si el tipo es conocido: se elige marco clase de este tipo y sus descendientes
		- Si es desconocido: se eligen aquellos marcos clase en que exista al menos una propiedad conocida en el marco pregunta
	- Cálculo de valores de equiparación
		- Una vez seleccionados los candidatos se calculan sus VE, que representa el grado de idoneidad
		- Para cada sistema se debe definir cómo se calcula. En general debe ser mayor cuanto más coincidentes son los valores de las propiedades. El grado en que la propiedad sea esencial también ifluirá, haciendo, cuanto más alto es, que más aumente el VE de las propiedades coincidentes y más disminuya el de las no coincidentes.
	- Decisión
		- Por último se decide qué marco o marcos clase se equipara finalmente al marco pregunta, dependiendo de los valores de equiparación que se hayan obtenido y la especificidad del marco clase (cuanto más específico, mejor). En caso de que no haya candidatos lo suficientemente relevantes o lo suficientemente específicos, se encontrarán otros mediante cualquiera de estos métodos:
			- Ascender a lo largo de la jerarquía hasta encontrar una equiparación relevante
			- Comenzar en el marco raíz y seleccionar en cada nivel elmarco con mejor VE
			- Buscar marcos relacionados usando las relaciones Fraternal, Disjunto, No-Disjunto o ad hoc.
### Herencia de propiedades
- Herencia simple
	- Un único camino entre el marco instancia con nodo raíz de la jerarquía
	- El valor de la propiedad se busca primero en la instancia, y luego se va subiendo por la jerarquía hasta encontrarlo. Siempre se accede a la  información más específica disponible
- Herencia múltiple
	- Varios caminos entre marco instancia y nodo raíz (forma de grafo)
	- Dificultad: determinar orden en que se exploran padres cuando se sube por la jerarquía, si los padres tienen propiedades con mismo nombre
	- Distintos algoritmos
		- Búsqueda en profundidad
			- Criterios
				- Recorrer de izquierda a derecha
				- Criterio de exhaustividad: evitar búsqueda reiterada de propiedades en marcos clase ya analizados
				- Criterio de especificidad: sólo se puede buscar la propiedad en una clase si previamente se ha buscado en todas sus subclases
			- Algoritmo: procedimiento de ordenación topológica
		- Búsqueda en amplitud: longitud de camino
			- Búsqueda en amplitud con profundidad iterativa
			- Eficiente en grafos sin propiedades repetidas
			- Dos problemas si presenta excepciones:
				- Ambigüedades
				- Conocimientos no especializados
			- Problema adicional: longitud de un camino puede no coincidir con el nivel de generalidad de una clase (clases que no se han especializado con el mismo nivel de detalle que sus hermanas -> se debe evitar)
		- Distancia inferencial (Touretzky)
			- Razona correctamente en BC redundantes, aunque no resuelve situaciones ambiguas.
			- Distancia inferencial: A y B estan a menor distancia que A y C si B está en el camino de A a C <- condición necesaria y suficiente
### Valores activos
- Demonios, valores activos o disparadores: *Si Necesito, Si Añado, Si Modifico, Si Borro*