## COMENTARIOS

Para ayudar a mantener el código, indicar detalles o, en general, añadir textos que deben ser leído por personas pero no por el interprete o el compilador, los lenguajes de programación suelen incluir algún modo de indicar que algo es un "comentario", y no una instrucción.

En Python, los comentarios comienzan con el signo almohadilla ]](#)]] seguido de un espacio.

La siguiente línea sería un comentario y, por lo tanto, sería ignorada por el intérprete de python:
```python
# Esto es un comentario`
```
[Comentarios 1](https://gist.github.com/psicobyte/de5d26425de5b7d0ab2e#file-comentarios-1) hosted with ❤ by [GitHub](https://github.com/)

Esto ocurre unque lo que haya tras el # sea código de python. En el siguiente ejemplo el valor final de "variable" es 10, y no 5:
```python
variable= 10
# variable= 5
```
[comentarios 2](https://gist.github.com/psicobyte/0fffabfafd4043f1798f#file-comentarios-2) hosted with ❤ by [GitHub](https://github.com/)

Un comentario también puede estar a continuación de código interpretable, en la misma línea, de este modo:
```python
gravedad= 9.8 # aceleración de gravedad en la Tierra, en m/s^2
```
[Comentarios 3](https://gist.github.com/psicobyte/b8276f7cdfed769e6c92#file-comentarios-3) hosted with ❤ by [GitHub](https://github.com/)

Es más que recomendable usar los comentarios para documentar el código lo máximo posible, tanto para los demás como para leerlo tú mismo. Hoy puedes saber qué hace exactamente, pero mañana lo olvidarás.

En palabras de Martin Golding: "Programa siempre como si el tipo que acabe manteniendo tu código fuera un psicópata violento que sabe dónde vives."

Además, pŕacticamente todo programa debería empezar con un comentario indicando qué es, para qué se usa, el autor y la licencia:
```python
#################https://gist.github.com/psicobyte/b8276f7cdfed769e6c92#file-comentarios-3#########################
#
# Copyright 2011 Allan Psicobyte
#
# Programa para resolver problemas NP en tiempo polinómico
#
# Es software libre y se distribuye bajo una licencia Affero (AFFERO GENERAL PUBLIC LICENSE: http://www.affero.org/oagpl.html).
#
# This program is free software and it's licensed under the AFFERO GENERAL PUBLIC LICENSE (http://www.affero.org/oagpl.html ).
#
##########################################
```
[Comentarios 4](https://gist.github.com/psicobyte/84e38fa5e13149515fd8#file-comentarios-4) hosted with ❤ by [GitHub](https://github.com/)

¿Te ha sabido a poco? Un método más avanzado de mantener una buena documentación en Python es por medio de Docstrings.
