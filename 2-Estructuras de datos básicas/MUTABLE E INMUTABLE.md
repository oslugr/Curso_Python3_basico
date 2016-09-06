## MUTABLE E INMUTABLE

En otros lenguajes de programación, las variables se pueden ver como "cajas" en las que se guarda un valor (una cadena, un número, etc).

Esta imagen también sirve en Python como una primera aproximación, pero la cosa es un poco más compleja.

En realidad, en Python, las variables deberían ser vistas como etiquetas, más que como cajas: Cuando asignamos un valor a una variable, en realidad estamos creando una variable con un nombre interno asignado por python (que nosotros no necesitamos conocer, pero que se puede ver con la función "id()") y a esa variable le asignamos una "etiqueta" con el nombre que hayamos usado para nuestra variable (por eso en Python el nombre realmente correcto para los nombres de variable es "identificadores").

Esto sirve tanto para variables, como para funciones, objetos, etc.

Python actúa de este modo porque es más eficiente a la hora de gestionar recursos. Por ejemplo, cuando asignamos el valor de esa variable a otra (haciendo algo como "variable2 = variable1") python no crea una vriable nueva, sino que asigna una nueva "etiqueta" al valor incial, de modo que tenemos un sólo dato almacenado en la memoria, pero referenciado por dos nombres distintos.

Pero ¿Qué pasa si modficamos el valor de una de las variables pero no el de la otra? Que Python elimina la etiqueta correspondiente a la variable modificada y crea una nueva variable (on un id interno distinto) con el nuevo valor.

Veamoslo con un ejemplo:

    #/usr/bin/python
    # -*- coding: utf-8 -*-

    # Ejemplo de variables e IDs

    # asignamos un valor a una variable:

    primera_variable = 5

    # copiamos ese valor en otra:

    segunda_variable = primera_variable

    # vamos a ver los id de cada una:

    print "ANTES"
    print "ID de la primera variable:"
    print id(primera_variable)

    print "ID de la segunda variable:"
    print id(segunda_variable)
    # como vemos, son el mismo.

    # modificamos la segunda:

    segunda_variable = segunda_variable + 1

    # Y volvemos a ver los id:

    print "DESPUES"

    print "ID de la primera variable:"
    print id(primera_variable)

    print "ID de la segunda variable:"
    print id(segunda_variable)

    # como vemos, la segunda ha cambiado
    view raw
[ejemplo-ids.py](https://gist.github.com/psicobyte/8b833540812d24ea10a49b8cd54969de#file-ejemplo-ids-py) hosted with ❤ by [GitHub](https://github.com/)

Aunque este funcionamiento interno de Python es bastante distinto de otros lenguajes, esto no afecta al uso pr nuestra parte, y podemos trabajar como con cualquier otro.

Escepto por un detalle.

Normalmente, cuando modificamos una variable, esta es destruída y creada una nueva. pero si se trata de, por ejemplo, una lista, esto no ocurre así.

Si modificamos una lista, el ID sigue siendo el mismo (porque, en realidad, hemos modificado uno o más elemmentos de la lista, lno la lista en sí).

La consecuencia es que, si copiamos una lista en otra, y modificamos una de ellas ¡La otra también cambia!

Este ejemplo seguramente aclare las cosas:

    #/usr/bin/python
    # -*- coding: utf-8 -*-

    # Ejemplo de listas e IDs

    # creamos una lista:

    primera_lista = [1, 2, 3]

    # la copiamos en otra:

    segunda_lista = primera_lista

    # las mostramos:

    print "primera lista:"
    print primera_lista

    print "segunda lista:"
    print segunda_lista
    # son iguales.

    # modificamos el primer elemento de la segunda lista:

    segunda_lista[0] = 1000

	# y las mostramos otra vez:

	print "DESPUES"

	print "primera lista:"
	print primera_lista

	print "segunda lista:"
	print segunda_lista
	# Han cambiado ambas!!!
	view raw
[ejemplo-modificar-listas.py](https://gist.github.com/psicobyte/3b2102c51e2bd1030a6e351252332841#file-ejemplo-modificar-listas-py) hosted with ❤ by [GitHub](https://github.com/)

Si queremos copiar una lista en otra y que realmente sean listas independientes, podemos hacerlo explícitamnete, usando la función "list()" de este modo:

	#/usr/bin/python
	# -*- coding: utf-8 -*-

	# Copiando listas

	# creamos una lista:

	primera_lista = [1, 2, 3]

	# la copiamos en otra:

	segunda_lista = list(primera_lista)
	view raw
[copiar-listas.py](https://gist.github.com/psicobyte/ca8cfaceebc209ba52cc86db3786f1a1#file-copiar-listas-py) hosted with ❤ by [GitHub](https://github.com/)

Dejo como ejercicio para cada uno el probar que, efectivamente, esto crea dos listas distintas.

Los objetos de Python que, como los números, son destruídos y creados de nuevo al modificarlos se llaman "inmutables". Los que pueden modificarse sin que cambie su ID son llamados "mutables".

Las listas, y diccionarios, por ejemplo, son mutables. Los números, cadenas o tuplas son inmutables.
