## Tema 5. Patrones de creación
### Abstract Factory
El objetivo del patrón Abstract Factory es la creación de objetos agrupados en familias sin tener que conocer las clases concretas destinadas a la creación de estos objetos.
#### Participantes
- FabricaAbstracta
- FabricaConcreta1, FabricaConcreta2
- ProductoAbstractoA (ProductoA1, ProductoA2), ProductoAbstractoB (ProductoB1, ProductoB2)
- Cliente
#### Dominios de aplicación
- Sistema necesita ser independiente de la forma en que se crean y agrupan sus productos
- Varias familias de productos que pueden evolucionar
### Builder
El objetivo del patrón Builder es abstraer la construcción de objetos complejos de su implementación, de modo que un cliente pueda crear objetos complejos sin tener que preocuparse de las diferencias en su implantación.
#### Participantes
- ConstructorAbstracto
- ConstructorConcreto
- Producto
- Director
#### Dominios de aplicación
- Construir objetos complejos sin conocer su implementación
- Construir objetos complejos con varias representaciones o implementaciones
### Factory Method
El objetivo del patrón Factory Method es proveer un método abstracto de creacióon de un objeto delegando en las subclases concretas su creación efectiva.
#### Participantes
- CreadorAbstracto
- CreadorConcreto
- Producto
- ProductoConcreto
#### Dominios de aplicación
- Una clase sólo conoce los objetos con que tiene relaciones
- Una clase transmite a sus subclases las eleccciones de instanciación aprovechando polimorfismo
###  Prototype
El objetivo de Prototype es la creación de nuevos objetos mediante duplicación de objetos existentes llamados prototipos que disponen de la capacidad de clonación.
#### Participantes
- Cliente
- Prototype
- PrototypeConcreto1, PrototypeConcreto2
#### Dominios de aplicación
- Un sistema de objetos debe crear instancias sin conocer su jerarquía de clases
- Un sistema de objetos debe crear instancias dinámicamente
- El sistema de objetos debe permanecer simple y no incluir una jerarquía paralela de clases de fabricación
### Singleton
El patrón Singleton tiene como objetivo asegurar que una clase sólo posee una instancia y proporcionar un método de clase único que devuelva esta instancia.
#### Participantes
- Singleton
#### Dominios de aplicación
- Sólo debe existir una instancia de una clase
- Esta instancia sólo debe ser accesible mediante un método de clase

