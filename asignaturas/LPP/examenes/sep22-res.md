## 1
### 1.a
\<object> := '{' \<cuerpo> '}'
\<cuerpo> := \<prop> | \<prop>',' \<cuerpo>
\<prop> := \<string>':'\<value>

### 1.b
La evaluación estricta y la evaluación en diferido son dos diferentes estrategias de evaluación de expresiones seguidas por los lenguajes de programación. Mientras en la evaluación estricta (también llamada ansiosa) se evalúan todas las expresiones de antemano, en la evaluación diferida (también llamada perezosa) no se evalúan hasta que no se va a hacer uso de ellas. Por ejemplo, en evaluación diferida no se evalúan los parámetros de una funcion hasta que no se invoca.
La evaluación estricta es propia de los lenguajes del paradigma imperativo, mientras la diferida es más común en los funcionales.


## 2
### 2.a
### 2.b
Un optimizador de código es la parte de un compilador encargada de realizar modificaciones sobre el código intermedio dirigidas a mejorar su eficiencia.
Entre las opciones de optimización que pueden ejecutar los optimizadores se encuntran hacer que el código sea más rápido y reducir su tamaño final. Algunas otras son la eliminación de código no usado, la evaluación en cortocircuito de expresiones booleanas, la eliminación de comprobación de rangos o desbordamientos de pila, etc.
Las operaciones realizadas por un optimizador se clasifican en dependientes de la máquina, como la reordenación de código o asignación de registros, y las independientes de la máquina, como la eliminación de redundancias.


## 3
### 3.a
Los lenguajes dinámicos son un conjunto de lenguajes cuya principal diferenciación es que tienen tipado dinámico. Esta circunstancia no constituye em sí misma un paradigama de programación, pero les da una serie de particularidades especiales.
Las principales características de estos lenguajes son:
- Tipado dinámico: el tipo de los datos que se asignan a variables no se declara, sino que se infiere directamente del valor. Además, una misma variable puede contener datos de distintos tipos a lo largo de su ciclo de vida. 
- Lenguajes interpretados: estos lenguajes no son compilados, sino que requieren de un intérprete o máquina virtual
- Portabilidad: al ser interpretados, no dependen de un tipo concreto de arquitectura sobre la que ejecutarse, por lo que un mismo programa se puede portar a cualquier máquina.
- Azúcar sintáctico: existen múltiples formas de expresar los mismos conceptos
Estas características les confiere a estos lenguajes la cualidad de tener un ciclo de desarrollo mucho más ágil que los lenguajes compilados y de tipado estático.

###  3.b
```Haskell
data Matriz = M([Fila])
data Fila = F([Integer])
  
dimension :: Matriz -> (Int, Int)
dimension (M(F(fila1):restoFilas)) =
	(length (F(fila1):restoFilas), length fila1)
```


## 4
### 4.a
### 4.b
```console
# /etc/shells: valid login shells
/b/sh
/b/bash
/u/b/bash
/b/rbash
/u/b/rbash
/b/dash
/u/b/dash
```


## 5
### 5.a
ASP, JSP y PHP son todos ellos lenguajes que se pueden embeber en HTML del lado del servidor.
- ASP (Active Server Pages) es un lenguaje desarrollado por Microsoft, ofrecido junto con su tecnología de servidor web IIS (Internet Information Server), en la que puede ser ejecutado.
- JSP (Java Server Pages) es una tecnología del ecosistema de Java que permite embeber scripts de este lenguaje en documentos HTML, de forma que se pueden usar para generar contenido dinámico. Se pueden usar mediante etiquetas, que invocarán clases de Java predefinidas.
- PHP (Hypertext Preprocessor) es un lenguaje open source del lado de servidor que puede correr en distintos servidores web, entre los que destaca principalmente Apache. Puede tanto generar documentos HTML completos como ser embebido en páginas HTML de forma que generará contenido parcial de estas dinámicamente.
### 5.b
- Ortogonalidad: hace referencia a que las características del lenguaje se puedan comprender y combinar de forma independiente unas de otras.
- Integridad conceptual: es la cualidad de un lenguaje de ofrecer un conjunto de conceptos simple, claro y unificado.
- Generalidad: la generalidad de un lenguaje consiste en que sus características se generen a partir de conceptos básicos conocidos por el programador
- Eficiencia: un criterio importante a la hora de elegir un lenguaje es la eficiencia, no sólo de la ejecución de los programas que podamos escribir en el lenguajes, sino también de sus herramientas de procesmiento y de los distintos procesos involucrados en el ciclo de desarrollo.