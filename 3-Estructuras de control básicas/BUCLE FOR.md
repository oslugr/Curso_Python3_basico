*BUCLE FOR*

El bucle **for** sirve para recorrer secuencialmente los elementos de una lista.

La estructura de for es la siguiente: 
```python
for Variable in Lista:
  instrucciones
```

Esto ejecutaría "instrucciones" para cada elemento de "Lista", que se ha ido almacenando en "Variable". Veámoslo con un ejemplo: 
```python
Huerto = ["zanahoria", "col", "lechuga", "col"]

for Planta in Huerto:
    if Planta != "col"
        print Planta
    else
print("Odio las coles")
```

Este ejemplo imprimirá cada uno de los valores de la lista "Huerto", a menos que este sea "col", en cuyo caso imprimirá el texto "Odio las coles".

El bucle **for**, al igual que vimos con **while**, también permite el uso de una cláusula **"else"** que se ejecutará cuando no quede ningún valor en la lista.
```python
for Variable in Lista:
    instrucciones
else
ya_no_quedan_elementos
```

A veces, este tipo de bucle puede resultar poco intuitivo. Aquellos que estén acostumbrados a otros lenguajes de programación comprobarán que el uso de for 
en Python (como una herramienta de recorrido de arrays) se corresponde, a lo que en lenguajes como Perl se llamaría foreach, más que a un for típico.
