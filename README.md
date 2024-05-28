![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/4851080f-665a-4567-ba1f-9ea6cc44b0de) 
![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/bb77ee06-6bd4-4008-bfd7-e6c3f6f95374)


# Wazuh-maestria-grupo3
Dimensionamiento de maquina virtual, pasos a seguir para la instalación y 

Descripción General:

Para instalar el servicio Wazuh, lo primero que necesitamos es un sistema operativo compatible. En este caso, utilizaremos Ubuntu Server. 

A continuación, se detallan los pasos para la instalación y configuración de Wazuh.

Descarga del Sistema Operativo. Descargar Ubuntu Server desde la página oficial (ver Figura 1): https://ubuntu.com/download/server

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/850d740a-2102-43ac-b8e1-53ab5f2c1dd5)

Figura 1 Descarga del Sistema Operativo.
 
Una vez descargado el sistema operativo lo vamos a instalar en una máquina virtual.
Para nuestra practica utilizamos el VMware sobre el servidor.
Lo vamos a configurar con 4GB de RAM y almacenamiento de 60GB como se puede visualizar en la Figura 2.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/a52eaa04-d6c3-46c6-ab0d-1fb674423fbb)

Figura 2 Instalar y configurar en una máquina virtual
 
Se monta la imagen .ISO en la máquina virtual y vamos a instalar nuestro sistema operativo Ubuntu Server (ver Figura 3).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/c1392ae5-b8d1-4da3-8b81-e7482bc7473f)

Figura 3 Instalar Ubuntu server.
 
Nos pedirá elegir el idioma y seleccionamos Español de la Figura 4.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/8d954d4f-4463-4b38-816a-b70fb8d69a9f)

Figura 4 Seleccionar el idioma.
 
Nos pedirá elegir el idioma del teclado en este caso lo definimos como español (ver Figura 5).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/89b75d4f-f6d8-4b09-9706-1dccf09969d9)

Figura 5 Seleccionar el teclado.
 
Elegimos el tipo de instalación – Ubuntu Server de la Figura 6

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/42b72571-710e-4af4-a501-cfea5cee0f91)

Figura 6 Tipo e instalación.

 
Esperamos que detecte la configuración de red automática y presionamos siguiente como la figura 7.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/6c050cd0-acf3-4aaa-88c0-21ca6b036e36)

Figura 7 Detección de la configuración.
 

Nos pedirá la configuración de proxy, sino la tenemos solo damos ha Hecho para continuar (ver Figura 8).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/64e42b8e-3bf2-428f-8cd4-7b7a77679ceb)

Figura 8 No se configura el proxy.
 
El asistente de configuración en este punto buscara mirror de instalación disponibles más cercano a nuestra ubicación para la descarga de los componentes necesarios del sistema operativo Ubuntu Server. Le damos ha Hecho para continuar (ver Figura 9).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/5a7de8b1-dd71-477e-900b-b627b1604dfc)

Figura 9 Instalación disponible.

 
Nos pedirá configurar el almacenamiento del sistema operativo, para lo cual nos da la opción de permitir que el asistente lo configure automáticamente o lo customicemos.

Para nuestro ejemplo dejamos que el asistente lo haga automáticamente e incluso que configure LVM en el disco.

Luego presionamos Hecho como la Figura 10.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/fadef702-0247-4ba8-be3b-8e9284c2bd5d)

Figura 10 Configuración del almacenamiento.
 
Resumen de la configuración automática de sistema de archivos en la Figura 11.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/92f8eea3-16ed-4b23-9131-a8d1a6c51544)

Figura 11 Resumen configuración automática.
 
Nos pide confirmar el redimensionamiento y la distribución del disco, le damos click en continuar como se observa en la Figura 12.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/808d89ac-390c-4e1f-9048-70ef44e02f5a)

Figura 12 Confirmar acción destructiva.
 
Nos pedirá la configuración del perfil para lo cual colocamos los siguientes datos en la Figura 13.

Usuario: maestria

Clave: maestria

Le damos ha Hecho para continuar.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/67f400cb-ea9b-427d-ab48-8bcedd6a002b)

Figura 13 Configuración del perfil.
 
Nos pedirá realizar un Upgrade a Ubuntu Pro, le damos a skip for now y en Continuar (ver Figura 14).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/ae7319a9-bb7a-4237-a026-e9ecf37cf161)

Figura 14 Upgrade del Ubuntu.
 
Nos pedirá configuración de SSH pero en este caso no lo seleccionamos y solo le damos click ha Hecho para continuar (ver Figura 15).

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/2e7860ca-0ad8-4f99-be00-8ed61ee82b5c)

Figura 15 Configuración ssh.

Una vez terminada la configuración de instalación el sistema completa la descarga de los componentes e instala el sistema operativo, luego le damos click a Reiniciar ahora como se observa en la Figura 16.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/950ea8d8-d94d-4f63-a745-f20a857aecac)

Figura 16 Instalación completa.
 
Debemos actualizar en el primer inicio de sesión.

Utilizaremos los siguientes comandos en la Figura 17.

sudo apt get update

sudo apt get upgrade

Obtenemos el siguiente resultado.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/ad4e0744-a443-4580-93c0-bbe524fc4f6f)

Figura 17 Update y Upgrade
 
Acceso a la Interfaz Web de Wazuh y se observan las credenciales de acceso el la Figura 17:

URL: https://192.168.1.106

Usuario: admin

Clave: dHe4fvQo1S1SPFgX+d?7iDjUIrAgO170

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/e297de24-f04a-467c-8fc1-1792773b88f5)

Figura 17 Resumen de la Instalación completa.

Ingresamos a la página principal de wazuh para validar el acceso. En la figura 18 se puede observar el acceso remoto a la pantalla de inicio de Wazuh

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/99e9e2e2-e58f-4d00-8963-32c1815ee069)

Figura 18 Inicio Wazuh

En la figura 19 se agrega en el portal del wazuh la IP del servidor y el nombre del agente que corresponde.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/43621d1f-2f38-4f8a-b54d-4e6d02e3be9c)

Figura 19 Ip de del servidor Wazuh y nombre del agente.

Wazuh te brinda ya la línea de código que se debe de correr en el server de Windows (ver Figura 20)

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/2269e1f0-ec23-4b80-9a14-d2ccc8d31e49)

Figura 20 Código brindando por el portal del Wazuh.
 
En los Windows server seleccionados realizamos la instalación con la línea de código facilitado por Wazuh en PowerShell de la Figura 21

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/26297350-63ff-4e4d-bb36-f1a3161a0e13)

Figura 21 Wazuh Agent instalado e iniciado.
 
Una vez instalados los agentes podemos observarlos de la siguiente manera en la página principal del administrador de wazuh como se observa en la Figura 22.

![image](https://github.com/lazuniga03/Wazuh-maestria-grupo3/assets/144503813/46af8061-fd5c-4887-b3b1-d9194fbabc10)

Figura 22 Dashboard del Wazuh
 

