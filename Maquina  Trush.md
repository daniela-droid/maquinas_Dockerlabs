Es una debían 

Escaneamos con namp

sudo nmap -sV -sC -sS --open -p- -T4 IP_victima -oN scaneo.txt

Luego hacemos algo de fuzzing con Gobuster

fuzzin- ==técnica automatizada de pruebas de seguridad que consiste en inyectar una gran cantidad de datos de entrada inválidos, inesperados o aleatorios en un programa o sistema para descubrir vulnerabilidades como fallos, cierres inesperados o fugas de información==.

![[Pasted image 20251104210123.png]]

![[Pasted image 20251104211311.png]]
![[Pasted image 20251104211637.png]]

descubrimos la siguiente pass ssh
![[Pasted image 20251104211656.png]]
![[Pasted image 20251104212455.png]]

También podemos utilizar el siguiente comando para ver si podemos escalar privilegios.

sudo find / -perm 4000 2</dev/null





herramientas usadas
nmap- para escaneo de puertos y versiones de servicios.
gobuster- para descubrir directorios que no están a la vista.
hydra- para descubrir contraseñas mediante utilizando diccionarios o diccionarios propios.


