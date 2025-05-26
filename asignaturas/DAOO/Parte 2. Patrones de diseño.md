## Tema 5. Patrones de creación
### Abstract Factory
### Builder
### Factory Method
###  Prototype
### Singleton
## Tema 6. Patrones estructurales
### Adapter
### Bridge
### Composite
El objetivo del patrón Composite es ofrecer un marco de diseño de una composición de objetos de profundidad variable, diseño que estará basado en un árbol.
Por otro lado, esta composición está encapsulada respecto a los clientes de los objetos que pueden interactuar sin tener que conocer la profundidad de la composición.
### Decorator
El objetivo del patrón Decorator es agregar dinámicamente funcionalidades suplementarias a un objeto. Esta agregación de funcionalidades no modifica la interfaz del objeto y es transparente de cara a los clientes.
El patrón Decorator constituye una alternativa respecto a la creación de una subclase para enriquecer el objeto.
#### Dominios de aplicación
- Sistema agrega dinámicamente funcionalidades a objeto sin modificar su interfaz
- Sistema gestiona funcionalidades que pueden eliminarse dinámicamente
- Uso de herencia para extender objetos no es práctico, puede ocurrir cuando la jerarquía ya es de por sí compleja
### Facade
El objetivo del patrón Facade es agrupar las interfaces de un conjunto de objetos en una interfaz unificada volviendo a este conjunto más fácil de usar por parte de un cliente.
El patrón Facade encapsula la interfaz de cada objeto considerada como interfaz de bajo nivel en una interfaz única de nivel más elevado. La construcción de la interfaz unificada puede necesitar implementar métodos destinados a componer las interfaces de bajo nivel.
### Flyweight
El objetivo del patrón Flyweight es compartir de forma eficaz un conjunto de objetos de granularidad fina.
#### Participantes
- FabricaFlyweight
- Flyweight
- Cliente
### Proxy
El patrón Proxy tiene como objetivo el diseño de un objeto que sustituye a otro objeto (el sujeto) y que controla el acceso.
El objeto que realiza la sustitución posee la misma interfaz que el sujeto, volviendo la sustitución transparente de cara a los clientes.
## Tema 7. Patrones de comportamiento
### Chain of Responsibility
El patrón Chain of Responsibility construye una cadena de objetos tal que si un objeto de la cadena no puede responder a la solicitud, puede transmitirla a su sucesor y así sucesivamente hasta que uno de los objetos de la cadena responde.
### Command
El patrón Command tiene como objetivo transformar una solicitud en un objeto, facilitando operaciones tales como la anulación, el encolamiento de solicitudes y su seguimiento.
### Interpreter
### Iterator
El patrón Iterator proporciona un acceso secuencial a a una colección de objetos a los clientes sin que éstos tengan que preocuparse de la implementación de esta colección.
### Mediator
El patrón Mediator tiene como objetivo construir un objeto cuya vocación es la gestión y el control de las interacciones en un conjunto de objetos sin que sus elementos deban conocerse mutuamente
### Memento
El patrón Memento tiene como objetivo salvaguardar y restablecer el estado de un objeto sin violar la encapsulación.
### Observer
El patrón Observer tiene como objetivo construir una dependencia entre un sujeto y los observadores de modo que cada modificación del sujeto sea notificada a los observadores para que puedan actualizar su estado.
### State
El patrón State permite a un objeto adaptar su comportamiento en función de su estado interno.

### Strategy
El patrón strategy tiene como objetivo adaptar el comportamiento y los algoritmos de un objeto en función de una necesidad sin cambiar las interacciones de este objeto con los clientes.
### Template method
El patrón Template Method permite delegar en las subclases ciertas etapas de una de las operaciones de un objeto, estando estas etapas descritas en las subclases.
#### Participantes
- Clase Abstracta
- Clase Concreta
### Visitor
El patrón Visitor construye una operación que debe realizarse sobre los elementos de un conjunto de objetos. Esto permite agregar nuevas operaciones sin modificar las clases de estos objetos.

