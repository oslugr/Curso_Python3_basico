## OBTENER AYUDA SOBRE UN MÓDULO

A continuación practicarás con comandos que ofrecen información necesaria para hacer un buen uso de los módulos de Python.

El comando **dir(nombre_modulo)** imprime un listado con las funciones disponibles para ese módulo.

Para obtener información específica de una función incluida en un módulo, lanzaremos el comando **help(nombre_modulo.nombre_funcion)**.

Prueba las siguientes órdenes en el interprete de Python:
```python
>>> import os 

>>> dir(os) 

>>> help(os) 

>>> help(os.getcwd) 
```