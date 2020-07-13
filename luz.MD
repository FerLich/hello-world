# Práctica Luz

> Alumno: Gonzalo Nahuel Vaca

## 1. Identifique los mensajes de RPL. ¿cuántos tipos de mensajes puede diferenciar? Enumérelos.

* DODAG Information Object
* DODAG Information Solicitation
* Destination Advertisement Object
* Destination Advertisement Object Acknowledgment

## 2. ¿Cuál es la dirección de destino de los mensajes? ¿Qué clase de dirección es?

> fe80::201:1:1:1 *Es una dirección IPv6*

## 3. ¿Mediante qué protocolo de IPv6 se establece el DODAG?

> Mediante el protocolo **ICMPv6**

## 4. ¿Cómo lo identifica?

> Se identifica por el *Next Header: ICMPv6* y por el *Type: RPL Control*

## 5. ¿Qué valor tiene el DODAGID en los mensajes RPL? ¿Con qué lo relaciona?

> DODAGID: fd00::201:1:1:1

Se relaciona con el root del grafo.

## 6. Ubique los mensajes UDP del nodo 2 al nodo 1. ¿A qué puesto están dirigidos?

> Destination Port: 5678

## 7. ¿Qué tipo de dirección es?

> IPv6

## 8. En Wireshark identifique los primeros mensajes originados en el nodo 1 (se puede establecer un filtro haciendo click con el botón derecho sobre el campo que se va a usar como filtro y seleccionado “Apply as filter” – por ejemplo “ipv6.src == fe80::c30c:0:0:1”). ¿Qué tipo de mensaje es?

> Es un mensaje **RPL Control** del tipo *Destination Advertisement Object*

## 9. ¿Cuál es la dirección de destino?

> ::201:1:1:1

## 10. ¿Cómo identifica que es un mensaje RPL?

> Dentro del IMCPv6, dentro del campo *Type* figura 155 **RPL Control**