## ¿Qué es un CPD?
#### Definición CPD
Es una sala o edificio especialmente acondicionado para albergar sistemas informáticos y de comunicaciones cuyo objetivo es proporcionar a dichos sistemas un entorno de funcionamiento controlado, seguro y fácilmente gestionable. 

Cableado de datos  (conectar equipos) - cableado de fuerza


## Disponibilidad de un CPD
#### Definición
Es el grado de funcionamiento continuado, sin interrupciones, de las infraestructuras del CDP, de modo que los sistemas informáticos ubicados en él puedan mantenerse operativos.

#### Cálculo
Habitualmente, la disponibilidad se calcula como el porcentaje de tiempo que el CDP se encuentra operativo referido a un año.

Disponibilidad = ((tiempo año - tiempo de parada) / tiempo año) * 100  

#### Calcular el tiempo de parada máximo por año con disponibilidad = 99,99
0,9999 = 8760 - x / 8760
8760 * 0,9999 = 8760 - x
x = 8760 - 8760 * 0,9999 = 0,876 h
0,876 * 60 = 52,56 minutos
0,56 * 60 = 33,6 seg = 33 seg

El tiempo de parada máximo por año es de 52 minutos y 33 segundos


## Infraestructuras de un CPD
#### Cerramiento
**Objetivo**
			Proporcionar un habitáculo para el CPD con un alto nivel de protección de los sistemas informáticos frente a riesgos físicos y acceso no autorizado

**Opciones constructivas**
- **Acondicionamineto de salas interiores**
- **Salas cofre**
		Es una estructura modular basada en paneles, estructuralmente independiente, que se puede levantar tanto en interiores como en exteriores
- **Contenedores**
		Embalaje transportable de tipos y dimensiones normalizadas (20 y 40 pies).
		Viene montado de fábrica
		Para que funcione se le debe conectar la red eléctrica y la red de conexión de datos
		Es necesario instalar un sistema de refrigeración (condensador)
		Rápido de instalar, móvil  y de bajo coste
			
#### Suelo técnico
**Objetivo**
		Proporcionar un espacio oculto, pero fácilmente accesible, bajo el habitáculo del CPD con el objetivo de distribiur cableado, tuberías o aire acondicionado.

**Diseño**
			Consiste en una estructura metálica con soportes de altura ajustable que proporcionan la base para un suelo de paneles o losetas desmontables. Las dimensiones estándar de estas losetas son 60x60 cm.

#### Infraestructura eléctrica
**Requisitos**
		Capacidad de gestión de un gran número de deispositvos
		Capacidad de gestión de potencias elevadas
		Fiabilidad
**Elementos de ifraestructura eléctrica**
		- **Interruptores automáticos (disyuntores)**
				Son dispositivos cortacircuitos, operados automáticamente, cuyo objetivo es proteger los circuitos eléctricos del CPD de cortocircuitos o sobrecargas. 
		- **PDU (Power Distribution Unit)**
				Es un dispositivo cuyo objetivo es la distribución de potencia eléctrica. Tiene una entrada de alta potencia que se distribuye entre múltiples salidas de potencia reducida. Las PDUs son, habitualmente, dispositivos monitorizables y gestionables.
		- **Cableado y bases de conexión**

- **PDU preconfigurada**
	**Objetivo**
		Distribuir energía a múltiples racks.
- **PDU de rack**
	**Objetivo**
		Distribuir energía a los dispositivos ubicados en un rack.

- **Sistema EPO**
	  **Objetivo**
		  Cortar completamente la energía eléctrica del CPD, incluida la energía de emergencia cuando se produce una situación de alarma
	  **Causas de disparo del sistema EPO**
		  1- Disparo de la alarma de activación del sistema de extinción de incendios
		  2- Disparo manual, provocado por un operario, ante una situación de riesgo para la vida de las personas






















		

