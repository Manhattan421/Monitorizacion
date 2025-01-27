# Comandos para la monitorización de almacenamiento:
### Comando free
El comando free muestra cómo está usando el sistema la memoria RAM. Cuando se ejecuta muestra cuánta memoria está siendo usada, cuánta está libre y cuánto espacio está siendo utilizado por el sistema para guardar datos temporales. Es como un vistazo rápido para saber si el sistema está usando mucha memoria o si tiene suficiente espacio disponible para ejecutar más programas.
- free -b  Muestra la memoria en bytes
![free](img/free-b.PNG)
- free -m  Muestra la memoria en megabytes (MB).
![free](img/free-m.PNG)
- free -g  Muestra la memoria en gigabytes (GB).
![free](img/free-g.PNG)

### Comando df
El comando df muestra cuánto espacio tiene disponible los discos o particiones del sistema. Es una herramienta para ver el "estado" del almacenamiento, muestra cuánto espacio tiene en total, cuánto ha usado y cuánto queda libre. Es útil para saber si el disco en cuestión está lleno o si aún queda espacio para guardar daots.
- df -T Muestra el tipo de sistema de archivos de cada partición (por ejemplo, ext4, xfs, nfs, etc.).
![ps](img/df-T.PNG)
- df -a Muestra todos los sistemas de archivos, incluidos los sistemas de archivos con 0 bloques de uso, como los montajes virtuales (por ejemplo, proc, sysfs, tmpfs, etc.).
![ps](img/df-a.PNG)
- df -l Muestra solo los sistemas de archivos locales (excluyendo los montajes de red como NFS, CIFS, etc.).
![ps](img/df-l.PNG)

### Comando du
Es un comando que significa “Disk Usage” (uso de disco). Su función principal es mostrar el espacio en disco utilizado por archivos y directorios en el sistema.
- du -x Muestra solo los archivos y directorios en el mismo sistema de archivos. Esto puede ser útil si tienes montajes de red o particiones adicionales.
![du](img/du-x.PNG)
- du -l Cuenta los archivos múltiples (con enlaces duros) solo una vez, en lugar de contar cada enlace por separado.
![du](img/du-l.PNG)
- du -P Muestra el tamaño del enlace simbólico en sí.
![du](img/du-P.PNG)

### Comando iostat
El comando iostat se usa para ver cómo están funcionando los discos y dispositivos de almacenamiento en el sistema. Muestra estadísticas sobre la velocidad de lectura y escritura de los discos y cuánta carga tienen en ese momento. Es útil para saber si los discos están trabajando muy lento o si hay algo que los está sobrecargando.
- iostat -c Muestra las estadísticas de la CPU, como el porcentaje de uso de la CPU para el sistema, la aplicación de usuario y el tiempo de inactividad.
![iostat](img/iostat-c.PNG)
- iostat -z Omite los dispositivos que no han tenido actividad de entrada/salida.
![iostat](img/iostat-z.PNG)
- iostat -t Muestra la hora en que se toma cada muestra de las estadísticas.
![iostat](img/iostat-t.PNG)
