
Alumno: Juan R. Barranco Esteban

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Boletín de ejercicios 1


**1\. Determinar el estado del sistema formado por los qubits cuyo estado se indica:**

$\ket{\psi_1} = u_1 \ket{0} + v_1 \ket{1}$
$\ket{\psi_2} = u_2 \ket{0} + v_2 \ket{1}$

El estado de un sistema de dos qubits se obtiene mediante el producto tensorial de los estados de cada uno de los qubits. Por tanto, el estado de este sistema será:
$\ket{\psi} = (u_1 \ket{0} + v_1 \ket{1})  \otimes (u_2 \ket{0} + v_2 \ket{1}) = u_1u_2\ket{00} + u_1v_2\ket{01} + v_1u_2\ket{10} + v_1v_2\ket{11}$



**2\. Indicar**
**a) el bra asociado al ket $\ket{\psi}$** 

El bra asociado a un ket se calcula obteniendo su conjugado transpuesto (operador adjunto).
El bra asociado a $\ket{\psi}$ es por tanto, 

$\bra{\psi} = \ket{\psi}^{\dagger}$

Suponiendo que el ket tenga la forma 

$\ket{\psi} = \sum_i{c_i}\ket{i}$

entonces su bra asociado será

$\bra{\psi} = \sum_{i}{c^{*}_i\bra{i}}$

donde $c^*_i$ es el conjugado complejo de $c_i$.


**b) el ket asociado al bra $\bra{\psi}$**
El ket asociado a un bra se obtiene de igual modo calculando el adjunto del bra:

$\ket{\psi} = \bra{\psi}^{\dagger}$




**3\. Dado el qubit $\ket{\psi} = u\ket{0} + v\ket{1}$, escribir el bra asociado**

Como se ha dicho anteriormente, el bra asociado a un ket es el adjunto de este (conjugado transpuesto).

Dado 

$\ket{\psi} = u\ket{0} + v\ket{1}$

donde  $u, v \in \mathbb{C}$, los kets $\ket{0}$ y $\ket{1}$ tienen las formas matriciales

$\ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad \ket{1} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$

entonces $\ket{\psi}$ tiene la forma matricial

$\ket{\psi} = \begin{bmatrix} u \\ v \end{bmatrix}$

Para obtener el bra tomamos el adjunto:

$\bra{\psi} = \ket{\psi}^{\dagger} = (u\ket{0} + v\ket{1})^{\dagger}$ 

$\bra{\psi} = u^{*} \bra{0} + v^{*}\bra{1}$

En forma matricial:

$\bra{\psi} = \begin{bmatrix} u^{*} \quad v^{*} \end{bmatrix}$




**4\. Calcula el producto escalar de los vectores:

$\ket{\psi_1} = u_1 \ket{0} + v_1 \ket{1}$
$\ket{\psi_2} = u_2 \ket{0} + v_2 \ket{1}$

El producto escalar entre dos vectores se define en notación de Dirac como

$\braket{\psi_1 | \psi_2}$ 

El bra $\bra{\psi_1}$ correspondiente a  $\ket{\psi_1}$ es:

$\bra{\psi_1} = u^{*}_1\bra{0} + v^{*}_1\bra{1}$

Por tanto el producto escalar de estos vectores es

$\braket{\psi_1 | \psi_2} = (u^{*}_1\bra{0} + v^{*}_1\bra{1})(u_2 \ket{0} + v_2 \ket{1})$

Si lo expresamos en forma matricial, en términos de la base computacional:

$\braket{\psi_1 | \psi_2} = \begin{bmatrix} u_1^{*} \quad v_1^{*} \end{bmatrix} \begin{bmatrix} u_2 \\ v_2 \end{bmatrix} = u_1^{*} u_2 + v_1^{*}  v_2$  




**5\. Comprobar que las matrices de Pauli son hermíticas y unitarias:
$\forall k \in \{1, 2, 3\} \quad \sigma_k = \sigma_k^{\dagger} = \sigma_k^{-1}$

Una matriz hermítica es aquella que es igual a su adjunta: $\sigma_k = \sigma_k^{\dagger}$

