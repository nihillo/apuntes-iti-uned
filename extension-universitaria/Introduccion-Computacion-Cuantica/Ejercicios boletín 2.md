**Curso de Introducción a la Computación Cuántica. UNED.** 
Alumno: Juan R. Barranco Esteban

---
## Ejercicios

**1\. Para cada una de las preguntas a continuación, suponer un sistema de dos qubits que comienza en el siguiente estado:**

$\ket{\psi} = \frac{1}{2}\ket{00} + \frac{1}{2}\ket{10} + \frac{1}{2}\ket{11}$

**a) ¿Cuál es la probabilidad de medir ambos qubits como 0?**

La probabilidad es el cuadrado de la amplitud de probabilidad del término $\ket{00}$, en este caso $(\frac{1}{2})^2 = \frac{1}{4}$


**b) ¿Cuál es la probabilidad de medir el primer qubit como 1?**

En este caso, la probabilidad es la suma  de los cuadrados de las amplitudes de probabilidad de los términos $\ket{10}$ y $\ket{10}$, es decir $(\frac{1}{2})^2 + (\frac{1}{2})^2 = \frac{1}{2}$.


**c) ¿Cuál es la probabilidad de medir el segundo qubit como 0?**

De forma análoga, la probabilidad es la suma  de los cuadrados de las amplitudes de probabilidad de los estados $\ket{00}$ y $\ket{11}$, es decir $(\frac{1}{\sqrt{2}})^2 + (\frac{1}{2})^2 = \frac{1}{2} + \frac{1}{4} = \frac{3}{4}$.


**d) ¿Cuál es el nuevo estado del sistema después de medir el primer qubit como 0?**

Tras la medición, el sistema se compondría de dos bits clásicos, con valor 0 en ambos.


**e) ¿Cuál es el nuevo estado del sistema después de medir el primer qubit como 1?**

Tras la medición, el sistema se compondría de dos bits clásicos, el primero de ellos con valor 1, y el segundo no lo sabemos de antemano pero puede ser 0 o 1 con probabilidades $P(0) = P(1) = \frac{1}{2}$.


**2\. Se lanzan dos monedas. ¿Cuál es el estado del sistema de dos monedas mientras están en el aire?**

Si representamos cada moneda como un qubit donde el valor 0 es cara, y el valor 1 es cruz, el estado del sistema mientras están en el aire es:

$\ket{\psi} = \frac{1}{2} (\ket{00} + \ket{01} + \ket{10} + \ket{11})$




**3\. Se lanzan dos dados de seis caras. ¿Cuál es la probabilidad total de obtener un número par en un dado y uno impar en el otro?**

Dado que, para cada dado, la mitad de las caras son pares y la mitad impares, se puede representar el sistema de una forma simplificada mediante dos qubits, uno por dado, en los que consideremos el valor 0 como uno cualquiera de los tres valores pares, y el valor 1 como uno cualquiera de los tres valores impares.

En estos términos, el sistema queda representado por el estado:

$\ket{\psi} = \frac{1}{2} (\ket{00} + \ket{01} + \ket{10} + \ket{11})$

La probabilidad viene dada por la suma de los cuadrados de las amplitudes de probabilidad de los estados $\ket{01}$ y  $\ket{10}$, es decir

$(\frac{1}{2})^2 + (\frac{1}{2})^2 = \frac{1}{4} + \frac{1}{4} = \frac{1}{2}$




**4\. ¿Es $\frac{1}{\sqrt{2}}\ket{00} + \frac{1}{\sqrt{2}}\ket{01}$ un estado entrelazado? Si es así, prueba que no se puede escribir como un producto. Si no, ¿cuál es el estado individual de los dos qubits?**

Un estado de dos qubits $\ket{\psi}$ no está entrelazado si se puede escribier como el producto de dos estados individuales:

$\ket{\psi} = (\alpha_0\ket{0} + \alpha_1\ket{1}) \otimes (\beta_0\ket{0} + \beta_1\ket{1})$

Expandiendo el producto tensorial:

