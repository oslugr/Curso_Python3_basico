Si se tienen problemas para introducir ciertos caracteres, como los acentos o la letra *Ñ*, el interprete de python responderá con un error con un aspecto similar a esto:

`SyntaxError: Non-ASCII character '\xxx' in file programa.py on line X, but no encoding declared; see http://www.python.org/peps/pep-0263.html for details`

Python, en principio, asume que la codificación es ASCII y, por tanto, no reconocerá caracteres fuera de esa codificación. Para solucionar esto, los documentos deberán ser definidos como UTF-8.

Para advertir a python de que este es el formato, la forma más simple es indicarlo por medio de una "Línea mágica". Justo debajo del shebang (eso de #!...), se coloca lo siguiente:

```python
# -*- coding: utf-8 -*-
```
de modo que la cabecera quedaría más o menos así:
```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
```
Con esto, el interprete de python debería admitir el uso de caracteres **UTF-8** en nuestros scripts. En cualquier caso, no es recomendable el uso de caracteres no **ASCII** en nombre de variables o funciones, etc.

Para más detalles o casos más complejos, se recomienda consultar la [página de información](https://www.python.org/dev/peps/pep-0263/) que indica el propio mensaje de error.
