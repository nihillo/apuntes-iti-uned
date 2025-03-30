
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

$\bra{\psi} = \ket{\psi}^{\dagger}$
<div style="page-break-after: always; visibility: hidden">
\pagebreak
</div>

### Boletín de ejercicios 2
lorem ipsum dolor sit amet