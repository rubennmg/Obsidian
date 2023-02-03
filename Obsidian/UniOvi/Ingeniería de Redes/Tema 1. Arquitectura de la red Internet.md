## Gestión de Internet
ISP - Proveedor de Servicios de Internet
IANA - ISP

## Evolución de Internet
ARPANET - Debía de ser una red redundante

## Sistemas autónomos
Actualmente no quedan rangos IPv4 libres

## Protocolos TCP/IP
![[Pasted image 20230130124020.png]]
###### Capa MAC
Ethernet - IEEE 802.3
Capa MAC - CSMA/CD - Acceso múltiple por detección de portadora con detección de colisiones
CSMA (Carrier Sense Multiple Access) /CD(Collision Detection)
Full-Duplex -> Los equipos pueden escuchar y transmitir a la vez (Tx + Rx)
backoff - tiempo de espera

En IEEE 802.11 se usa CSMA/CA

###### Capa LLC
Control de flujo y control de errores


![[Pasted image 20230202111338.png]]

	          14 bytes                                                Control de errores (4 bytes)

## Capa red/IP (Internet)
Protocolo no orientado a conexión. Sus objetivos son el direccionamiento IP y el encaminamiento.


## NAT/PAT
IPv4 -> 32 bits (2³² direcciones) +- 4000 millones IPs



Clase A -> /8
Clase B-> /16
Clase C -> /24

CIDR -> redes classless