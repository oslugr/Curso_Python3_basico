## CONTROL DE EXCEPCIONES

Cosas como la clásica división por cero o el tratamiento de tipos de datos incompatibles (sumar cadenas, por ejemplo) provocarán errores en tiempo de ejecución (excepciones) que darán al traste con el programa.

Para facilitar el manejo de este tipo de cosas tenemos la estructura *try*:

Dicho de un modo simple, lo que hace *try* es ejecutar un bloque de sentencias en un "entorno controlado", para que el error generado (si se da) no detenga el programa, si no que se retorne de modo que pueda manejarse.

Veámoslo con un ejemplo. En el siguiente bloque:
```python
resultado = dividendo/divisor
print("La división resulta: ", resultado)
```

Si *divisor* tuviese el valor "0" el programa daría un error y se interrumpiría. Para prever esa posibilidad se puede modificar así:
```python
try:
resultado = dividendo/divisor
    print("La división resulta: ", resultado)
except:
    if divisor == 0:
print("No puedes dividir por cero, animal")
```

El bloque dentro de *try* es ejecutado y **si retorna cualquier error**, entonces ejecuta el bloque contenido en *except*, en caso contrario se continúa la ejecución del programa ignorando ese bloque.

(De acuerdo, la descrita es una solución muy limitada, pero se puede incluir en un bucle mayor para que permita volver a introducir el dato, etc...)

Dado que existen muchos tipos de errores distintos, sería deseable una forma algo más sofisticada y concreta de manejar estos. En el caso de arriba, por ejemplo, el programa puede dar un error si divisor es cero o si es una cadena, y sería deseable manejar ambos casos de distinta manera.

Para ello, *except* permite escribirse de modo que indique el tipo de error concreto al que responde, de la siguiente forma:
```python
except Tipo_de_Error:
```

Y, además, pueden colocarse tantos bloques *except* como sean necesarios.

De este modo, nuestro ejemplo se podría mejorar más o menos así:
```python
try:
    resultado = dividendo/divisor
    print("La divisón resulta: ", resultado)
except ZeroDivisionError:
    if divisor == 0:
        print("No puedes dividir por cero, animal")
except ValueError:
    if divisor == 0:
print("Hay que ser bruto: eso no es un número")
```

Cada uno de los bloques *except* se ejecuta sólo si se da el tipo de error especificado.

Puedes ver un listado exhaustivo de códigos de excepciones y su descripción en la [documentación de python](https://docs.python.org/3/library/exceptions.html).

Si estás pensando que esto se parece a un *if* un tanto sofisticado tienes razón. De hecho, esta estructura permite también una sentencia *else*, que se ejecuta cuando no hay errores. De este modo, el ejemplo anterior sería más correcto escrito así:
```python
try:
    resultado = dividendo/divisor
except ZeroDivisionError:
    if divisor == 0:
    print("No puedes dividir por cero, animal")
except ValueError:
    if divisor == 0:
        print("Hay que ser bruto: eso no es un número")
else:
print("La divisón resulta: ", resultado)
```

Nota que dentro del *try* hemos dejado sólo la instrucción que requiere que verifiquemos, dejando el *"print"* en el else final.