$\ket{\psi} = \alpha_0\beta_0\ket{00} + \alpha_0\beta_1\ket{01} + \alpha_1\beta_0\ket{10} + \alpha_1\beta_1\ket{11}$

Si comparamos con el estado dado

$\ket{\psi} = \frac{1}{\sqrt{2}}\ket{00} + \frac{1}{\sqrt{2}}\ket{01}$

tenemos:

$\alpha_0\beta_0\ = \frac{1}{\sqrt{2}}$,
$\alpha_0\beta_1 = \frac{1}{\sqrt{2}}$,
$\alpha_1\beta_0 = 0$,
$\alpha_1\beta_1 = 0$

Se puede verificar que estas igualdades se cumplen para los valores

$\alpha_0 = 1, \quad \alpha_1 = 0, \quad \beta_0 = \frac{1}{\sqrt{2}}, \ \quad \beta_1 = \frac{1}{\sqrt{2}}$

con lo que tenemos

$\ket{\psi} = 1 \cdot \frac{1}{\sqrt{2}}\ket{00} + 1 \cdot \frac{1}{\sqrt{2}}\ket{01} + 0 \cdot \frac{1}{\sqrt{2}}\ket{10} + 0 \cdot \frac{1}{\sqrt{2}}\ket{11} = \frac{1}{\sqrt{2}}\ket{00} + \frac{1}{\sqrt{2}}\ket{01}$

Podemos concluir, por tanto, que el estado no está entrelazado.




**5\. ¿Están los siguientes estados de dos qubits entrelazados?**

**a) $\frac{1}{\sqrt{2}}\ket{01} + \frac{1}{\sqrt{2}}\ket{10}$**

Siguiendo el mismo curso de deducción que en el ejercicio anterior, tenemos en este caso: 

$\alpha_0\beta_0\ = 0$,
$\alpha_0\beta_1 = \frac{1}{\sqrt{2}}$,
$\alpha_1\beta_0 = \frac{1}{\sqrt{2}}$,
$\alpha_1\beta_1 = 0$

De las dos primeras ecuaciones se obtiene que $\beta_0 = 0$, pero esto no es consistente con la tercera. Por tanto, el sistema no puede expresarse como combinación lineal y podemos concluir que sí está entrelazado.


**b) $\frac{1}{\sqrt{2}}\ket{01} - \frac{1}{\sqrt{2}}\ket{10}$**

$\alpha_0\beta_0\ = 0$,
$\alpha_0\beta_1 = \frac{1}{\sqrt{2}}$,
$\alpha_1\beta_0 = -\frac{1}{\sqrt{2}}$,
$\alpha_1\beta_1 = 0$

Ocurre exactamente lo mismo que en el caso anterior (de las dos primeras igualdades se obtiene que $\beta_0 = 0$, pero esto es inconsistente con la tercera), por lo que el estado está entrelazado.


**c) $\frac{\sqrt{3}}{2}\ket{00} - \frac{1}{2}\ket{11}$**

$\alpha_0\beta_0\ = \frac{\sqrt{3}}{2}$,
$\alpha_0\beta_1 = 0$,
$\alpha_1\beta_0 = 0$,
$\alpha_1\beta_1 = \frac{1}{2}$

El sistema de ecuaciones no tiene solución: de las primeras ecuaciones se sigue que $\beta_1 = 0$, lo cual es inconsistente con la cuarta ecuación. Por tanto los qubits están entrelazados.


**d) $\frac{1}{\sqrt{2}}\ket{10} + \frac{1}{\sqrt{2}}\ket{11}$**

$\alpha_0\beta_0\ = 0$,
$\alpha_0\beta_1 = 0$,
$\alpha_1\beta_0 = \frac{1}{2}$,
$\alpha_1\beta_1 = \frac{1}{2}$

El sistema tiene solución para $\alpha_0 = 0, \quad \alpha_1 = \frac{1}{2}, \quad \beta_0 = \beta_1 = 1$. Los qubits no están entrelazados.


**e) $\frac{1}{2}\ket{00} + \frac{1}{2}\ket{01} + \frac{1}{2}\ket{10} + \frac{1}{2}\ket{11}$**

