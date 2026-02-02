# Estado del Arte

## Sistemas de control de accesos con RFID

## Introducción
Los sistemas de control de accesos permiten restringir la entrada a espacios físicos
mediante algún método de identificación. Actualmente, la tecnología RFID es una de las
más utilizadas por su bajo costo y facilidad de implementación.

Este estado del arte revisa proyectos relacionados con sistemas de control de accesos
basados en RFID, similares al proyecto desarrollado en este repositorio.

## Desarrollo
La mayoría de los proyectos analizados utilizan tarjetas o llaveros RFID que son leídos
por un microcontrolador. Los lectores más comunes son el RC522, debido a su
compatibilidad con Arduino y ESP32.

Una tendencia clara es el uso del ESP32 por su conectividad WiFi, lo que permite validar
accesos y almacenar registros en bases de datos como MySQL. Para la apertura física se
emplean relés, servomotores o cerraduras eléctricas.

## Conclusión
Los sistemas de control de accesos con RFID son una solución ampliamente utilizada. El
proyecto presentado se basa en estas implementaciones para desarrollar un sistema
funcional y práctico.
