# Bitácora - Seguridad de Datos

## Índice 

 - Primer Parcial
    - Tarea 997
    - Tarea 995
    - Tarea 994
    - Tarea 993
    - Tarea 992
    - Tarea 989
    - Tarea 985
    
## 

## Tarea 997 - GitHub Education

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/Images/GitHubEdu.png)

##

## Tarea 995 - Conceptos Básicos de Seguridad

|**CIA Triad**|
|:-----------:|

Se trata del acronimo de *Confidencialidad*, *Integridad* y *Disponibilidad*, siendo estos 3 los pilares de la seguridad de la información.

Cada punto tiene diferente importancia dentro de esta triada. De esta forma, podemos definir cada punto como:
 
 - **Confidencialidad**:
   Que no se revele información a quien no esta autorizado. Se busca garantizar que la información sea accedidad solamente    por las personas a quien se les otorga el permiso.
   
 - **Integridad**:
   Que los datos no sean alterados. Consiste en que la información no sea modificada en cualquiera de sus 3 estados (*almacenamiento*, *proceso* o *transito*).
   
 - **Disponibilidad**:
   Que la información siempre esté accesible para las personas autorizadas. Se busca que la información tenga un acceso 
   activo en todo momento según sea necesario.

|**Usability Triangle**|
|:--------------------:|

El triángulo FSU, un acrónimo de Funcionalidad-Seguridad-Usabilidad, tres cosas fundamentales a la hora de desarrollar productos de software.

Dependiendo de a quién o qué desarrollaremos, uno de estos tres aspectos podría explotarse más que otro, el punto negro que está en medio del triángulo define que tan seguro, funcional y usable es nuestro producto. Dicho punto puede movilizarse a una esquina del triángulo según sea la necesidad, pero mientras más se acerca a una esquina evidentemente se aleja de las otras.

|**Riesgo**|
|:--------:|

El término riesgo de seguridad de la información se refiere al daño potencial causado por ataques a los sistemas de TI. El riesgo de TI incluye una amplia gama de eventos potenciales, como violaciones de datos, acciones de cumplimiento normativo, costos financieros, daños a la reputación y otros.

|**MFA**|
|:-----:|

La autenticación multifactor (MFA) es un proceso de registro en varios pasos que requiere que los usuarios ingresen algo más de información que simplemente una contraseña. Por ejemplo, junto con la contraseña, los usuarios deberán ingresar un código que se envía a su correo electrónico, responder a una pregunta secreta o escanear una huella dactilar. Una segunda forma de autenticación puede ayudar a evitar el acceso no autorizado a una cuenta si la contraseña del sistema se ha visto expuesta.

|**Vulnerabilidad**|
|:----------------:|

Una vulnerabilidad es una debilidad existente en un sistema que puede ser utilizada por una persona malintencionada para comprometer su seguridad. Las vulnerabilidades pueden ser de varios tipos, pueden ser de tipo hardware, software, procedimentales o humanas y pueden ser explotadas o utilizadas por intrusos o atacantes.

|**Amenaza**|
|:---------:|

Se refiere a la explotación de fallos que se utilizan para afectar la operatividad de un sistema, con la intención de sacar algún provecho.

Las amenazas informáticas pueden clasificarse, según su origen y a grandes rasgos, en dos categorías:

  - Amenazas informáticas externas
  - Amenazas informáticas internas

Las amenazas informáticas pueden tener un impacto significativo en las operaciones comerciales de una organización.

Pueden conducir a la pérdida de datos, al tiempo de inactividad de los sistemas críticos, a pérdidas financieras, etc.

|**Impacto**|
|:---------:|

Un impacto en la seguridad de la información es cuando existe una amenaza a la seguridad informática y esta logra atravesar las medidas de defensa, bien sea malware, virus, etc. cualquier tipo de ataque informático que pueda poner en peligro cualquier tipo de información, datos, etc.

Pueden ser de tipo:

   - Financiero
   - Operacional
   - Legal o regulatorio
   - Reputación
   - Estratégico

## 
## Tarea 994 - Instalar ParrotSec

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/Images/Parrot.jpg)

##
## Apuntes Martes 23/01/2024