$\alpha_0\beta_0\ = \frac{1}{2}$,
$\alpha_0\beta_1 = \frac{1}{2}$,
$\alpha_1\beta_0 = \frac{1}{2}$,
$\alpha_1\beta_1 = \frac{1}{2}$

El sistema tiene solucion, por tanto los qubits no están entrelazados.


**f) $\frac{1}{\sqrt{2}}\ket{00}  + \frac{1}{2}\ket{10} + \frac{1}{2}\ket{11}$**

$\alpha_0\beta_0\ = \frac{1}{\sqrt{2}}$,
$\alpha_0\beta_1 = 0$,
$\alpha_1\beta_0 = \frac{1}{2}$,
$\alpha_1\beta_1 = \frac{1}{2}$

El sistema de ecuaciones no tiene solución: de las primeras ecuaciones se sigue que $\beta_1 = 0$, lo cual es inconsistente con la cuarta ecuación. Por tanto los qubits están entrelazados.




**6\. Dos qubits pasan por una puerta CNOT. El primer qubit es el de control. ¿Cuál es la salida para los siguientes estados iniciales?**

**a) $\ket{00}$**

Para esta entrada, la salida es $\ket{00}$ ya que al ser $\ket{0}$ el primer qubit, el segundo no se altera.


**b) $\ket{01}$**

De forma análoga al apartado anterior, la salida es $\ket{01}$.


**c) $\ket{11}$**

En este caso, al tener el primer qubit a $\ket{1}$, el segundo se modifica, por lo que la salida es $\ket{10}$.


**c) $\frac{1}{\sqrt{2}}\ket{01} + \frac{1}{\sqrt{2}}\ket{10}$**

Aquí tenemos una superposición de dos estados, por lo que la salida será también una superposición de estados, cada uno el resultante de cada uno de los de la entrada: 

$\frac{1}{\sqrt{2}}\ket{01} + \frac{1}{\sqrt{2}}\ket{11}$


**d) $\frac{1}{\sqrt{2}}\ket{00} + \frac{1}{2}\ket{10} - \frac{1}{2}\ket{11}$**

De forma análoga al apartado anterior:

$\frac{1}{\sqrt{2}}\ket{00} + \frac{1}{2}\ket{11} - \frac{1}{2}\ket{10}$




**7\. La salida de una puerta CNOT es la que se muestra en la figura. ¿Cuál es la entrada?**

![[Pasted image 20250403070155.png]]

Vemos que el qubit de control es $\ket{0}$ por lo que la entrada será necesariamente igual que la salida: $\ket{01}$




**8\. ¿Puedes predecir el estado producido por estos circuitos?

![[Pasted image 20250403070435.png]]

Tenemos primero una puerta CNOT que no tiene efecto ya que el qubit de control es $\ket{0}$ y despues una $X$ sobre el segundo qubit, por lo que la salida será $\ket{01}$


![[Pasted image 20250403070620.png]]

La puerta $X$ invierte el primer qubit, y la CNOT no hace nada porque el de control es $\ket{0}$: salida $\ket{10}$


   ![[Pasted image 20250403070744.png]]

La puerta $X$ invierte el segundo qubit, que pasa a ser $\ket{1}$. Éste es el qubit de control de la puerta CNOT, por lo que tras esta el primer qubit pasa a $\ket{1}$. Estado final: $\ket{11}$

   
![[Pasted image 20250403070950.png]]
Ambos qubits se invierten al principio. Luego en la puerta CNOT se invierte el primero, resultando en la salida $\ket{01}$.




**10\. ¿Puedes predecir el estado producido por este circuito?

![[Pasted image 20250403073021.png]]

La puerta de Hadamard sobre el primer qubit pasará el estado inicial a

$\frac{1}{\sqrt{2}}(\ket{00} + \ket{10})$

Posteriormente, la puerta CNOT con el segundo qubit como control no tendrá efecto sobre ninguno de los dos componentes de la superposición, al tener ambos $\ket{0}$ en el segundo qubit. Por tanto, la salida será:

$\frac{1}{\sqrt{2}}(\ket{00} + \ket{10})$

