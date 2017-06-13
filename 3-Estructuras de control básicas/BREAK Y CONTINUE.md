**Break y continue**

Adicionalmente al control que nos permiten las instrucciones *for* y *while*, Python nos ofrece herramientas para ajustar su comportamiento.

La sentencia break, dentro de for o while, permite interrumpir el flujo normal del bucle, saliendo automáticamente de él independientemente de si se cumple o no la condición del bucle.

Por ejemplo:
```python
x= 0
while x < 10:
    if x == 5
        break
    print x
x = x + 1
```

Este bucle se interrumpirá cuando x valga 5 (valor que no llegará a imprimirse), aunque se siga cumpliendo la condición de while.

Hay que precisar que *break* sale **completamente** del bucle, con lo que no se ejecutará tampoco ninguna instrucción "else" que este pudiera tener.

Menos "dramática" que *break* es la instrucción continue. Esta permite interrumpir el ciclo como lo hace *break*, pero sin salir del bucle. De este modo sólo se interrumpe una iteración.

Por ejemplo:
```python
x= 0
while x < 9:
    x = x + 1
    if x == 5:
        continue
print x
```

Este ejemplo, pese a ser casi idéntico al anterior, tiene un resultado distinto. Esta vez se imprimirán todos los números del 1 al 10 (como está especificado en la cláusula del *while*), pero 
omitiendo el 5 (que ha sido saltado por el *continue*).
