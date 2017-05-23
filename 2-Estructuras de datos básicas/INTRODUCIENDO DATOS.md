## INTRODUCIENDO DATOS CON INPUT()

### Input devuelve unicamente una cadena de texto en Python 3

En Python 2.x se utilizaban dos funciones para ingresar datos por un teclado, `raw_input()` pasándolo a una cadena de texto, e `input()` evaluándolo como un tipo:

En Python 3.x se sustituyo al `input` de Python 2.x, añadiendo la funcionalidad del `raw_input` como un nuevo `input()`. Si, suena lago raro, pero cómo este curso trata sobre Python 3.x lo que interesa es la funcion en sí, dejando a un lado el como se hacía, o no, antiguamente. 

* Un ejemplo:

```python
print ("Un programa para saber que edad te gustaría tener")

nombre = input("¿Cuál es tú nombre? ")

primero = int(input("¿Qué edad tienes? "))
segundo = int(input("¿Y la edad que quisieras tener? "))

print ("Si yo,",nombre,", con la edad de",primero-segundo,"me conformaría")
