# Nmap
Esta herramienta hace un escaneo de todos los puertos disponibles dada una dirección IP.

Si utilizamos el comando nmap sin ninguna flag este solo analizara los 1000 puertos mas comunes.

![Pasted image 20250703182252](../Imagenes/Pasted%20image%2020250703182252.png)


El PORT es el numero de puerto escaneado y su categoría, como es predeterminada sin ninguna flag este va a escanear solo los TCP.

El STATE confirma que puertos están abiertos y a veces hay puertos que tiene un STATE de filtared que quiere decir, que el fireware solo permite el acceso al puerto desde direcciones especificas. 

El SERVICE indica el nombre del servicio que esta asignado a ese puerto, pero este no indica que se esta escuchando por ese puerto, así que hasta que no se haga un nmap que interactúe con el servicio e intente obtener información, podría tratarse de otro servicio.

**Comandos con flags**
	**Service Version Detection**
		Indica que servicio están corriendo dentro de los puertos y sus versiones exactas
			`-sV`
	**Script Scan**
		Ejecuta una coleccion de scripts predeterminados para saber informacion adicional.
			`-sC`
	**Port Selection**
	Escanea en todos los puertos
		`-p-`
	**Script Scan Especifico**
		Permite ejecutar un script especifico para auditar un puerto de nuestro host
			`nmap --script <script name> -p<port> <host>`
		