|**Hack Value:**|
|:--------------|
Se trata del valor que tiene un objetivo para un hacker.
|**Target of Evaluation:**|
Es el equipo o sitio que requiere de intervención de expertos en seguridad con el fin de evitar o cubrir vulnerabilidades.
|**Exploit:**|
Hace referencia al ataque que se realiza a alguna vulnerabilidad dentro de un sitio.
|**Zero-Day Attack:**|
Son los ataques que se llevan en software que aun no se ha lanzado, por lo que los desarrolladores deben trabajar en eso incluso antes de lanzar el producto.
|**Vulnerability:**|
Es toda area de riesgo que tiene un equipo o sitio, ya sean brechas en la estructura o areas de aprovechamiento para los hackers.
|**Daisy Chaining:**|
Se refiere a la acción de encubrir los pasos que se llevaron a cabo luego de una infiltración dentro de un equipo o sitio, a fin de evitar que se descubra al responsable.
|**Authenticity (Autenticidad):**| 
Es la comprobación que se lleva a cabo a fin de verificar que quien esta accediendo es quien dice ser. 
|**Non Repudiation:**|
El no repudio garantiza que ninguna parte pueda negar que envió o recibió un mensaje mediante cifrado y/o firmas digitales o aprobó cierta información. Tampoco puede negar la autenticidad de su firma en un documento.

|**Attack** =|Goals + Motives + Objectives|
|:-----------|:---------------------------|   

**Tipos de Amenazas:**

* Naturales
* Seguridad Física
* Humanas (Especial enfasís en *Insiders* y *Social Engineering*)
* De Red 
* Host
* De Aplicación  

##

## Tarea 993 - AtTiny85 y PoC

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/Images/AtTiny85.jpeg)

```bash
    #include "DigiKeyboard.h"

    void setup() 
    {
        //empty
    }

    void loop() 
    {
        DigiKeyboard.sendKeyStroke(0);
        DigiKeyboard.delay(100);
        DigiKeyboard.sendKeyStroke(KEY_W, MOD_CONTROL_LEFT);
        DigiKeyboard.delay(100);
        DigiKeyboard.sendKeyStroke(KEY_F4, MOD_ALT_LEFT);
    }
```
##

## Tarea 992 - ESP32

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/Images/ESP32.jpeg)

##

## Tarea 989 - Instalar JuiceShop

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/Images/JuiceShop.png)

##

## Tarea 985 - SQL Injection

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/SQL%20Injection/SQL_Injection_1.png)

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/SQL%20Injection/SQL_Injection_2.png)

![App Screenshot](https://github.com/v-Chriz-v/Seguridad_Datos/blob/main/Bitacora/Primer%20parcial/SQL%20Injection/SQL_Injection_3.png)

Los dos Labs sin resolver necesitaban la versión PRO de Burp Suite 

##

## Apuntes 15/02/2024

|**Alta Disponibilidad:**|
|:-----------------------|
Es la capacidad que tiene un sistema de TI para ser accesible y confiable casi todo el tiempo, lo cual elimina o disminuye el tiempo de inactividad.
|**Active Directory:**|
Se trata del término que utiliza Microsoft para referirse a su implementación de servicio de directorio en una red distribuida de computadoras. Utiliza distintos protocolos, principalmente LDAP, DNS, ​ DHCP y Kerberos.
|**Open LDAP**|
**OpenLDAP** es una implementación gratuita y de recurso abierto del protocolo LDAP. 
**LDAP** (Lightweight Directory Access Protocol) es un protocolo estándar para usuarios, dispositivos y clientes de comunicación con un servidor de directorio. El protocolo LDAP facilita al usuario la autenticación y autorización para los recursos de las tecnologías de la información, los cuales pueden incluir servidores, aplicaciones, redes, servidores de archivo y más.
|**Entropía de contraseña**|
Predice cómo de difícil será descifrar una contraseña dada, a través de ataques de fuerza bruta, ataques de diccionario u otros métodos comunes.

Pentesting (Whitebox, Blackbox, Graybox), (Internas, Externas)
* Reconocimiento (Footprinting)
* Escaneo
* Ganar acceso
* Mantener el acceso
* Cubrir Huellas

##

## Apuntes 20/02/2024

**Puertos definidos:** 
* 80 http
* 22 ssh
* 21 ftp
* 23 telnet
* 25 smtp
* 53 dns 
* 3306 MySql
* 8080 Tomcat

Puertos máximos = **65536** (2^16)

|**Puertos efímeros:**|
|:--------------------|
Van desde el 49152 hasta el 65535 y son unos puertos temporales de usar y tirar que el sistema operativo asigna a las aplicaciones cuando los necesitan. Una vez que la conexión ha terminado ese puerto queda libre y puede ser reutilizado nuevamente por cualquier otra aplicación.

**¿Qué pasa cuando los puertos efímeros se agotan?** 
* Cuando esto sucede, los nuevos intentos de establecer conexiones pueden fallar o pueden encontrarse con demoras significativas, lo que puede llevar a un rendimiento deficiente de las aplicaciones o servicios que dependen de esas conexiones. Además, puede haber problemas de escalabilidad si hay una gran cantidad de solicitudes simultáneas que necesitan puertos efímeros.

**Nmap** hace un escaneo de puertos a toda una red.
**Netcat** hace el escaneo a un solo host.
##