## Tema 6. Patrones estructurales
### Adapter
El objetivo del patrón Adapter es convertir la interfazs de una clase existente en la interfaz esperada por los clientes también existentes de modo que puedan trabajar de manera conjunta. Se trata de conferir a una clase existente una nueva interfaz para responder a las necesidades de los clientes.
#### Participantes
- Cliente
- Interfaz
- Adaptador
- Adaptado
#### Dominios de aplicación
- Integrar en el sistema un objeto cuya interfaz no se corresponde con la requerida por el sistema
- Proveer interfaces múltiples a un objeto en su etapa de diseño
### Bridge
El objetivo del patrón Bridge es separar el aspecto de implementación de un objeto de su aspecto de representación y de interfaz.
De este modo, por un lado la implementación puede encapsularse por completo y por otro lado la implementación y la representación pueden evolucionar de manera independiente y sin que ninguna suponga restricción alguna sobre la otra.
#### Participantes
- ClaseAbstracta
- ClaseConcreta
- Implementacion
- ImplementacionA, ImplementacionB
#### Dominios de aplicación
- Evitar un vínculo demasiado fuerte entre representación e implementación, especialmente cuando la implementación se selecciona en el curso de la aplicación
- Evitar que los cambios en la implementación de los objetos tengan impacto en las interacciones entre estos y sus clientes
- Permitir extensión de representación e implementación mediante creación de nuevas subclases
- Evitar jerarquías de clases demasiado complejas
### Composite
El objetivo del patrón Composite es ofrecer un marco de diseño de una composición de objetos de profundidad variable, diseño que estará basado en un árbol.
Por otro lado, esta composición está encapsulada respecto a los clientes de los objetos que pueden interactuar sin tener que conocer la profundidad de la composición.
#### Participantes:
- Componente - clase abstracta que contiene la interfas de los objetos de la composición, implementa los métodos comunes e introduce la firma de los métodos que gestionan la composición agregando o suprimiendo componentes
- Hoja - clase concreta que describe hojas de la composición
- Compuesto - clase concreta que describe objetos compuestos de la jerarquía. Posee una asociación de agregación con la clase componente.
- Cliente - objetos que acceden a los objetos de la composición y los manipulan.
#### Dominios de aplicación
- Representar jerarquías de composicion de un sistema
- Los clientes deben ignorar si se comunican con objetos compuestos o no
### Decorator
El objetivo del patrón Decorator es agregar dinámicamente funcionalidades suplementarias a un objeto. Esta agregación de funcionalidades no modifica la interfaz del objeto y es transparente de cara a los clientes.
El patrón Decorator constituye una alternativa respecto a la creación de una subclase para enriquecer el objeto.
#### Participantes
- ComponenteAbstracto
- ComponenteConcreto
- Decorador
- DecoradorConcretoA, DecoradorConcretoB
#### Dominios de aplicación
- Sistema agrega dinámicamente funcionalidades a objeto sin modificar su interfaz
- Sistema gestiona funcionalidades que pueden eliminarse dinámicamente
- Uso de herencia para extender objetos no es práctico, puede ocurrir cuando la jerarquía ya es de por sí compleja
### Facade
El objetivo del patrón Facade es agrupar las interfaces de un conjunto de objetos en una interfaz unificada volviendo a este conjunto más fácil de usar por parte de un cliente.
El patrón Facade encapsula la interfaz de cada objeto considerada como interfaz de bajo nivel en una interfaz única de nivel más elevado. La construcción de la interfaz unificada puede necesitar implementar métodos destinados a componer las interfaces de bajo nivel.
#### Participantes
- Fachada
- Clases y componentes del sistema
#### Dominios de aplicación
- Proveer una interfaz simple a un sistema complejo
- Dividir un sistema en subsistemas, la comunicación entre subsistemas se define de forma abstracta a su implementación gracias a fachadas
- Sistematizar la encapsulación de la implementación de un sistema de cara al exterior
### Flyweight
El objetivo del patrón Flyweight es compartir de forma eficaz un conjunto de objetos de granularidad fina.
#### Participantes
- FabricaFlyweight
- Flyweight
- Cliente
#### Dominios de aplicación
- Posibilidad de compartir pequeños objetos
	- Cuando el sistema utiliza un gran número de objetos
	- El almecenamiento de los objetos es costoso
	- Existen numerosos conjuntos de objetos que pueden reemplazarse por algunos objetos compartidos una vez que parte de su estado se vuelve extrínseco
