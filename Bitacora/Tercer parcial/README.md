# Bitácora - Seguridad de Datos

## Índice

 - Tercer Parcial
    - Tarea 983
    - Tarea 982
    - Tarea 981
    - Tarea 980
    
## 

## Tarea 983 - Hardening de CentOS7

Antes del Hardening:
![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/HardeningAntes.png)

Despues del Hardening:
![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/HardeningDespues.png)

##

## Tarea 982 - UTM



##

## Tarea 981 - PoC en MS2

IRC es un protocolo de chat en línea que utiliza el puerto 6667 para establecer conexiones con los servidores de IRC. Este sistema de conversación en línea utiliza canales para permitir la comunicación entre usuarios de todo el mundo.
Unreal IRCD es un demonio de chat de retransmisión de código abierto  originalmente basado en Dreamforge, método antiguo de charla, el cual permite conectar a un servidor de chat de retransmisión de internet. Una de sus vulnerabilidades que se implementó en esto fue la de la puerta trasera (estuvo asi durante 7 meses cualquiera que descargue el archivo era vulnerable) con el servicio de metasploitable. 
Esta versión contiene una puerta trasera que pasó desapercibida durante meses : se activa al enviar las letras "AB" seguidas de un comando del sistema al servidor en cualquier puerto de escucha. Metasploit tiene un módulo para explotar esto y obtener un shell interactivo, como se muestra a continuación.

* Realizar escaneo de vulnerabilidades con nmap 
* Luego, buscar herramientas para explotar esta vulnerabilidad
* Poner la dirección ip 
* Clonar el repositorio
* Descargar nuestro exploit.py 
* Otorgar permisos de ejecución con el comando chmod
* Editar el exploit con el comando sudo nano explot.py, aquí se asigna hacia donde escucha ip y port  
* Accesos remoto se gana escuchando la conexión reversa y para esto nos ayuda la herramienta netcat 
* exploit.py dirección_ip_objetivo puerto -payload netcat (el guión en el payload nos sirve para obtener otra máquina virtual )
* sudo nc -nlvp puerto 443

En nuestro caso, hacemos un acceso no autenticado al sistema mediante este puerto. La siguiente línea de código nos sirve para redireccionar el acceso a nuestra red mediante un puerto establecido:

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/configip.png)

El script también usa un payload que otorga una conexión mediante netcat que devuelve una consola shell bash en la máquina objetivo.

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/payloadsestablecidos.png)

Mediante el siguiente código se envían las letras “AB”, lo cual activa una puerta trasera en Metasploitable

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/cadenaAB.png)

Si la conexión es exitosa, obtenemos el acceso al sistema de manera remota

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/conexionrecibida.png)

Al ejecutar el script con las ip y puertos ya establecidos, obtenemos el acceso al sistema. La prueba a continuación muestra como en la conexión remota (izquierda) se listan los directorios existentes en el sistema de Metasploitable (derecha).

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/entrandoalavm.png)

Para probar los permisos, creamos un directorio llamado “entramos” desde la conexión remota y, posteriormente, listamos los directorios en Metasploitable y logramos observar como el directorio se creó exitosamente.

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/exploitfuncionando.png)

Codigo obtenido de: https://github.com/Ranger11Danger/UnrealIRCd-3.2.8.1-Backdoor/blob/master/exploit.py


##

## Tarea 980 - Hardening en Benchmark - CentOS 8

Las siguientes capturas muestran los porcentajes de seguridad de CentOS 8 luego de aplicarle un hardening.

Antes del Hardening:
![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/CentOS8.png)

Aplicamos el [script para fortalecer el sistema (Hardening)](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/CentOS8.sh)

Despues del Hardening:
![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Tercer%20parcial/Images/CentOS8-hardening.png)

##