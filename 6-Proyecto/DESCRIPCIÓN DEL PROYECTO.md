## DESCRIPCIÓN DEL PROYECTO  

El proyecto trata de evaluar lo que se ha aprendido de este lenguaje a lo largo del curso, y será obligatorio entregarlo y superarlo para aprobar el curso. En general, habrá que usar todos los conocimientos descritos en los diferentes módulos del curso:
Consistirá en crear un programa que convierta un fichero de texto separado por comas (CSV) en una página HTML con una tabla que incluya el mismo fichero. El programa tendrá que leer de un fichero CSV los siguientes datos:

* Nombre,apellido1,apellido2,email
* Nombre,apellido1,apellido2,email
* Nombre,apellido1,apellido2,email
* Nombre,apellido1,apellido2,email
* Nombre,apellido1,apellido2,email
* (...etcétera...)

y convertirlo en una página web que incluya la siguiente tabla

| Nombre     | Apellido1   | Apellido2    | Email          |
|:-----------|:------------|:-------------|:---------------|
| Elena      | Nito        | Del Bosque   | elena@gmail.com|
| Achero     | Galvan      | Izado        | achero@yahoo.es|

La tabla debe contener tantas filas como lineas tenga el fichero csv.

El programa deberá solicitar el nombre del fichero CSV que debe abrirse y nombre del fichero HTML que debe crearse, y debe gestionar e informar de incidencias tales como que los ficheros no existan o no puedan crearse.

El alumno enviara el **proyecto_nombrealumno.py**, para comprobar su funcionamiento. Se valorará positivamente el uso adecuado de los conceptos con los que se ha trabajado durante el curso