### Proxy
El patrón Proxy tiene como objetivo el diseño de un objeto que sustituye a otro objeto (el sujeto) y que controla el acceso.
El objeto que realiza la sustitución posee la misma interfaz que el sujeto, volviendo la sustitución transparente de cara a los clientes.
#### Participantes
- Sujeto
- SujetoReal
- Proxy
#### Dominios de aplicación
- Proxy virtual
- Proxy remoto
- Proxy de protección
## Tema 7. Patrones de comportamiento
### Chain of Responsibility
El patrón Chain of Responsibility construye una cadena de objetos tal que si un objeto de la cadena no puede responder a la solicitud, puede transmitirla a su sucesor y así sucesivamente hasta que uno de los objetos de la cadena responde.
#### Participantes
- Gestor
- GestorConcreto1, GestorConcreto2
- Cliente
#### Dominios de aplicación
- Cadena de objetos gestiona solicitud según orden definido dinámicamente
- Forma en que una cadena gestiona una solicitud no tiene por qué conocerse en sus clientes
### Command
El patrón Command tiene como objetivo transformar una solicitud en un objeto, facilitando operaciones tales como la anulación, el encolamiento de solicitudes y su seguimiento.
#### Participantes
- Cliente
- Solicitante
- Solicitud
- SolicitudConcreta
- Receptor
#### Dominios de aplicación
- Objeto debe configurars epara realizar un porcesamiento concreto
- Las solicitudes deben poder encolarse y ejecutarse en un momento cualquiera
- Las solicitudes pueden ser anuladas
- Las solicitudes deben quedar registradas en un archivo de log
- Las solicitudes deben estar reagrupadas bajo la forma de una transacción
### Interpreter
El patrón Interpreter proporciona un marco para representar mediante objetos la gramática de un lenguaje con el fin de evaluar, interpretándolas, expresiones escritas en este lenguaje.
#### Participantes
- Expresion
- Operador
- OperadorConcreto1, OperadorConcreto2
- ElementoTerminal
- ElementoTerminalConcreto1, ElementoTerminalConcreto2
#### Dominios de aplicación
- La gramática de las expresiones es simple
- La evaluación no necesita ser rápida
### Iterator
El patrón Iterator proporciona un acceso secuencial a una colección de objetos a los clientes sin que éstos tengan que preocuparse de la implementación de esta colección.
#### Participantes
- Coleccion
- ColeccionConcreta
- Elemento
- ElementoConcreto
- Iterador
- IteradorConcreto
#### Dominios de aplicación
- Recorrer una colección sin acceder a la representación interna de esta
- Debe ser posible gestionar varios recorridos de forma simultanea
### Mediator
El patrón Mediator tiene como objetivo construir un objeto cuya vocación es la gestión y el control de las interacciones en un conjunto de objetos sin que sus elementos deban conocerse mutuamente.
#### Participantes
- Mediador
- MediadorConcreto
- Elemento
- ElementoConcreto1, ElementoConcreto2
#### Dominios de aplicación
- Conjunto de objetos basado en comunicación compleja que conduce a asociar numerosos objetos entre ellos
- Objetos difíciles de reutilizar debido a sus asociaciones con otros objetos
- Modularidad del sistema mediocre, obligando a escribir numerosas subclases cuando se debe adaptar una parte del sistema
### Memento
El patrón Memento tiene como objetivo salvaguardar y restablecer el estado de un objeto sin violar la encapsulación.
#### Participantes
- ObjetoOriginal
- Memento
- GestionEstado
#### Dominios de aplicación
- Estado interno de un objeto debe memorizarse para poder ser restaurado posteriormente sin que la encapsulación quede fragmentada
### Observer
El patrón Observer tiene como objetivo construir una dependencia entre un sujeto y los observadores de modo que cada modificación del sujeto sea notificada a los observadores para que puedan actualizar su estado.
#### Participantes
- Sujeto
- SujetoConcreto
- Observador
- ObservadorConcreto
#### Dominios de aplicación
- Modificación en el estado de un objeto genera modificaciones en otros objetos que se determinan dinámicamente
- Objeto avisa a otros objetos sin tener que conocer su tipo (estar fuertemente acoplado con ellos)
- No se desea fusionar dos objetos en uno solo
### State
El patrón State permite a un objeto adaptar su comportamiento en función de su estado interno.
#### Participantes
- MaquinaEstados
- Estado
- EstadoConcretoA, EstadoConcretoB
#### Dominios de aplicación
- El comportamiento de un objeto depende de su estado
- La implementación de esta dependencia mediante instrucciones condicionales se vuelve muy compleja
### Strategy
El patrón strategy tiene como objetivo adaptar el comportamiento y los algoritmos de un objeto en función de una necesidad sin cambiar las interacciones de este objeto con los clientes.
#### Participantes
- Entidad
- Estrategia
- EstrategiaConcretaA, EstrategiaConcretaB
#### Dominios de aplicación
- El comportamiento de una clase puede estar implementado mediante distintos algoritmos
- La implementación de elección del algoritmo mediante condicionales se vuelve compleja
- Un sistema posee numerosas clases idénticas salvo una parte correspondiente a su comportamiento
### Template method
El patrón Template Method permite delegar en las subclases ciertas etapas de una de las operaciones de un objeto, estando estas etapas descritas en las subclases.
#### Participantes
- Clase Abstracta
- Clase Concreta
#### Dominios de aplicación
- Una clase compartida con otra u otras clases con código idéntico que puede factorizarse siempre que las partes específicas a cada clase hayan sido desplazadas a nuevos métodos
- Un algoritmo posee una parte invariable y partes específicas a distintos tipos de objetos
### Visitor
El patrón Visitor construye una operación que debe realizarse sobre los elementos de un conjunto de objetos. Esto permite agregar nuevas operaciones sin modificar las clases de estos objetos.
#### Participantes
- Elemento
- ElementoConcreto1, ElementoConcreto2
- Visitante
- VisitanteConcreto1, VisitanteConcreto2
#### Dominios de aplicación
- Es necesario agragar numerosas funcionalidades a un conjunto de clases sin volverlas pesadas
- Un conjunto de clases poseen una estructura fija y es necesario agregarles funcionalidades sin modificar su interfaz
