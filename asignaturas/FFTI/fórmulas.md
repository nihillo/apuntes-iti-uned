
## Campo eléctrico

### Ley de Coulomb

Escalar (módulo): 
$F = k\frac{Q_1 Q_2}{d^2}$ 

Vectorial: 
$\vec{F} = k\frac{Q_A Q_B}{d^2} \hat{u}_{Q_A-Q_B}$ 


### Campo eléctrico debido a una carga puntual

$\vec{E_P} = k Q_i \frac{\vec{r_P} - \vec{r_i}}{|\vec{r_P} - \vec{r_I}|^3}$ 

$E = \frac{kQ_i}{r^2}$


### Flujo eléctrico

$\phi = \vec{E} \circ \vec{A} = EA \cos{\theta}$


## Conducción y resistencia

### Ley de Ohm

$R = \frac{V}{I}$ 

### Resistencia de un conductor

$R = \rho \frac{l}{A} = \frac{1}{\sigma} \frac{l}{A}$

### Resistividad respecto a la temperatura

$\rho = \rho_0[1 + \alpha(t - t_0)]$

donde $\rho_0$ es la resistividad a la temperatura de referencia $t_0$ (para la que, salvo otra indicación, tomaremos 20ºC) y $\alpha$ es el coeficiente de temperatura, propio del material 

### Potencia - Ley de Joule

$P = V\cdot I$ 

### Energía eléctrica

$W = P \cdot \Delta t$


----
## Potencial eléctrico

### Potencial debido a una carga
$V = \frac{kq}{r}$

### Potencial de un sistema de cargas puntuales
$V = \sum_{i=1}^{n} \frac{kq_i}{r_i}$

### Potencial de una superficie esférica uniformemenete cargada

$V = k\frac{kQ}{r}; ~ r > R$ 

$V = \frac{kQ}{R}; ~ r \leq R$

r: distancia desde el centro de la esfera hasta el punto en que se calcula el potencial
R: radio de la esfera

### Trabajo para mover una carga entre dos puntos
$W = q\Delta V$ 

----
## Capacidad y condensadores

### Capacidad
$C = \frac{Q}{V}$

### Condensador de placas paralelas

$E = \frac{\sigma}{\epsilon_0} = \frac{Q}{\epsilon_0 A}$ 

$C = \frac{Q}{V} = \frac{\epsilon_0 A}{d}$

$V = Ed = \frac{Qd}{\epsilon_0 A}$


### Energía acumulada en un condensador

$W = \frac{1}{2}\frac{Q^2}{C} = \frac{1}{2}QV = \frac{1}{2}CV^2$ 


### Condensadores en serie

$\frac{1}{C_s} = \sum_i{\frac{1}{C_i}}$ 

$Q$ es igual en todos los condensadores, $= Q_i$ 
$V_s$ es la suma de las $V_i$ de los condensadores


### Condensadores en paralelo

$C_p = \sum_i{C_i}$ 

$Q_p$ es la suma de las $Q_i$ de los condensadores
$V$ es igual en todos los condensadores, $= V_i$ 

### Condensadores con dieléctrico

$C = \kappa C_0$ 
$E = \frac{E_0}{\kappa}$ 

$\kappa$: constante dieléctrica
$\{X\}_0$: magnitud para condensador de iguales características 

----
## Campo magnético

### Fuerza sobre una carga

$\vec{F} = q \vec{v} \times \vec{B}$


### Campo magnético generado por un solenoide

$B = \mu_0 \frac{NI}{l}$

### Autoinductancia

$LI = N\phi_m$ 

### Flujo magnético 

$\phi_m = BA$ 


### Ecuaciones de Maxwell y Ley de Lorentz

#### Ley de Gauss
$\oint_S \vec{E} \circ d\vec{A} = \frac{Q}{\epsilon_0}$ 

#### Ley de Gauss del magnetismo
$\oint_S \vec{B} \circ d\vec{A} = 0$ 

#### Ley de Faraday
$\oint \vec{E} \circ d\vec{l} = - \frac{d\phi_m}{dt}$ 

#### Ley de Ampère generalizada
$\oint \vec{B} \circ d\vec{l} = \mu_0\epsilon_0 \frac{d\phi_e}{dt}$ 

#### Ley de Lorentz
$\vec{F} = q\vec{E} + q\vec{v} \times \vec{B}$ 

### Fuerza entre dos conductores rectilíneos
$\frac{F}{l} = \frac{\mu_0}{4 \pi} \frac{2 I_1 I_2}{a}$ 

de atracción si las corrientes van en el mismo sentido, de repulsión si van en sentido contrario

### Momento magnético

$\vec{\mu} = NIA \hat{n}$ 

----
## Régimen transitorio

### Circuitos R-C sin fuentes
$U(t) = U_0 \cdot e^{-t/\tau}$ 
$\tau = R \cdot C$ 

----
## Corriente alterna

### Factor de potencia
$f.d.p. = \frac{P}{S} = \frac{R}{Z} = \cos\phi$
donde $\phi$ es el desfase ente $U$ e $I$, es decir $\phi_U - \phi_I$ 


### Impedancia
- Resistencia : $\vec{Z}_R = R = R \lfloor 0º$
- Bobina: $\vec{Z}_L = j\omega L = \omega L \lfloor 90º$
- Condensador: $\vec{Z}_C = j \frac{-1}{\omega C} = \frac{1}{\omega C} \lfloor -90º$

#### R-L paralelo
$\vec{Z} = \frac{\omega R L}{\sqrt{R^2+\omega^2L^2}} \lfloor \arctan(R/\omega L)$  

#### R-C paralelo
$\vec{Z} = \frac{R}{\sqrt{1 + \omega^2 (RC)^2}} \lfloor \arctan(\omega R C)$  

----
## Transmisión de la información

### Ley de Snell

$\frac{\sin\theta_i}{\sin\theta_R} = \frac{n_2}{n_1}$



