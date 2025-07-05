# Puertos
Son puntos virtuales donde empiezan y terminan las conexiones de red y son administrados por el SO host y estos permiten a los ordenadores diferenciar entre distintos tipos de trafico.
Hay puestos que están estandarizados para todos aquellos dispositivos conectados a una red
	Puerto: 80 (HTTP trafico de sitios web)
	Puerto: 443 (HTTPS)

**Categorías de puestos:**
	1. Protocolo de Control de Transmisión (TCP)
		Esta orientado a la conexión entre un cliente y un servidor, donde el servidor tiene que estar en estado de escucha y el cliente enviando las solicitudes de conexión.
	2. Protocolo Datagramas de Usuario (UDP)
		Es un modelo de comunicación sin conexión donde no hay protocolos de enlace, lo se se traduce en que no se garantiza la entrega satisfactoria de los datos.

**Puertos Comunes**

| Puerto(#) | Categoria |   Protocolo   |
| :-------: | :-------: | :-----------: |
|   20/21   |    TPC    |      FTP      |
|    22     |    TPC    |      SSH      |
|    23     |    TPC    |    Telnet     |
|    25     |    TPC    |     SMTP      |
|    80     |    TPC    |     HTTP      |
|    161    |  TPC/UDP  |     SNMP      |
|    389    |  TPC/UDP  |     LDAP      |
|    443    |    TPC    | SSL/TLS(HTTP) |
|    445    |    TPC    |      SMB      |
|   3389    |    TPC    |      RDP      |


