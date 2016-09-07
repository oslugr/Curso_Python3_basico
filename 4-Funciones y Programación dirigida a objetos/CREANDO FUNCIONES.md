## CREANDO FUNCIONES

Otra forma de definir el concepto de función es como un fragmento de código con un nombre asociado que realiza una serie de tareas y devuelve un valor. A los fragmentos de código que tienen un nombre asociado y no devuelven valores se les suele llamar procedimientos. En Python no existen los procedimientos, ya que cuando el programador no especifica un valor de retorno la función devuelve el valor None, equivalente al null de Java.

El formato general para usar en funciones Python, es el siguiente:
```python
 def nombre_funcion(arg1,arg2,... argN):

	 cuerpo
```
Aparece la palabra reservada def que es la abreviatura de define en inglés, la cual crea una función y le asigna un nombre. En las siguientes lineas, indentadas, se coloca el cuerpo de la función. Estas instrucciones se ejecutaran cuando la función sea llamada o invocada, en definitiva, cuando la utilicemos.

A continuación del nombre, como en la mayoría de lenguajes, aparece la lista de argumentos, que puede estar vacía.

Cuando sea necesario, en el cuerpo de la función se utilizará la palabra reservada return:
```python
 def nombre_funcion(arg1,arg2,... argN):

 	...

	return valor
```
Se utilizar al final de cuerpo, para enviar un resultado al lugar donde se hizo la llamada a la función.
```python
 def cuadrado(x):

	 return x**2
```
En el ejemplo anterior, podríamos leerlo así: se define la función cuadrado de x como el valor que resulta de elevar x al cuadrado.

Veamos un primer ejemplo, más completo:
```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

def tablasMultiplicar():
    for i in range(0,11):
        print "\n Tabla del ", i , "\n"
        for j in range(0,11):
            print i, " X ", j, " = ", i*j
            
tablasMultiplicar()
```