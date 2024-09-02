# red p2p de compartición de archivos
## Clase St0263

## Estudiantes: Alberto Andres Diaz Mejia aadiazm@eafit.edu.co - Moises David Arrieta Hernandez  mdarrietah@eafit.edu.co

## Profesor: Edwin Nelson Montoya

## 1. Implementación de un sistema P2P donde cada nodo / proceso contiene uno o más microservicios que soportan un sistema de compartición de archivos distribuido y descentralizado.
## El proyecto implementa una red distribuida utilizando el algoritmo Chord, que se comunica a través de gRPC, permitiendo a los nodos gestionar y almacenar datos distribuidos de manera eficiente.

### 1.2 Loa aspectos que no se puedieron realizar fue el despliegue de los nodos como máquinas virtuales con docker en AWS Academy

## 2.0 Arquitectura y Diseño de Alto Nivel
#### Modelo Cliente-Servidor:
modelo cliente-servidor donde múltiples nodos actúan como servidores que pueden manejar solicitudes tanto de clientes como de otros nodos. 

###Sistema Distribuido:
El proyecto implementa una red Chord, que es un protocolo para sistemas de tabla hash distribuidos. Los nodos en la red cooperan para localizar y almacenar datos de manera eficiente a través de un espacio de claves particionado.

###Comunicación RPC (Remote Procedure Call):
Se utiliza gRPC, un marco de trabajo de alto rendimiento para realizar llamadas RPC, lo que permite que componentes separados de la red se comuniquen entre sí como si fueran llamadas locales.

###Tabla de Dedos (Finger Table):
Cada nodo mantiene una tabla que reduce significativamente el número de pasos necesarios para localizar un nodo responsable de una clave determinada. Esto mejora la eficiencia de las operaciones de búsqueda.

## 3.0 Descripcion de ambiente de desarrollo
### Lenguajes utilizados: python
### Bibliotecas y paquetes: gRPC y Protocol Buffers (Protobuf), Concurrencia y Multithreading, hashlib, typing.

## 4.0
### Chord Algorithm: El proyecto implementa el algoritmo Chord, que es un protocolo y algoritmo para un sistema de tabla hash distribuida que permite gestionar la ubicación y recuperación eficiente de datos en una red de nodos.
###Estructuras de Datos Específicas:
###Node y Finger: Clases que representan los nodos en la red Chord y las entradas en la tabla de dedos de un nodo, respectivamente.
Operaciones de Red Chord:
###Inserción y búsqueda de claves: Implementadas mediante métodos RPC que permiten insertar y buscar claves dentro de la red Chord, utilizando el enrutamiento definido por la tabla de dedos de cada nodo.

## Video: https://www.youtube.com/watch?v=eTC6m8vNSzo

## Referencias:
https://www.basware.com/en/solutions/procure-to-pay/procure-to-pay-process/
https://www.youtube.com/watch?v=iP28dHZIgBc
https://github.com/fivosts/Chord-DHT
https://github.com/MNoumanAbbasi/Chord-DHT-for-File-Sharing
https://github.com/melzareix/chord-dht
https://github.com/ChuanXia/Chord
