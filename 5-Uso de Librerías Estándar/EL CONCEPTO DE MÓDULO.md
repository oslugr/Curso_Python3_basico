## EL CONCEPTO DE MÓDULO

Un módulo es una parte de algo. Algo es modular si es posible separarlo en partes o piezas. Los bloques de LEGO son el ejemplo perfecto de modularidad. Puedes coger diferentes piezas y crear diferentes cosas con ellas.

En Python, un módulo es una pequeña pieza de un gran programa. Sencillamente un módulo es un fichero dentro de tu disco duro. En el caso de Pyhton es un fichero cuya [extensión](https://es.wikipedia.org/wiki/Extensi%C3%B3n_de_archivo) es .*py

Motivos por los que usar módulos:

* Se crean ficheros pequeños, donde es mas fácil de localizar elementos de tu código.

* Un módulo se puede usar en todos los programas que desees. Sin necesidad de repetir código fuente.

Para un nuevo módulo, se crea un fichero y se nombra como **"nombre_modulo.py"**. En este fichero incluimos el código que necesitemos para resolver problemas dentro de un determinado ámbito, por ejemplo, le asigno el nombre *"matematicas.py"* a mi fichero. Lo ideal es incluir dentro de este fichero funciones, para hacer determinados cálculos matemáticos. Una función que calcule las raíces de un polinomio de segundo grado no debería faltar en nuestro módulo.

Para utilizar las funciones de nuestro módulo escribiremos en nuestro archivo las siguientes palabras: **import matematicas**. De esta forma tendremos disponibles todas las funciones que están definidas en nuestro fichero *"matematicas.py"*, las cuales usaremos en el nuevo programa.

A la hora de importar un módulo, Python recorre todos los directorios indicados en la variable de entorno PYTHONPATH en busca de un archivo con el nombre adecuado. El valor de la variable PYTHONPATH se puede consultar desde el intérprete de Python con dos sencillas órdenes. En primer lugar **"import sys"** y después **"sys.path"** *(!ojo! en el intérprete no escribimos las comillas)*.

En los siguientes apartados conoceremos los módulos estándar de Python y las funciones más utilizadas dentro de cada módulo. 