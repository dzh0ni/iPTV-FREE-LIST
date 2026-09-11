![logo](https://github.com/dzh0ni/iPTV-FREE-LIST/blob/master/Imagenes/xtreamui-R22F.jpg)

# xTream UI r22f

## :information_source: Descripción

Xtream-UI es una plataforma de gestión para servidores de transmisión que permite administrar canales, usuarios, conexiones y recursos desde una interfaz web.

Este repositorio contiene recursos, instrucciones y referencias relacionadas con la instalación y configuración de Xtream-UI r22f.

## :memo: Notas

Asegúrate de tener privilegios de administrador para ejecutar los comandos.

Antes de la instalación, verifica la documentación oficial para cualquier cambio o actualización.

## :computer: Actualizar el sistema
```bash
apt-get update -y 
apt-get upgrade -y
apt-get autoremove -y
apt-get autoclean -y
```
 
## :package: Instalar herramientas y dependencias
```bash
apt-get install -y iperf3 wget git curl nano bzip2 gzip zip unzip dos2unix iftop htop nload speedometer screen perl bc ca-certificates software-properties-common build-essential libxslt1-dev libcurl3 libgeoip-dev python 
```

## :alarm_clock: Configurar la zona horaria
```bash
apt-get install -y tzdata
dpkg-reconfigure tzdata
```

## :earth_africa: Verificar la configuración de la zona horaria
```bash
timedatectl
```

## :arrow_down: Descargar e instalar Xtream-UI
```bash
rm -rf install.py*
wget https://bitbucket.org/emre1393/xtreamui_mirror/downloads/install.py
python install.py
```

## :bulb: Permisos nginx
Si obtiene un error de denegación de permiso de nginx, vuelva a hacer que los binarios de nginx sean ejecutables.

```bash
chmod +x /home/xtreamcodes/iptv_xtream_codes/nginx_rtmp/sbin/nginx_rtmp
chmod +x /home/xtreamcodes/iptv_xtream_codes/nginx/sbin/nginx
/home/xtreamcodes/iptv_xtream_codes/start_services.sh
```

## :bulb: Tablas y archivos .update

Si no puede ver las nuevas tablas de la base de datos después de una nueva instalación, agregue un archivo llamado .update en la carpeta de administración.

```bash
touch /home/xtreamcodes/iptv_xtream_codes/admin/.update
/home/xtreamcodes/iptv_xtream_codes/start_services.sh
```

## :hammer_and_wrench: Requisitos

- Versión recomendada: `Ubuntu 18.04 Server x86_64`
- Se recomienda utilizar una instalación limpia o un sistema recién formateado.
- Se requieren privilegios de `root` o permisos de administrador.
- Se recomienda disponer de una conexión a Internet estable durante la instalación.
- El idioma predeterminado del sistema es el inglés.
- Antes de comenzar, se recomienda realizar una copia de seguridad de cualquier configuración o dato importante.


## :bulb: Recomendaciones

- Se recomienda realizar la instalación sobre un servidor limpio o recién formateado.
- Verifica que el servidor cumpla con los requisitos antes de comenzar.
- Ejecuta los comandos con privilegios de `root` o mediante `sudo`.
- Mantén una conexión a Internet estable durante todo el proceso de instalación.
- Realiza una copia de seguridad antes de modificar una instalación existente.
- Verifica la documentación y compatibilidad de Xtream-UI antes de realizar actualizaciones.
- No ejecutes comandos de fuentes desconocidas sin revisar previamente su contenido.
- Después de la instalación, comprueba que todos los servicios de Xtream-UI estén funcionando correctamente.

## :blue_book: Recursos y documentación

- **Guía oficial:** [Xtream-UI](https://xtream-ui.org/xtream-ui-r22f)
- **Instalador en GitHub:** [xtream-ui-install](https://github.com/xtream-ui-org/xtream-ui-install)
- **Lofertech:** [Guía de instalación](https://lofertech.com/xtream-ui-installation)
- **Mexiqueando:** [Instalación paso a paso](https://mexiqueando.site/xtream-ui-r22f-instalacion-paso-a-paso/)
- **ForoISP:** [Información y configuración](http://foroisp.com/threads/1776-Cabecera-IPTV-Servidor-Xtream-UI-Parte-6)
- **Tutoriales de Emre1393:** [YouTube](https://www.youtube.com/@emre1393)
- **Proyecto Emre1393:** [Instalador](https://bitbucket.org/emre1393/xtreamui_mirror/src/master) | [Librerías](https://bitbucket.org/emre1393/xtreamui_mirror/downloads)

## :email: Contacto

- :busts_in_silhouette: **dZh0ni:** [Telegram](https://t.me/dZh0ni_Dev) — Mantenedor del repositorio

☆ dZh0ni ☆
