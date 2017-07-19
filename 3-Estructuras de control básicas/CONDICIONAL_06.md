## CONDICIONAL

En `Python`, el anidamiento de funciones no se hace con llaves ni otros símbolos contenedores, si no por medio de la indentación. Las instrucciones con un nivel de indentación (un tabulador) están contenidas en las que no están indentadas que les preceden, las instrucciones con dos tabuladores están incluidas en las anteriores, etc.

La estructura básica para el control del flujo de un programa es el "si condicional", que permite la ejecución de un segmento de código dependiendo de las condiciones concretas.
```python
if expresion_a_evaluar:
    ejecutar_si_cierto
```
[ejemplo-if-1](https://gist.github.com/psicobyte/423d624787386e1b4d24#file-ejemplo-if-1) hosted with ❤ by [GitHub](https://github.com)

(Nota los dos puntos (:) detrás de la expresión). Como toda estructura de control en Python, la definición de la función termina con los dos (:) puntos e irá identada (4 espacios).

En este caso, la sentencia "ejecutar_si_cierto" solo se ejecutará si "expresion_a_evaluar" devuelve un valor lógico "cierto", y se ignorará si retorna un valor de "falso".

La anterior estructura puede ampliarse añadiendo un bloque alternativo:
```python
if expresion_a_evaluar:
    ejecutar_si_cierto
else:
    ejecutar_en_caso_contrario
```
[ejempli-if-2](https://gist.github.com/psicobyte/6cd4752b4df4b2a4ae23#file-ejempli-if-2) hosted with ❤ by [GitHub](https://github.com)

En este caso, el código incluído dentro del bloque else se ejecutará sólo si "expresion_a_evaluar" tiene un valor falso.

O también existe la siguiente generalización:
```python
if expresion_a_evaluar_1:
    ejecutar_si_cierto_1
elif expresion_a_evaluar_2:
    ejecutar_si_cierto_2
elif expresion_a_evaluar_3:
    ejecutar_si_cierto_3
else:
    ejecutar_si_ninguna
```
[Ejemplo-if-3](https://gist.github.com/psicobyte/39f5509ca43a777d14f0#file-ejemplo-if-3) hosted with ❤ by [GitHub](https://github.com)

En la que se dan varias opciones, que se ejecutarán cuando sea cierta la expresión correspondiente, y una última que sólo se ejecutará si no es cierta ninguna de las anteriores.
Por ejemplo:
```python
if x > 10:
    print("La variable es mayor que diez")
elif x < 10:
    print("La variable es menor que diez")
else:
    print("La variable es, precisamente, diez")
```
[Ejemplo-if-4](https://gist.github.com/psicobyte/eb7a19e6d515c053462f#file-ejemplo-if-4) hosted with ❤ by [GitHub](https://github.com) 

