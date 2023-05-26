## Millman
- En el numerador, sólo las ramas que tengan fuente
- En el denominador, todas las ramas

$U_{xy} = \frac{\frac{U_1}{R_1}+ ... +\frac{U_N}{R_N}}{\frac{1}{R_1}+ ... +\frac{1}{R_N} + ... + \frac{1}{R_M}}$



## Thevenin
1. Calcular $U_{eq}$, como la tensión a circuito abierto entre los dos nudos para los que se está haciendo el Thevenin
2. Calcular $R_{eq}$, como resultado de eliminar la fuente del circuito y añadir una $U_x$ entre los puntos para los que se está haciendo el Thevenin. Hecho esto establecemos las igualdades convenientes según la ley de Ohm y despejamos la $R_{eq}$.

## Transistores

### Transistor bipolar
1. V en la base
2. Sustituir transistor por modelo 
	1. fuente 0,7V en BE, sentido según tipo (NPN o PNP)
3. I en base y colector
	1. I en CE: $I_C = \beta \cdot I_B$
4. V entre colector y emisor
5. Determinación zona de trabajo
	1. $U_B$ < 0.7 -> corte
	2. else: conduce
			1. NPN: $U_{CE} \leq 0$ / PNP: $U_{CE} \geq 0$ -> saturación 
		1. else: activa
6. I en el emisor

### Transistor MOSFET
1. Tensión en la puerta ($U_{GS}$)
2. Comparar con tensión umbral ($U_{th}$)
	1. Si $U_{GS} < U_{th}$ -> corte
	2. Else: conduce
		1. Calcular tensión drenador surtidor ($U_{DS}$)
			1. Si $U_{DS} > U_{CON}$ -> saturación o intensidad constante
				1. Modelo: Fuente de intensidad; $I_{D} = g \cdot (U_{GS} - U_{th})^2$
			2. Si $U_{DS} < U_{CON}$ -> zona ohmica
				1. Modelo:  Resistencia con valor $R_{DS} = \frac{U_{CON}}{I_D}$ 

### Tipos MOSFET

Acumulación: línea discontinua
Deplexión: línea continua

Canal N:  flecha hacia dentro (No pincha)
Canal P: flecha hacia afuera (Pincha)

### Determinación familias lógicas CMOS
- N:
	- Conduce si G = 1
	- No conduce si G = 0
- P:
	- Conduce si G = 0
	- No conduce si G = 1

1. Hacer tabla de verdad y evaluar salida para cada combinación de entradas
2. En base a la tabla de verdad, determinar la función lógica

## Bobinas acopladas

1. Determinar signo de $L$. En el lado de la $U$ que se quiere calcular, ver sentido de la $I$.
	1. Si mismo sentido $I$ y $U$, un incremento en $I$ producirá un incremento en $\phi$ en el sentido contrario, el cual producirá un incremento en $U$ en su sentido. -> es decir, **a igual sentido de $I$ y $U$, $L$ positivo, a distinto sentido, $L$ negativo**.
2. Determinar signo de $M$. Si la $I$ hace lo mismo (entra o sale) en la otra bobina respecto al terminal correspondiente, $M$ llevará el mismo signo que $L$, si no, el opuesto.

Forma de la ecuación:   $U_i = \pm L_i \frac{dI_i}{dt} \pm M \frac{dI_j}{dt}$ 


