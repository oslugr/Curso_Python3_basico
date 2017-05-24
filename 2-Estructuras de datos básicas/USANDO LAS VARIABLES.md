## USANDO LAS VARIABLES

Para saber el tipo de una variable, tenemos la función **type**, que se usa del siguiente modo:

`type(MiVariable)` 

Donde **MiVariable** es la variable de la que queremos saber el tipo.

Esta función retorna el tipo de dato de la variable.

Por ejemplo:

Prueba a ejecutar el siguiente código.
```python
#!/usr/bin/python3.6

# Esto es un entero

Entero = 32 

# Esto es una cadena 

Cadena = "Hola Mundo" 

print(type(Entero)) 
print(type(Cadena)) 
```
Existen una serie de *"alias"* previstos para poder hacer comparaciones con los valores que retorna **type()**, de los cuales los más usado son los siguientes:

* bool Para valores lógicos "Cierto" o "Falso", como se verá más adelante en este curso.
* float Para números en coma flotante.
* int Para números enteros.
* str Para variables de tipo cadena.

*En realidad, type no sólo funciona con variables, si no que también tiene uso en contextos de cadenas, arrays, funciones, clases, módulos y cualquier otra estructura que pueda tener un tipo.*

## Cambiado el tipo de dato en una variable

Dado que Python es tan exigente a la hora de tratar con los tipos de datos, se hace necesario un procedimiento para cambiar de un tipo a otro, para así poder operar con ellos.

Python posee una serie de funciones que permiten esto mismo, y que funcionan del mismo modo general: Se les introduce un dato de un tipo determinado y retornan ese mismo valor, pero de un tipo distinto.

Los más habituales son los siguientes:

* **str(MiVariable)** Convierte MiVariable a una cadena.
* **int(MiVariable)** Convierte MiVariable a un entero.
* **float(MiVariable**) Convierte MiVariable a un número en coma flotante.

El siguiente código cambiaría el tipo de dato de Entero **(int)** a Cadena **(str)**:
```python
#!/usr/bin/python3.6

# Esto es un entero
Entero = 2000

#Convertimos a Cadena
Cadena= str(Entero)

print(type(Entero))
print(type(Cadena)) 
```
