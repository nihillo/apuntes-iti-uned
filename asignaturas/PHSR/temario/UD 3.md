# 13. Introducción a la criptografía aplicada en la informática
- Elementos básicos de cualquier sistema criptográfico
- Distintos niveles criptográficos en el software de redes y sistemas
- Tipos de ataques a sistemas criptográficos
# 14. Métodos criptográficos - Sistemas de clave privada, sistemas de clave pública y sistemas de una sóla vía (one-way hash)
- Algoritmos de clave privada o de criptografía simétrica
- Funciones de una sola vía
- Algoritmos de clave pública o de criptografía asimétrica
# 15. Certificación, autenticación e integridad de la información. Firma digital y PKI
## Autenticación, integridad y no repudio de la información
## Sistemas de firma digital
## El estándar X.509 y las autoridades de certificación
- Certificado digital
- Autoridad de certificación 
- Estándar X.509
- Campos de un certificado X.509
	- Versión
	- SN (número de serie)
		- Lista de revocación de certificados (CRL)
	- Identificador algoritmo
	- Parámetros
	- AC (autoridad certificadora)
	- Inicio validez
	- Fin validez
	- Usuario
	- Algoritmo
	- Parámetros
	- Clave pública del usuario
	- Firma digital de la AC
		- Cifrado del hash del resto del certificado con la clave privada de la AC
- Proceso de solicitud y generación de certificado
	1. Usuario genera clave pública y privada
	2. Genera petición de certificado y la envía a la AC
	3. La AC comprueba la identidad y envía el certificado del usuario y el suyo propio
	4. Usuario instala su propio certificado y el de la AC
- Proceso de comprobación de validez
	1. A envía su certificado a B
	2. B descifra la firma del certificado de A mediante la clave pública de la AC y comprueba que sea válida
	3. Si la firma es correcta, comprueba que el certificado no esté caducado ni revocado
	4. Si la firma es válida y el certificado no está caducado ni revocado, se acepta
- PKI (Public Key Infrastructure)
## Los modelos de infraestructura de clave pública o PKI
## Problemas de seguridad de las firmas digitales y de las PKI
# 16. Protocolos criptográficos - SSL, PGP, IPSec y otros
## Protocolos de comercio electrónico: SSL
## Protocolos de comercio electrónico: SET
## Los protocolos IPSec
###  Protocolo AH - Authentication Header
### Protocolo ESP - Encapsulating Security Payload
### Asociaciones de seguridad en IPSec
### Un ejemplo básico de uso de IPSec
### Protocolo PGP
# 17. Introducción a las Redes Privadas Virtuales
## Caracterización de las redes privadas virtuales
- Características
	- Integridad
	- Privacidad
	- Autenticación
	- Control de acceso
	- Auditoría y registro de actividades
	- Calidad del servicio
- Tipos
	- Extremo a extremo
	- Intermedias
	- Origen-intermedio
### Ventajas e inconvenientes de las VPN
- Ventajas
	- Reducción de costes
	- Mejora de la seguridad
	- Integración de los datos
	- Flexibilidad y escalabilidad
	- Simplificación de las operaciones
- Inconvenientes
	- Gastos puesta en marcha (equipos, infraestructura)
	- Riesgos de seguridad
	- Complejidad del sistema
	- Rendimiento
### Arquitectura y planificación de RPVs
- Componentes
	- Tunneling
	- Servicios de seguridad
- Elementos
	- Red no segura
	- Pasarelas de seguridad
	- Servidores de política de seguridad
	- Servidores de certificación
- PKI y autenticación
### Rendimiento, mantenimiento y seguridad
- Rendimiento. Factores:
	- Velocidad y fiabilidad
	- Fortaleza del procesado de cifrado
- Mantenimiento
	- Gestión de fallos de funcionamiento
	- Gestión de configuración
	- Gestión de auditoría y contabilidad del uso de recursos
	- Gestión de la seguridad
- Seguridad
## Configuración típica de una VPN que use IPSec
## VPN mediante SSL
## VPN a través de redes MPLS
- Redes MPLS: Multi Protocol Label Switching 
	- utilizan etiquetas de nivel 2 de OSI para tomar las decisiones de encaminamiento
	- orientadas a conexión
	- rutas preconfiguradas - LSP (Label Switching Paths)
- La VPN se basa no en un protocolo de cifrado sino en la estructura propiamente dicha de la red
- Tipos:
	- VPN nivel 3
		- Proveedor participa en el encaminamiento de nivel 3
	- VPN nivel 2
		- Proveedor interconecta sedes a través de tecnología de nivel 2 (capa de enlace): Ethernet, Frame Relay o ATM
		- Cliente mantiene control de encaminamiento de nivel 3
	- LAN Privadas Virtuales (VPLS)

# 18. Introducción a los protocolos criptográficos en redes inalámbricas
- Redes inalámbricas. Conceptos básicos
	- 802.11 a/b/g/n
	- Puntos de acceso
	- SSID, BSSID, dirección MAC
	- Paquetes baliza (Beacons)
	- Encriptación
- Teoría de ataques a redes inalámbricas
	- Problemas de autenticación, privacidad e integridad
	- Ataques. Fase de ereconocimiento
	- Tipos de ataques
	- Ataques a clientes de redes inalámbricas
- Medidas no criptográficas para protección de redes inalámbricas
	- Principios de diseño seguro para redes inalámbricas
	- malas defensas no criptográficas
	- Buenas defensas no criptográficas
- Medidas criptográficas para protección de redes inalámbricas
	- WEP (Wired Equivalent Privacy)
	- WPA (Wi-Fi Protected Access)
	- WPA2-Enterprise con certificados digitales