Si no puedes usar red para transferir archivos (por firewall u otras restricciones),se puede **convertir el archivo en texto codificado en base64**:
	`base64 archivo -w 0`
Luego se pega esa cadena en la máquina remota y la decodificas:
	`echo <cadena_base64> | base64 -d > archivo`


Verificar que el archivo se transfirió bien
		`file archivo`
	Para ver qué tipo de archivo es.

También se puede comparar el **hash MD5** en ambas máquinas:
	`md5sum archivo`
Si el hash es igual, significa que el archivo no se corrompió.