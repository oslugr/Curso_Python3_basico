## CIERTO Y FALSO

Las estructuras que permiten controlar el flujo de un programa se basan, fundamentalmente, en el "valor de verdad" de una sentencia.

¿Qué es un valor lógico "cierto" o "falso" para Python?

En general, los valores no definidos, cadena vacía, lista vacía y el 0 son interpretado como "falso".

El resto de valores se consideran "cierto".

Naturalmente, el valor de verdad puede ser (y suele ser) el resultado de una operación de comparación.

Los operadores de comparación son los siguientes:
```python
    menor que ("<")
    mayor que (">")
    igual a ("==")
    menor o igual que ("<=")
    mayor o igual que (">=")
    distinto de ("!=")
    está en ("in")
    no está en ("not in")
    es ("is")
    no es ("is not")
```
Todos estos operadores retornarán valores de "cierto" o "falso".

Se pueden unir proposiciones con los habituales operadores lógicos "and" (y) y "or" (o), y también existe la preposición "not" (no), para invertir el valor de verdad.El primer programa suele ser el clásico que imprime un mensaje por la pantalla. En Python sería de esta forma:
print "Hola, mundo libre"

Que aparecerá de la forma siguiente si lo ejecutamos directamente desde el intérprete:
```python
python3.6
Python 3.6.1 (default, Mar 22 2017, 06:17:05) 
[GCC 6.3.0 20170321] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print ("¡Hola, Mundo Libre!")
¡Hola, Mundo Libre!
```
Como veis, tiene dos partes: la orden print y la cadena de caracteres, entre paréntesis y comillas, ("Hola, mundo libre"). A diferencia de otros lenguajes, en python 3 `print` es una función y por lo tanto debe llevar los paréntesis. Por tanto que sea la función `print` tiene otras ventajas, por ejemplo utilizando parámetros opcionales, pudiendo controlar el salto de línea `(\n)` reemplazandolo por otra cosa:
```python
print ("¡Hola, Mundo Libre!,", end="")
print (" agregamos cualquier texto más")
```
Lo más habitual en los programas es tenerlos en un fichero aparte. Editémoslo (con alguno de los editores anteriores) y guardémoslo en hola.py. Ya que tenemos abierta la línea de comandos con Python, salgamos de ella (quit() o `control-d` en UNIX o `Control-Z` en Windows) y ejecutémoslo directamente con:

`python hola.py`

El resultado será el mismo de antes, como es natural.

En entornos Linux/Unix es habitual también incluir al principio del fichero con el programa una línea que permite ejecutarlo directamente desde línea de comandos, sin necesidad de llamar explícitamente al intérprete. Esta línea, llamada "shebang", suele ser `#!/usr/bin/python` o `#!/usr/bin/env python` (esta última más genérica). El fichero quedaría algo así:
```python
#!/usr/bin/python
print ("¡Hola, Mundo Libre!")
```
(Nótese la línea en blanco). Para hacerlo ejecutable se sigue también el procedimiento habitual en Linux:

`chmod +x hola.py`

con lo que posteriormente ya se puede ejecutar también de la forma habitual:

`bash% ./hola.py`

Los **"./"** puede que no sean necesarios si se tiene el propio directorio incluido en el camino de ejecución, pero no suele ser una práctica habitual (ni segura) así que es mejor curarse en salud haciendo de la forma anterior. El resultado, de todas formas, tiene que ser el mismo.
