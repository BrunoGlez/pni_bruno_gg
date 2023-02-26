# EJERCICIO DE ENCAMINAMIENTO ESTÁTICO I

1. Realiza en Packet Tracer el diagrama de red tal y como el que se adjunta. Debes poner las direcciones ip que se indican así como los carteles.

![](img/001.png)

2. Realiza un un ping entre el `PC0`y el `PC2`, pega el resultado en la caja de código:

```
C:\>ping 10.0.0.2

Pinging 10.0.0.2 with 32 bytes of data:

Reply from 10.0.0.2: bytes=32 time=2ms TTL=128
Reply from 10.0.0.2: bytes=32 time<1ms TTL=128
Reply from 10.0.0.2: bytes=32 time=4ms TTL=128
Reply from 10.0.0.2: bytes=32 time=3ms TTL=128

Ping statistics for 10.0.0.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 4ms, Average = 2ms

C:\>
``` 

3. Muestra las tablas `arp`de cada uno de los PC y de los routers:

+ PC0

```

```

+ PC2

```

```

+ Router R1

```
R1#show arp
Protocol  Address          Age (min)  Hardware Addr   Type   Interface
Internet  11.0.0.1                -   0040.0BE0.36B0  ARPA   FastEthernet1/0
Internet  192.168.1.1             -   00E0.F77C.6E8E  ARPA   FastEthernet0/0
```

+ Router R2

```
R2#show arp
Protocol  Address          Age (min)  Hardware Addr   Type   Interface
Internet  10.0.0.1                -   00D0.BA99.3ED2  ARPA   FastEthernet0/0
Internet  11.0.0.2                -   000C.85BD.E590  ARPA   FastEthernet1/0
```

4. Establece las rutas estáticas necesarias para que haya comunicación entre los dos equipos de las diferentes redes. Inserta una captura de ping desde cada máquina. Pega los comandos en las cajas de código y rellena las tablas adjuntas.

+ Router R1

```

```




+ Router R2

```

```

5. Realiza un un ping entre el `PC0`y el `PC2`, pega el resultado en la caja de código:

```
C:\>ping 10.0.0.2

Pinging 10.0.0.2 with 32 bytes of data:

Reply from 10.0.0.2: bytes=32 time=2ms TTL=128
Reply from 10.0.0.2: bytes=32 time<1ms TTL=128
Reply from 10.0.0.2: bytes=32 time=4ms TTL=128
Reply from 10.0.0.2: bytes=32 time=3ms TTL=128

Ping statistics for 10.0.0.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 4ms, Average = 2ms

C:\>
```


6. Muestra las tablas `arp` de cada uno de los PC y de los routers:

+ PC0

```

```

+ PC2

```

```

+ Router R1

```
R1#show arp
Protocol  Address          Age (min)  Hardware Addr   Type   Interface
Internet  11.0.0.1                -   0040.0BE0.36B0  ARPA   FastEthernet1/0
Internet  192.168.1.1             -   00E0.F77C.6E8E  ARPA   FastEthernet0/0
```

+ Router R2

```
R2#show arp
Protocol  Address          Age (min)  Hardware Addr   Type   Interface
Internet  10.0.0.1                -   00D0.BA99.3ED2  ARPA   FastEthernet0/0
Internet  11.0.0.2                -   000C.85BD.E590  ARPA   FastEthernet1/0
```