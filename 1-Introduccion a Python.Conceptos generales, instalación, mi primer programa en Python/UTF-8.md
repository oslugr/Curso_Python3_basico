Ahora, en Python 3, las cadenas por defecto son Unicode (utf-8), por tanto ya no que hay que declarar ni
guardar el archivo en esa codificación, ni con la anterior `# -*- coding: utf-8 -*-` línea debajo del shebang.

Por tanto, ahora funcionará normalmente e inmediatamente al ejecutar algo como lo siguiente con "ñ" y/o "acento":
```python
print("mis ñus són animales de ñulandía jeje")
```
En Geany habrá que especificar que utilice Python3 en `> Construir > Establecer comandos de construcción`:

![](https://github.com/Makova/Curso_Python3_basico/blob/master/img/python3-Geany1.png)
![](https://github.com/Makova/Curso_Python3_basico/blob/master/img/python3-Geany2.png)