Una matriz unitaria es aquella cuyo producto por su adjunta es la matriz identidad:  $\sigma_k \sigma_k^{\dagger} = I$ (o dicho de otro modo, aquella que es igual a su inversa $\sigma_k = \sigma_k^{-1}$).

Las matrices de pauli son:

$\sigma_1 = \begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix}, \quad \sigma_2 = \begin{pmatrix}0 & -i \\ i &  0 \end{pmatrix}, \quad \sigma_3 = \begin{pmatrix}1 & 0 \\ 0 & -1 \end{pmatrix}$  

Verificaciones:
- $\sigma_1$:
	- $\sigma_1^{\dagger} = \begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix} = \sigma_1$, por lo que es hermítica.
	- $\sigma_1 \sigma_1^{\dagger} = \begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1 \end{pmatrix} = I$, por lo que es unitaria. 
- $\sigma_2$:
	- $\sigma_2^{\dagger} = \begin{pmatrix}0 & -i \\ i & 0 \end{pmatrix} = \sigma_2$, por lo que es hermítica.
	-  $\sigma_2 \sigma_2^{\dagger} = \begin{pmatrix}0 & -i \\ i & 0 \end{pmatrix}\begin{pmatrix}0 & -i \\ i & 0 \end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1 \end{pmatrix} = I$, por lo que es unitaria. 
- $\sigma_3$:
	- $\sigma_3^{\dagger} = \begin{pmatrix}1 & 0 \\ 0 & -1 \end{pmatrix} = \sigma_3$, por lo que es hermítica.
	-  $\sigma_3 \sigma_3^{\dagger} = \begin{pmatrix}1 & 0 \\ 0 & -1 \end{pmatrix}\begin{pmatrix}1 & 0 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1 \end{pmatrix} = I$, por lo que es unitaria. 




**6\. Calcular los productos tensoriales de:
a) $\sigma_1 \otimes \sigma_2$

$\sigma_1 \otimes \sigma_2 = \begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix} \otimes \begin{pmatrix}0 & -i \\ i &  0 \end{pmatrix} = \begin{pmatrix} 0 & 0 & 0 & -i \\ 0 & 0 & i & 0 \\0 & -i & 0 & 0 \\ i & 0 & 0 & 0 \end{pmatrix}$


**b) $\sigma_2 \otimes \sigma_1$**

$\sigma_2 \otimes \sigma_1 = \begin{pmatrix}0 & -i \\ i &  0 \end{pmatrix} \otimes \begin{pmatrix}0 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 0 & 0 & 0 & -i \\ 0 & 0 & -i & 0 \\0 & i & 0 & 0 \\ i & 0 & 0 & 0 \end{pmatrix}$




**7\. Un conjunto de qubits se encuentran en el estado**

$\ket{\psi} = \frac{1}{3}(\ket{001} + \ket{010} + \sqrt{7}\ket{100})$

**¿Cuál es la probabilidad de que la medida del primer qubit (el de más a la izquierda) sea 1?**

El posible estado en que el primer qubit sea uno es $\ket{100}$

cuya amplitud de probabilidad es $\frac{\sqrt{7}}{3}$

por tanto, su probabilidad, que es el cuadrado de la amplitud de probabilidad, será:

$(\frac{\sqrt{7}}{3})^{2} = \frac{7}{9}$




**8\. Dado el vector v, ¿qué estado físico podría describir?**
$v = \begin{bmatrix}5 + 3i \\ 6i\end{bmatrix}$

Normalizamos en primer lugar el vector

$|v| = \sqrt{(5^2 + 3^2) + (6^2)} = \sqrt{34 + 36} = \sqrt{70}$

$v' = \frac{1}{\sqrt{70}} \begin{bmatrix}5 + 3i \\ 6i\end{bmatrix}$

Por tanto, expresado en la base computacional, $v$ representa el estado de un qubit que se expresa a continuación:

$\ket{\psi} = \frac{1}{\sqrt{70}}\left[(5 + 3i)\ket{0} + 6i\ket{1}\right]$




**9\. Si se tiene el siguiente circuito cuántico:**

![[Pasted image 20250330120119.png]]

**Determinar el estado a la salida si la entrada es $\ket{11}$**

