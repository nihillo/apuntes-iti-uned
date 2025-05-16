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
- Clasificación: encontrar los marcos clase (uno o varios) de la BC que describen más consistentemente al marco pregunta
- Etapas:
	- Selección de marcos candidatos
	- Cálculo de valores de equiparación
	- Decisión
### Herencia de propiedades
- Herencia simple
	- Un único camino entre el marco instancia con nodo raíz de la jerarquía
	- Algoritmo:
		- Se busca la propiedad ne marco instancia
		- Sebusca la propiedad en marco clase, y subiendo por la jerarquía de herencia hasta encontrar un nodo en que se encuentre la propiedad
		- Se busca la propiedad en el nodo raíz
	- Facetas *Si Necesito* y valor por omisión también pueden responder a la pregunta. En caso de estar definidas ambas debe existir estrategia de control que ayude a decidir entre una y otra.
- Herencia múltiple
	- Varios caminos entre marco instancia y nodo raíz
	- Dificultad: determinar orden en que se exploran padres cuando se sube por la jerarquía, si los padres tienen propiedades con mismo nombre
	- Distintos algoritmos
		- Búsqueda en profundidad
			- Criterios
				- Recorrer de izquierda a derecha
				- Crietrio de exhaustividad: evitar búsqueda reiterada de propiedades en marcos clase ya analizados
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