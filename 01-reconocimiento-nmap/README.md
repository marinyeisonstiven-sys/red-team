Objetivo**: Mapear servicios y puertos abiertos en Metasploitable2
IP Objetivo**: 192.168.233.128
Herramienta**: nmap
Comando usado**: `nmap -sV -sC 192.168.233.128`

Hallazgos**:
- Puerto 21 FTP: vsftpd 2.3.4 - Login anónimo permitido
- Puerto 22 SSH: OpenSSH 4.7p1 
- Puerto 23 Telnet: Linux telnetd
- 978 puertos filtrados

Impacto: 3 servicios críticos expuestos. FTP anónimo es vector de entrada.
Remediación: Deshabilitar FTP anónimo, cerrar telnet, usar solo SSH con llaves.

evidencia 
![captura nmap] (1784173922794.jpg) 
