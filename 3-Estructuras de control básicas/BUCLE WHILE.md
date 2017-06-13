## BUCLE WHILE

La instrucción while crea un blucle que se ejecutará mientras su condición sea cierta.

La estructura de while es la siguiente:
```python
while condicion:
    instruccion_a_ejecutar
```
[ejemplo while 1](https://gist.github.com/psicobyte/49558d950abd5026abc7#file-ejemplo-while-1) hosted with ❤ by [GitHub](https://github.com)

Por ejemplo:
```python
while a < 10:
    print(a)
    a = a + 1
```
[Ejemplo while 2](https://gist.github.com/psicobyte/37c8f3f49d8bb66a8d38#file-ejemplo-while-2) hosted with ❤ by [GitHub](https://github.com)

Este ejemplo irá recorriendo el bucle, imprimiendo el valor de "a" y sumándole uno, mientas este sea menor que 10.

While también permite una sentencia "else" que se ejecutará cuando la condición del bucle no sea cierta (es decir, fuera del blucle) de este modo:
```python
while condicion:
    instruccion_a_ejecutar
else
    instruccion_fuera_del_bucle
```
[Ejemplo while 3](https://gist.github.com/psicobyte/cf8864c3dc5d8e82d6a9#file-ejemplo-while-3) hosted with ❤ by [GitHub](https://github.com) 
