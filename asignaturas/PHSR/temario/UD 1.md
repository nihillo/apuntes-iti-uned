# 1. Descripción del problema de la seguridad en las comunicaciones y en la información
- Unas cuantas preguntas que ayudan a definir mejor el problema
- Soluciones "perfectas" y soluciones razonables
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
- Ataques man-in-the-middle
## Ataques basados en vulnerabilidades del software
## Ataques de denegación de servicio (DOS)
## Ataques por medio de código malicioso
## Ataques a dispositivos móviles
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