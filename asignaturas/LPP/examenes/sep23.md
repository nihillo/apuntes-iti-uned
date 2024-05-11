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
- ==Evaluación en cortocircuito: es un procedimiento de evaluación de expresiones de un lenguaje por el cual, para una determinada expresión, en cuanto se obtiene el resultado se dejan de evaluar el resto de opciones.
- ==Evaluación diferida: es una estrategia por la cual sólo se evalúan las expresiones de un lenguaje en el momento en que son necesarias. También se le llama evaluación perezosa.
- ==Evaluación estricta: es una estrategia por la cual se evalúan siempre todas las expresiones, independientemente de que no se vayan a usar. También se le llama evaluación ansiosa.