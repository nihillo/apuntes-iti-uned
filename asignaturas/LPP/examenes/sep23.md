## 1
### 1.a
A la vista del árbol de derivación de la gramática:

- oración
	- sintagma-nominal
		- artículo
			- a
			- the
		- sustantivo
			- girl
			- dog
	- sintagma-verbal
		- verbo
			- sees
			- pets
		- sintagma-nominal
			- artículo
				- a
				- the
			- sustantivo
				- girl
				- dog

Vemos que que toda oración se compone de exactamente 5 palabras, para cada una de las cuales hay 2 alternativas.
Por tanto, el número de oraciones posibles es 2^5 = 32.

### 1.b
- Evaluación en cortocircuito: es un procedimiento de evaluación de expresiones de un lenguaje por el cual, para una determinada expresión, en cuanto se obtiene el resultado se dejan de evaluar el resto de opciones. Esto adquiere relevancia por ejemplo en expresiones con operadores de conjunción o disyunción. En algunos casos de estas, el primer operando puede devolver ya un resultado para la expresión completa, en cuyo caso no se evalúa el segundo operando.
- Evaluación diferida: es una estrategia por la cual sólo se evalúan las expresiones de un lenguaje en el momento en que son necesarias. También se le llama evaluación perezosa. Esta forma de evaluación se usa especialmente en lenguajes funcionales.
- Evaluación estricta: es una estrategia por la cual se evalúan siempre todas las expresiones, independientemente de que no se vayan a usar. También se le llama evaluación ansiosa. Esta forma de evaluación se usa sobre todo en lenguajes imperativos.

## 2
### 2.a
(1) S -> ASB
(5) ASB -> aASB
(2) aASB -> abSB
(4) abSB -> abdB
(6) abdB ->abddcd

- S 
	- A
		- a
		- A
			- b
	- S
		- d
	- B
		- d
		- c
		- d

### 2.b
El análisis sintáctico ascendente es un procedimiento de análisis sintáctico por el cual se construye el árbol de análisis sintáctico desde las hojas a la raíz, recorriendo las cadenas de izquierda a derecha y sustituyendo durante el proceso aquellos fragmentos en que se identifiquen consecuentes de las reglas de producción por los antecedentes de estas, hasta llegar al símbolo inicial de la gramática que será la raíz del árbol
Se corresponde con un recorrido en postorden, ya que primero se reconocen los hijos y luego, mediante reducciones, se reconoce el padre.
A estos métodos de análisis Shift-reduce (desplazar-reducir). Se conoce así porque durante el análisis, en cada iteración, se tiene la cadena de entrada y una pila en la que se van acumulando los estados que se han procesado de ella, leyendo desde la izquierda. Las operaciones que se realizan en cada paso son, o bien un desplazamiento del primer símbolo de la cadena de entrada hacia la pila (shift) o bien una reducción de lo que tengamos en la cima de la pila al antecedente de su regla de producción correspondiente (reduce).
Los métodos de análisis sintáctico ascendente (LR) permiten reconocer la mayoría de las construcciones de los lenguajes de programación y son más potentes que los descendentes (LL).

## 3
### 3.a
```Prolog
antepasado(X,Y) :-
	hijo(Y,X).
	
antepasado(X,Y) :-
	hijo(Y,Z),
	antepasado(X,Z).
```

### 3.b
Existen tres tipos de sincronización de procesos en la programación concurrente: 
- Sincronización condicional: un determinado proceso debe esperar a que se active una determinada condición que sólo puede ser activada por otro proceso. 
- Exclusión mutua: se da cuando los procesos compiten por el acceso a un recurso compartido que sólo se puede usar por un proceso a la vez. La sección crítica es el conjunto de instrucciones que sólo pueden ser ejectuadas por un proceso a la vez. Los procesos deben sincronizarse de forma que cuando está siendo ejecutada por uno, los demás que desean acceder a ella deben esperar.
- Sincronización de barrera: tipo especial de sincronización que se da para la casuística en que un conjunto de procesos ejecutan una serie de acciones de forma secuencial, de tal forma que una determinada acción no puede ser ejecutada por ningún proceso hasta que no se haya ejecutado la anterior por todos ellos.
Hay diferentes herramientas que pueden usar los lenguajes para la sincronización de procesos. Una de las más básicas y conocidas es el uso de semáforos.
Un semáforo es un tipo abstracto de datos que contiene los siguientes atributos
- un contador de valores positivos, incluido el 0
- una lista de procesos asociados
- una serie de operaciones: initial, wait y signal
La operación initial inincializa el semáforo poniendo el contador al valor que se indique.
La operación wait permite que el proceso que la invoca continúe si el contador tiene un valor mayor que 0, decrementando el contador, o que se bloquée (añadiéndolo a la lista de bloqueados) si el valor es 0.
La operación signal incrementa el contador si no hay procesos bloqueados, o en caso contrario ejecuta aleatoriamente uno de los procesos bloqueados, manteniendo entonces el contador inalterado.

