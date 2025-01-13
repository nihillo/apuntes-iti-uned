## Pautas
- Voraz
	- Optimizar función objetivo
	- Solución global formada por soluciones paso a paso
	- No es necesario reconsideración
- Divide y Vencerás
	- Descomponer problema en subproblemas hasta problema trivial
	- Será más eficiente si las particiones tienen tamaño parecido
- Programación Dinámica
	- Se resuelven problemas de tamaño creciente por etapas
	- Etapas intermedias son almacenadas en memoria
	- Cada etapa intermedia es el estado óptimo
- Vuelta Atrás
	- Recorrido en profundidad
	- Utilizado en árboles y grafos normalmente
	- Ventajas: simple/intuitivo
	- Desventajas: ineficiente
- Ramificación y Poda
	- Exhaustivo, como vuelta atrás
	- Ramificación: el recorrido no tiene que ser en profundidad
	- Poda: utilizamos cotas para detener el recorrido

## Problema -> esquema

| Problema                                       | Esquema (familia)     | Nombre algoritmo(s)    |
| ---------------------------------------------- | --------------------- | ---------------------- |
| Almacenamiento óptimo en un soporte secuencial | Voraz                 |                        |
| Árbol de recubrimiento mínimo                  | Voraz                 | Prim<br>Kruskal        |
| Asignación de cursos                           | Vuelta Atrás          |                        |
| Asistencia a incidencias                       | Voraz                 |                        |
| Camino de coste mínimo                         | Voraz                 | Dijkstra               |
| Camino de coste mínimo                         | Programación Dinámica | Floyd                  |
| Ciclos Hamiltonianos                           | Vuelta Atrás          |                        |
| Coeficientes binomiales                        | Programación Dinámica |                        |
| Coloreado de grafos                            | Vuelta Atrás          |                        |
| Cursos de formación                            | Ramificación y Poda   |                        |
| Devolución de cambio                           | Programación dinámica |                        |
| Distancia de edición                           | Programación Dinámica |                        |
| Distancia de edición                           | Ramificación y poda   |                        |
| Elemento mayoritario                           | Divide y Vencerás     |                        |
| Liga de equipos                                | Divide y Vencerás     |                        |
| Mantenimiento de conectividad                  | Voraz                 |                        |
| Mensajería urgente                             | Voraz                 |                        |
| Minimización de tiempo en el sistema           | Voraz                 |                        |
| Mochila (no fraccionable)                      | Programación Dinámica |                        |
| Mochila (fraccionable)                         | Voraz                 |                        |
| Multiplicación asociativa de matrices          | Programación Dinámica |                        |
| Ordenación                                     | Divide y Vencerás     | Mergesort<br>Quicksort |
| Pastelería                                     | Ramificación y Poda   |                        |
| Planificación con plazos                       | Voraz                 |                        |
| Reparto equitativo de activos                  | Vuelta Atrás          |                        |
| Robot desplazándose en un circuito             | Voraz                 |                        |
| Robot en busca del tornillo                    | Vuelta Atrás          |                        |
| Skyline de una ciudad                          | Divide y Vencerás     |                        |
| Subconjuntos de una suma dada                  | Vuelta Atrás          |                        |
| Trómino                                        | Divide y Vencerás     |                        |
| Viajante de comercio                           | Ramificación y Poda   |                        |
| Viaje por el río                               | Programación Dinámica |                        |