En el primer paso se aplica una puerta de Hadamard al qubit $q1$. Teniendo en cuenta que suponemos que a la entrada este qubit tendrá $\ket{1}$, la transformación que se aplicará en este paso será:

$H\ket{1} = \frac{1}{\sqrt{2}}(\ket{0} - \ket{1})$

Por tanto, el estado del sistema tras esto será

$\frac{1}{\sqrt{2}}(\ket{0} - \ket{1}) \otimes \ket{1} = \frac{1}{\sqrt{2}}(\ket{01} - \ket{11})$

Posteriormente se aplica una puerta CNOT sobre $q2$ con $q1$ como control. Esta puerta invierte el qubit objetivo cuando el de control es $\ket{1}$, y lo deja inalterado cuando es $\ket{0}$. Por tanto, esta puerta no modificará el término $\ket{01}$ y transformará el $\ket{11}$ en $\ket{10}$, por lo que el estado tras esto será:

$\frac{1}{\sqrt{2}}(\ket{01} - \ket{10})$

Finalmente, tenemos otra puerta de Hadamard sobre $q1$. En este paso tenemos dos términos, $\ket{01}$ y $\ket{10}$, por lo que deben aplicarse:

$H\ket{0} = \frac{1}{\sqrt{2}}(\ket{0} + \ket{1})$
$H\ket{1} = \frac{1}{\sqrt{2}}(\ket{0} - \ket{1})$

Lo cual aplicado al estado actual del sistema nos dará

$\frac{1}{\sqrt{2}}\left[\frac{1}{\sqrt{2}}(\ket{0} + \ket{1}) \otimes \ket{1} - \frac{1}{\sqrt{2}}(\ket{0} - \ket{1}) \otimes \ket{0} \right]$

Simplificando:

$\frac{1}{2}\left[ (\ket{01} +\ket{11}) - (\ket{00} - \ket{10}) \right]$

$= \frac{1}{2}(\ket{00} +\ket{01} + \ket{10} + \ket{11})$




**10\. Probar que se cumplen las siguientes relaciones:**

**(i) $X^2 = Y^2 = Z^2 = I$**
Las puertas lógicas $X$, $Y$ y $Z$ están representadas por las matrices de Pauli, las cuales ya se ha visto anteriormente que, en los tres casos:
- Son hermíticas, es decir, son iguales a sus adjuntas: $\sigma_k = \sigma_k^{\dagger}$
- Son unitarias, es decir, para todas ellas su producto por su adjunta es la matriz identidad:  $\sigma_k \sigma_k^{\dagger} = I$.

De estas dos propiedades, se deriva que el producto de cada una de ellas por sí misma es a su vez la matriz identidad:

$X^2 = Y^2 = Z^2 = I$


**(ii) $H = \frac{1}{\sqrt{2}}(X + Z)$**
$\frac{1}{\sqrt{2}}(X + Z) = \frac{1}{\sqrt{2}}\left[\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} + \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}\right] = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} = H$


**(iii) $X = HZH$**

$HZH = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$ 

$= \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix} \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} = \frac{1}{2}\begin{pmatrix} 0 & 2 \\ 2 & 0 \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = X$ 


**(iv) $Z = HXH$**

$HXH = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$

$= \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ -1 & 1 \end{pmatrix} \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} = \frac{1}{2}\begin{pmatrix} 2 & 0 \\ 0 & -2 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = Z$ 


**(v) $-1Y = HYH$**

$HYH = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$

$=\frac{1}{\sqrt{2}} \begin{pmatrix} i & -i \\ -i & -i \end{pmatrix}\frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}= \frac{1}{2} \begin{pmatrix} 0 & 2i \\ -2i & 0 \end{pmatrix} = \begin{pmatrix} 0 & i \\ -i & 0 \end{pmatrix} = -1Y$


**(vi) $S = T^2$**

$T^2 = \begin{pmatrix} 1 & 0 \\ 0 & e^{i\pi/4} \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & e^{i\pi/4} \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix} = S$


**(vii) $-1Y = XYX$**
$XYX =\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}\begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}= \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}= \begin{pmatrix}0 & i \\ -i & 0 \end{pmatrix} = -1 Y$

<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Boletín de ejercicios 2

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
