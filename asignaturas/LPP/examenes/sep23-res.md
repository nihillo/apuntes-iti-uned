## 1
### 1.a
Un autómata a pila es un autómata que dispone de una memoria auxiliar, denominada pila, en la que se van almacenando símbolos según un procedimiento LIFO (Last-In-First-Out). A diferencia de los autómatas finitos, cada una de las transiciones que se efectúan con el autómata a pila depende del símbolo de entrada y del símbolo de pila. Un autómata a pila acepta una cadena si al procesarla, empezando con la pila vacía, y siguiendo las transiciones que tengan lugar, conduce a un estado final. 
Los autómatas finitos definen lenguajes y gramáticas regulares, mientras que los autómatas a pila definen lenguajes y gramáticas independientes del contexto, las cuales son un superconjunto de las regulares. Por lo general, en el procesamiento de un lenguaje, el análisis léxico atiende a lenguajes regulares, mientras el sintáctico pertenece al ámbito de los independientes del contexto no regulares, por lo que se harán necesarios autómatas a pila para procesarlos.

### 1.b


## 2
### 2.a
La fase del compilador encargada de la generación y optimización de código objeto consiste fundamentalmente en la traducción de cada una de las instrucciones de código intermedio a una serie de instrucciones de código máquina.
Si bien esto originalmente se hacía de forma muy ad hoc, lo que hacía el proceso dependiente del lenguaje que se estuviera compilando y de la máquina para la que se estuviera haciendo, a partir de los años 60 se han venido utilizando dos técnicas para este proceso:
- Traducción dirigida por la sintaxis, consistente en asignar a cada regla sintáctica una serie de reglas de traducción
- análisis sintáctico recursivo descendente, consistente en construir las reglas mediante el análisis del árbol sintáctico desde su raíz hacia abajo.
### 2.b


## 3
### 3.a
```Haskell
factorial :: Integer -> Integer
factorial 1 = 1
factorial n = n * factorial (n-1)
```

### 3.b
La evaluación perezosa o diferida es una estrategia por la cual no se evalúan las expresiones hasta que no es necesario.
Por ejemplo, si una expresión condicional depende de la evaluación de una determinada expresión que devuelve un booleano, esta expresión no se evaluará hasta el momento en que se tenga que decidir si se entra a ejecutar el código contenido en la rama condicional. 
Esta técnica se opone a la de evaluación ansiosa o estricta, por la cual todas las expresiones son evaluadas de antemano.
La evaluación perezosa es muy común entre los lenguajes del paradigma funcional, mientras la ansiosa lo es entre los del imperativo.



## 4
### 4.a 
```XML
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
	<xs:element name="tienda">
		<xs:complexType>
			<xs:sequence>
				<xs:element name="guitarra" type="GuitarraType" minOccurs="0" maxOccurs="unbounded" />
				<xs:element name="bateria" type="BateriaType" minOccurs="0" maxOccurs="unbounded" />
			</xs:sequence>
		</xs:complexType>
	</xs:element>

	<xs:complexType name="GuitarraType">
		<xs:sequence>
			<xs:element name="marca" type="xs:string" />
			<xs:element name="modelo" type="xs:string" />
			<xs:element name="tipo" type="xs:string" />
			<xs:element name="numeroCuerdas">
				<xs:restriction base="xs:int">
					<xs:minInclusive value="6" />
					<xs:maxInclusive value="7" />
				</xs:restriction>
			</xs:element>
		</xs:sequence>
	</xs:complexType>
			
	<xs:complexType name="BateriaType">
		<xs:sequence>
			<xs:element name="marca" type="xs:string" />
			<xs:element name="modelo" type="xs:string" />
			<xs:element name="tipo" type="xs:string" />
			<xs:element name="numeroTimbales" type="xs:string" />
		</xs:sequence>
	</xs:complexType>
</xs:schema>
```

### 4.b
```XPath
/artistas/artista[anonacimiento<1900]/nombre
```


## 5
### 5.a 
Perl se destaca por su capacidad para el manejo de expresiones regulares y su potencia para la manipulación de texto y el procesamiento de datos, lo que lo hace muy apropiado para el procesamiento de cadenas.
Hay tres tipos de variables en Perl:
- Escalares: sus identificadores comienzan por el símbolo $, y guardan valores simples como cadenas o valores numéricos.
- Arrays: sus identificadores comienzan por @ y guardan por posición listas de escalares, empezando por el índice 0. El acceso al valor guardado en una determinada posición se nota sin embargo como escalar, por ejemplo.
	- @colores = ('rojo', 'azul', 'verde')
	- $colores\[1] 
- Arrays asociativos: sus identificadores comienzan por % y guardan pares clave-valor. El acceso al valor asociado a una clave se nota como escalar, y la referencia a la clave que se quiere acceder si coloca entre llaves
	- %cantidades = ('rojo', 0, 'azul', 3, 'verde' 4)
	- $cantidades{'rojo'}

### 5.b
El principio de ocultación de información consiste en determinar qué partes de las abstracciones oculta una parte del código de otras y cuáles muestra. En general los lenguajes deberían ofrecer mecanismos de ocultación de la información ya que esto favorece la modularidad y la separación de responsabilidades, lo cual repercute en la calidad, mantenibilidad y escalabilidad del código.
En la programación orientada a objetos, la ocultación de información juega un papel fundamental, siendo uno de los principales principios por los que se rige. Se manifiesta en propiedades básicas como la visibilidad de los atributos y métodos de las clases, según la cual se puede determinar si son públicos (accesibles desde fuera de la clase) o privados (accesibles dentro). En un nivel mayor de abstracción, el propio polimorfismo es también una forma de ocultación de información, ya que un determinado cliente se puede comunicar con objetos de distintos tipos polimórficos sin necesidad de conocer de qué tipo exacto son, siempre y cuando compartan una misma interfaz.