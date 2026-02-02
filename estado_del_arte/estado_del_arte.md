# Estado del Arte

## Sistemas de control de accesos con RFID

Los sistemas de control de acceso con RFID permiten identificar usuarios mediante tarjetas o llaveros sin contacto. En los últimos años, han sido muy utilizados por su bajo costo y facilidad de implementación en proyectos académicos y aplicaciones reales.

###Sistemas con Arduino y RC522

En proyectos académicos, el uso de Arduino junto al lector RC522 es muy común para validar tarjetas RFID. Estos sistemas suelen almacenar una lista de usuarios en el propio dispositivo y activar un actuador (servo o relé) al detectar una credencial autorizada. Su principal limitación es la falta de conectividad y gestión centralizada, lo que restringe el número de usuarios y la auditoría de accesos.

### Evolución con ESP32 y WiFi

El uso del ESP32 representa un avance importante porque permite conectar el sistema a Internet. Esto posibilita enviar datos a una base de datos, gestionar usuarios de forma remota y registrar accesos en tiempo real. Los trabajos revisados muestran que el ESP32 es ideal para integrar RFID con servicios web y almacenamiento remoto.

### Integración con base de datos

La conexión a bases de datos (como MySQL) permite almacenar registros de accesos, usuarios y horarios, lo cual es clave para auditoría y control. Los enfoques más comunes son:

Validación local + registro remoto, o

Validación remota en servidor.

### Actuadores

Para la apertura física se utilizan principalmente servomotores (en proyectos pequeños) y relés para controlar cerraduras eléctricas en sistemas más robustos.

Conclusión

Los sistemas RFID con Arduino/ESP32 y RC522 son una solución accesible para control de accesos. La tendencia actual es integrar ESP32 con bases de datos para gestionar usuarios y registrar accesos en tiempo real. Aun así, se detecta una oportunidad de mejora en seguridad (clonación de tarjetas) y en la gestión avanzada de usuarios. El proyecto de este repositorio se basa en estas implementaciones para desarrollar un sistema funcional con registro en base de datos.
