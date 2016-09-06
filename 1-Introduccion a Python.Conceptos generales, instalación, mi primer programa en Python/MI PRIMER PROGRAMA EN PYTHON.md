El primer programa suele ser el clásico que imprime un mensaje por la pantalla. En Python sería de esta forma:
print "Hola, mundo libre"

Que aparecerá de la forma siguiente si lo ejecutamos directamente desde el intérprete:

`Python 2.6.5 (r265:79063, Apr 16 2010, 13:09:56) [GCC 4.4.3] on linux2 Type "help", "copyright", "credits" or "license" for more information. >>> print "Hola, mundo libre" Hola, mundo libre >>>`

Como veis, tiene dos partes: la orden print y la cadena de caracteres, entre comillas, "Hola, mundo libre". A diferencia de otros lenguajes, en muchos casos en Python se pueden evitar los paréntesis en las llamadas a funciones; este es uno de ellos. Resulta obvio que el argumento para la función print es la cadena, así que ¿para qué más? Por otro lado, la cadena está entre comillas, como resulta habitual, y print incluye un retorno de carro al final de la misma, también como suele ser habitual. Por último, se utiliza como terminador de la orden el simple retorno de carro; no hace falta ningún otro carácter para indicarlo. Si ya está claro que se ha acabado, ¿para qué poner más cosas?

Lo más habitual en los programas es tenerlos en un fichero aparte. Editémoslo (con alguno de los editores anteriores) y guardémoslo en hola.py. Ya que tenemos abierta la línea de comandos con Python, salgamos de ella (quit() o control-d) y ejecutémoslo directamente con:
python hola.py

El resultado será el mismo de antes, como es natural.

En entornos Linux/Unix es habitual también incluir al principio del fichero con el programa una línea que permite ejecutarlo directamente desde línea de comandos, sin necesidad de llamar explícitamente al intérprete. Esta línea, llamada "shebang", suele ser `#!/usr/bin/python` o `#!/usr/bin/env python` (esta última más genérica). El fichero quedaría algo así:

`#!/usr/bin/python

print "Hola, mundo libre"`

(Nótese la línea en blanco). Para hacerlo ejecutable se sigue también el procedimiento habitual en Linux:

`chmod +x hola.py`

con lo que posteriormente ya se puede ejecutar también de la forma habitual:

`bash% ./hola.py`

Los **"./"** puede que no sean necesarios si se tiene el propio directorio incluido en el camino de ejecución, pero no suele ser una práctica habitual (ni segura) así que es mejor curarse en salud haciendo de la forma anterior. El resultado, de todas formas, tiene que ser el mismo.
