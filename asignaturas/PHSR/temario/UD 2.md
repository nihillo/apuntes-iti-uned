# 7. Métodos no criptográficos en la implantación de la política de seguridad
- Herramientas para puesta en marcha de la política de seguridad
- Otros elementos a tener en cuenta
## Herramientas para la puesta en marcha de la política de seguridad
## Otros elementos a tener en cuenta

# 8. Los cortafuegos y sus aplicaciones
## Ventajas, inconvenientes y tipos de cortafuegos
- Puntos fuertes
	- Punto esencial de la aplicación de la política de seguridad
	- Soportan técnicas avanzadas de autenticación
	- Centralizar alarmas y registros de tráfico
	- Menos configuración que un sistema de propósito general
	- Necesitan pocos usuarios definidos
	- Política general restrictiva
- Puntos débiles
	- Dejar de usar ciertos servicios
	- Sensación de seguridad falsa
	- Centralización de medidas en un sólo sistema
	- Cuello de botella para tráfico
- Tipos
	- Filtros de paquetes
	- Gateways de aplicaciones
	- Tipo stateful inspection
	- Híbridos
## Filtros de paquetes
- Cada filtro compuesto de una serie de reglas
- Campos de cabeceras que se usan como criterios de filtrado
	- IP origen y destino
	- Puerto origen y destino
	- Protocolo
	- Opciones de la cabecera TCP
- Puntos débiles
	- Difícil mantenimiento
	- Si se tiene que hacer una excepción puede ser que haya que cambiar toda la configuración
	- No permiten control a nivel de usuario o datos
	- No es fácil filtrar protocolos con más de una conexión activa simultáneamente
- Definición de reglas de filtrado
### Ejemplo: ACL de encaminadores Cisco
- Standard. Access Control Entry (ACE)
	- access-list N {permit|deny} dirección-IP-origen \[máscara]
	- interface nombre-interface
	- ip access-group N {in|out}
- Extended
	-  access-list N {permit|deny} protocolo dir.IP-fuente \[máscara-fuente] \[op puerto-fuente] dir.IP-destino \[máscara-destino] \[op puerto-destino]
- NOTA: el puerto se puede escribir numéricamente (p. ej. "eq 25") o con el nombre del servicio (p. ej. "eq smtp")

## Gateways de aplicación o servidores proxy
## Qué se puede mejorar
# 9. Tecnologías de última generación en cortafuegos
- Caso práctico: modelo IPTables
	- Procesado de paquetes en IPTables
	- Sintaxis de las reglas de IPTables
	- IPTables como puerta de enlace de la red
	- Redirección de tráfico entrante (DNAT)
	- Guardar y restaurar reglas de filtrado
	- Herramientas gráficas de configuración
- Caso de estudio: el modelo Cisco ASA
	- Qué son los niveles ASA
	- Otras características avanzadas del ASA
# 10. Herramientas de análisis de vulnerabilidades para la auditoría de seguridad en redes
## Introducción
- Definición
- Tipos
	- En tiempo real
		- Busqueda de vulnerabilidades en aplicaciones o sistemas en ejecución, contra listado de vulnerabilidades conocidas, mediante cierto motor de búsqueda
		- También engloba herramientas de auditoría de redes y escaneo de puertos
	- Analizadores estáticos de código
		- SSCA (Static Source Code Analyzer)
		- Analízan código, esté o no en ejecución
		- Diferentes tipos de algoritmos para realizar la búsqueda
		- Uso recomendable en ciclo de diseño y desarrollo
## Caso práctico: la herramienta Nmap
### Instalación y uso de Nmap

## Caso práctico: la herramienta Nessus
## Herramientas de análisis de vulnerabilidades en código fuente (SSCA)
- Uso
	- Examinar código heredado
		- OJO trampa examen: "en ejecución". NO analiza en ejecución.
	- Como herramienta rutinaria en el ciclo de desarrollo
		- Esquema ciclo
- Características generales de las herramientas SSCA
- Tipos de herramientas SSCA
	- Clasificaciones
		- Según lenguajes que entienden
		- Según clases de vulnerabilidades que analizan
		- Según longitud de código que pueden analizar
	- Tipos según propósito
		- De chequeo de estilos
		- De chequeo de propiedades
		- De tipo "bug finding"
		- De tipo "security review"
- Qué herramiienta seleccionar
# 11. Herramientas de detección de intrusiones en red para monitorización de seguridad en redes
- Caso práctico: Snort
- Caso práctico: Sguil
- Honeypots
	- Ejemplos de honeypots reales
# 12. Diseño seguro de redes. Conceptos de alta disponibilidad y sistemas redundantes
- Diseño de soluciones de alta disponibilidad
- Problemas de infraestructura y soluciones
- Problemas en el nivel 2 de OSI y soluciones
- Problemas en el nivel 3 de OSI y soluciones
- Consideraciones para el resto de los niveles OSI
- Consideraciones para el almacenamiento en red: SAN
- Consideraciones para los dispositivos de seguridad