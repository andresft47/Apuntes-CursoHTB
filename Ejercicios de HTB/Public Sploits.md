![[Pasted image 20250704181702.png]]
Exploramos en el navegador el servidor para saber que tipos de exploits podemos explotar, y nos damos cuenta que podemos buscar exploits relacionados con Simple Backup.

![[Pasted image 20250704181954.png]]
![[Pasted image 20250704181934.png]]

iniciamos metasploit
![[Pasted image 20250704181751.png]]

Hacemos un nmap del servicio y la versión que esta corriendo en ese puerto y verificamos que es servicio http en el puerto 32706, que es el del wordpress.
![[Pasted image 20250704181811.png]]

Buscamos dentro de metasploit cual esta relacionado con el Simple Backup, y encontramos un modulo que esta relacionado.
![[Pasted image 20250704181839.png]]

Lo usamos con el comando use 0 que es el índice del modulo, luego hacemos un `set FILEPATH /flag.txt` para  leer el archivo flag.txt del servidor remoto, y luego el set ip del servidor y del puerto donde esta escuchando.
Y lo corremos con run y este devuelve un archivo flag.txt que fue cargado en la maquina local.
![[Pasted image 20250704181903.png]]
