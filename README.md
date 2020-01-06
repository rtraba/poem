# PoEM
Proof of Existence Manager

This repository is a wraper for OpenTimestamps. https://github.com/opentimestamps/javascript-opentimestamps
The idea is basically to provide a service that generates proofs and persists .ots files in a KV database.
PoEM should also automatically check for upodates in .ots in pending-attesteation state.

![](https://github.com/rtraba/poem/blob/master/blpockcerts_architecture-Page-7.png)



# PoEM (Proof of Existence Manager)
A API se diseñ+o como un wraper de OpenTimestamps (https://github.com/opentimestamps/javascript-opentimestamps). La idea es poder proveer un servicio que genera pruebas de existencia y en lugar de delegar el tratamiento de los archivos .ots en el consumidor del servicio, almacena las pruevas en una base de datos persistente. A demás el wraper es responsable de mantener actualizados los archivos .ots según los calendar servers vayan pudiendo impactar las pruebas en la blockchain de Bitcoin.

Se tienen 5 contenedores que representan la arquitectura desplegable con docker-compose para facilitar el proceso.
A continuación vemos un breve diagrama que muestra el esquema de dependencias entre los contendores que hacen al funcionamiento de la API:

![](https://github.com/rtraba/poem/blob/master/blpockcerts_architecture-Page-7.png)
