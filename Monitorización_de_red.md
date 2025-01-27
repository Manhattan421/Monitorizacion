# Comandos para la monitorización de red:
### Comando tcpdump
Este comando proporciona toda la información sobre la RAM, cuanta RAM se está utilizando, cuenta está disponible, etc. 
El comando free sin opciones nos devolverá entonces los resultados para la memoria Total, Usada y Libre de tu ordenador o servidor.
- tcpdump -i + la interfaz de red, Especifica la interfaz de red en la que quieres escuchar el tráfico.
![free](img/.PNG)
- tcpdump -c + el numero de paquetes, Limita la captura a un número específico de paquetes.
![free](img/.PNG)
- tcpdump -X Muestra el contenido de los paquetes en formato hexadecimal y ASCII. Es útil para ver los datos de los paquetes, como los contenidos de una solicitud HTTP, por ejemplo.
![free](img/.PNG)

### Comando tcptrack
Aunque es una aplicación bastante desconocida, nos muestra todos los datos del consumo de nuestra conexión.
- tcptrack -i + la interfaz de red, Especifica la interfaz de red que deseas monitorear que en nuestro caso es la enp0s3
![free](img/.PNG)
- tcptrack -n Muestra las direcciones IP y puertos en formato numérico, sin intentar resolver los nombres de host o los nombres de servicio. Esto puede hacer que la salida sea más rápida.
![free](img/.PNG)
- tcptrack -v Muestra más detalles sobre las conexiones, como el estado de la conexión
![free](img/.PNG)

### Comando iptraf-ng
Es una herramienta interactiva que proporciona estadísticas detalladas sobre el tráfico de red en tiempo real.
- iptraf-ng -i + la interfaz de red, Especifica la interfaz de red que deseas monitorear.
![free](img/.PNG)
- iptraf-ng -d Muestra estadísticas detalladas sobre la actividad de cada interfaz de red y el tráfico.
![free](img/.PNG)
- iptraf-ng -h Muestra la ayuda, listando todas las opciones disponibles del comando.
![free](img/.PNG)

### Comando netstat
El comando netstat genera visualizaciones que muestran el estado de la red y estadísticas de protocolo.
El estado de los protocolos TCP, SCTP y los puntos finales de UDP puede visualizarse en formato de tabla. 
También puede visualizarse información sobre la tabla de enrutamiento e información de interfaces.
- netstat -u Muestra solo las conexiones UDP activas.
![free](img/.PNG)
- netstat -r Muestra la tabla de enrutamiento del sistema, puedes ver cómo se enrutan los paquetes en la red.
![free](img/.PNG)
- netstat -g Muestra las direcciones de grupo multicast activas.
![free](img/.PNG)
