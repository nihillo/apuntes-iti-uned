1. Preliminares
	1. Introducción
	2. Conceptos básicos
		1. Criptografía
		2. Criptosistema
		3. Esteganografía
		4. Criptoanálisis
		5. Compromiso entre criptosistema y criptoanálisis
		6. Seguridad en sistemas informáticos
2. Fundamentos teóricos de la criptografía
	1. Teoría de la información
		1. Cantidad de información
		2. Entropía
		3. Entropía condicionada
		4. Cantidad de información entre dos variables
		5. Criptosistema seguro de Shannon
		6. Redundancia
		7. Desinformación y distancia de unicidad
		8. Confusión y difusión
	2. Complejidad algorítmica
		1. Concepto de algoritmo
		2. Complejidad algorítmica
		3. Algoritmos polinomiales, exponenciales y subexponenciales
		4. Clases de complejidad
		5. Algoritmos probabilísticos
	3. Aritmética modular
		1. Concepto de aritmética modular
		2. Cálculo de inversas en Zn
		3. Teorema chino del resto
		4. Importancia de los números primos
		5. Algoritmos de factorización
		6. Tests de primalidad
		7. Anillos de polinomios
	4. Curvas elípticas en Criptografía
		1. Curvas elípticas en R
		2. Curvas elípticas en GF(n)
		3. Curvas elípticas en GF(2n)
		4. El problema de los logaritmos discretos en curvas elípticas
		5. Curvas elíptics usadas en criptografía
	5. Aritmética entera de múltiple precisión
		1. Representación de enteros largos
		2. Operaciones aritméticas sobre enteros largos
		3. Aritmética modular con enteros largos
	6. Criptografía y números aleatorios
		1. Tipos de secuencias aleatorias
		2. Utilidad de las secuencias aleatorias en criptografía
		3. Generación de secuencias aleatorias criptográficamente válidas
3. Algoritmos criptográficos
	1. Criptografía clásica
		1. Algoritmos clásicos de cifrado
		2. Máquina de rotores. La máquina ENIGMA
		3. El cifrado de Lorenz
	2. Cifrados por bloques
		1. Introducción
		2. DES
		3. Variantes de DES
		4. IDEA
		5. El algoritmo de Rijndael (AES)
		6. Modos de operación para algoritmos de cifrado por bloques
		7. Criptoanálisis de algoritmos de cifrado por bloques
	3. Cifrados de flujo
		1. Secuencias pseudoaleatorias
		2. Tipos de generadores de secuencia
		3. Registros de desplazamiento retroalimentados
		4. Generadores de secuencia basados en cifrados por bloques
		5. Algoritmos de generación de secuencia
	4. Cifrados asimétricos
		1. Aplicaciones de los algoritmos asimétricos
		2. Ataques de intermediario
		3. Algoritmo RSA
		4. Algoritmo de Diffie-Hellman
		5. Otros algoritmos asimétricos
		6. Criptografía de curva elíptica
	5. Funciones resumen
		1. Propiedades
		2. Longitud adecuada para una signatura
		3. Funciones MDC
		4. Seguridad de las funciones MDC
		5. Funciones MAC
		6. Cifrados autentificados
		7. Funciones KDF
	6. Esteganografía
		1. Mëtodos esteganográficos
		2. Detección de mensajes esteganografiados
	7. Pruebas de conocimiento cero
		1. Introducción
		2. Elementos
		3. Desarrollo
		4. Modos de operación
		5. Conocimiento cero sobre grafos
		6. Ataques de intermediario
4. Aplicaciones criptográficas
	1. Protocolos de comunicación segura
		1. Introducción
		2. Protocolos TCP/IP
		3. Protocolos SSL
		4. Protocolos TLS
		5. Protocolos IPsec
	2. Autentificación, certificados y firmas digitales
		1. Introducción
		2. Firmas digitales
		3. Certificados digitales
		4. Verificación de certificados digitales
		5. Autentificación mediante funciones resumen
	3. PGP
		1. Fundamentos e historia de PGP
		2. Estructura de PGP
		3. Vulnerabilidades de PGP