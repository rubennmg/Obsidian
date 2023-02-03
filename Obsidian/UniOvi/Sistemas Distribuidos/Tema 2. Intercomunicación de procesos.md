## Sockets
Conexión - TCP
Sin conexión - datagramas (UDP)


atomicidad de los mensajes -> si se envían 1000 mensajes en un send, no se tienen por qué recibir todos en un recv (de una vez). Se recibirán todos pero en varias alturas


##### Funciones de la API para TCP
![[Pasted image 20230202095515.png]]
##### Servidor
1. **socket**
2. **bind** (0.0.0.0, 8082)-> asignar explícitamente IP + Puerto al socket
			IP-> una de las IP de la máquina
			0.0.0.0 - significa cualquier interfaz de la máquina
3. **listen**(7) -> transforma el socket a tipo escucha y crea la cola de tamaño n
4. **accept**(s) -> indica sobre qué socket se hace accept. _Es bloqueante_
5. **recv**(SD) -> puede ser bloqueante              SD - socket datos creado en el servidor
6. **send** -> es hipotéticamente bloqueante (puede serlo, pero no lo vamos a considerar)
7. **close**(SD)


##### Cliente
1. **socket**
2. **connect**(IPServidor, 8082) -> es bloqueante hasta que se establezca la conexión
3. **send** -> es hipotéticamente bloqueante (puede serlo, pero no lo vamos a considerar)
4. **recv** -> puede ser bloqueante
5. **close** 

