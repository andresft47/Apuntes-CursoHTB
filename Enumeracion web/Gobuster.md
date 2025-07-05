# Gobuster
Permite realizar ataques de fuerza bruta para descubrir directorios y archivos ocultos en servidores web.

**Comando**

![Pasted image 20250704094757](../Imagenes/Pasted%20image%2020250704094757.png)

**Interpretación de códigos de estado HTTP:**
	`200`: Éxito (el archivo/directorio existe)  
	`301`: Redirección (posible contenido válido)  
	`403`: Acceso denegado (el archivo existe, pero está protegido)  
	`404`: No encontrado (no aparece en la salida de Gobuster)

**Detección de WordPress**

![Pasted image 20250704094938](../Imagenes/Pasted%20image%2020250704094938.png)

- Se identificó `/wordpress` redirigido (301), lo cual indica la instalación del CMS más popular.

- Acceder directamente en el navegador (`http://<IP>/wordpress`) mostró el asistente de instalación → Posible **RCE** (ejecución remota de código).

**Modo DNS**  
El modo `dns` intenta descubrir **subdominios ocultos o no documentados** de un dominio principal usando una **wordlist**. Por ejemplo, a partir de `inlanefreight.com`, puede encontrar:  
	`blog.inlanefreight.com`  
	`admin.inlanefreight.com`  
	`dev.inlanefreight.com`

![Pasted image 20250704095326](../Imagenes/Pasted%20image%2020250704095326.png)


