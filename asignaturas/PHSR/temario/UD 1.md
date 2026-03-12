# 1. Descripción del problema de la seguridad en las comunicaciones y en la información
## Unas cuantas preguntas que ayudan a definir mejor el problema
- Qué se quiere tener protegido
	- Inventario
	- Análisis de riesgos
- Contra quién se quiere proteger
	- Modelo de confianza
- Cómo se quiere proteger
	- tipos de ataques
	- tipos de defensas
- Cuánto dinero se puede emplear en implantar y mantener el proceso de seguridad
## Soluciones "perfectas" y soluciones razonables
- Aproximación militar
- Aproximación realista
- Política de seguridad
# 2. Seguridad en los elementos físicos existentes en una red
- Sistemas de cableado o inalámbricos
- Repetidores, hubs y conmutadores (switches)
- Encaminadores (routers)
- Servidores y otras máquinas
# 3. Seguridad en los elementos software existentes en una red
- Sistemas operativos y aplicaciones
- Protocolos y aplicaciones IP
- Mejoras de seguridad con IPv6
- Criterios de evaluación de seguridad
# 4. Métodos de ataque a equipos y redes
## Taxonomía de los tipos de ataques
- Origen
	- Externos
	- Internos
- Complejidad
	- No estructurados
	- Estructurados
- Formación, experiencia y capacidad del atacante
- Objetivos y técnicas
	- Obtención de información sobre los objetivos a atacar
	- Basados en mala administración de sistemas
	- Basados en vulnerabilidades de red
	- Basados en vulnerabilidades de software
	- Encaminados a sabotear un servicio
## Ataques orientados a la obtención de información sobre el objetivo
### Ingeniería social
- Phishing
### Herramientas informáticas
- ping
- nslookup
- port scanner
	- nmap
- analizadores de vulnerabilidades
	- Nessus
	- Metaexploit Framework
- finger
### Escuchadores o "sniffers" de paquetes
- Wireshark
### Análisis de metadatos
- Exiftool
## Ataques basados en la mala administración de sistemas
- Tipos
	- Robo de nombres de usuario y contraseñas
	- Acceso basado en relaciones de confianza
	- Aplicaciones de compartición de disco
	- Mala configuración de protocolos mal autenticados
	- Spoofing
- Cracker
	- diccionario
	- fuerza bruta
		- se necesita el fichero con los hashes de contraseñas de los usuarios
		- se prueba a generar los hashes de todas las contraseñas posibles y se prueban contra él, hasta que se encuentra la que se busca
	- Crackers
		- Brutus
		- John the Ripper
		- L0phtrack
- Relaciones de confianza
	- rlogin
	- rcp
	- rsh
- Zonas wi-fi abiertas
	- Rogue AP (tipo Man-in-the-Middle)
- Compartición de dierctorios
	- Servidores NFS (Network File System)
	- Entorno Windows de compartición de directorios
- Protocolos con mala administración de autenticación
	- SNMP
	- OSPF (Open Shortest Path First)
	- EIGRP (Enhanced IGRP)
- Spoofing 
	- IP spoofing
## Ataques basados en vulnerabilidades de protocolos de red
- Ataques a TFTP y SMTP, RIP, IGRP, ICMP
### Ataques man-in-the-middle
- DNS spoofing
- ARP spoofing
- Ataques a DHCP
	- Rogue DHCP
## Ataques basados en vulnerabilidades del software
- Efecto autoplay
- Uso de cookies
- Vulnerabilidades provocadas por mala implementación
- Buffer overflow
	- DOS
	- Ataques para obtener acceso a un sistema
- Worm Morris
- SQL injection
- Puertas falsas
- Bugs
- Ventana de vulnerabilidad
- Exploit
- Exploit de día 0
## Ataques de denegación de servicio (DOS)
- Clasificación
	- basados en peculiaridades de protocolos
	- basados en malas implementaciones de aplicaciones o protocolos
	- basados en SYN floods
	- distribuidos (DDOS)
- Ataques DOS basados en peculiaridades de protocolos
	- Poca importancia seguridad en diseño de protocolos
		- Ping floods
			- enviar muchos más mensajes ICMP de los que el destino puede gestionar normalmente
			- aplicaciones
				- fping - envía mensajes ICMP a la velocidad máxima que la tarjeta de red del equipo pueda controlar
		- smurf
	- Peculiaridades TCP
		- land
	- Peculiaridades IP
		- teardrop
- Ataques DOS basados en en malas implementaciones 
	- ping de la muerte
	- Out Of Band (OOB) data crash
- Ataques DOS basados en SYN floods
	- Mecanismo 3 step handshake
- Ataques DOS distribuidos (DDOS)
	- BotNets
## Ataques por medio de código malicioso
- Virus informáticos
- Troyano
- Tipos según dónde se alojan
	- Sector de arranque
	- Infectan archivos
	- De propagación automática desde el receptor (worms)
- Tipos según forma de actuar
	- Virus
	- Gusanos (worms)
	- Troyanos
	- Spyware
## Ataques a dispositivos móviles
- Motivaciones
- Técnicas
# 5. Defensas básicas ante ataques
- Controles de acceso físico a sistemas
- Controles de acceso lógico a sistemas
- Otros controles simples de acceso a la información
# 6. La política de seguridad como respuesta razonable a los problemas de seguridad en redes
- Qué es una política de seguridad
- Aspectos físicos de la política de seguridad
- Aspectos lógicos de la política de seguridad
- Aspectos legales de la política de seguridad
	- LOPD
	- LSSI
	- Esquema Nacional de Seguridad, ENS
- Aspectos organizativos de la política de seguridad
	- Estándar ISO/IEC 15408
	- Estándar ISO/IEC 27001
	- Buenas prácticas de ITIL e ISO/IEC 20000