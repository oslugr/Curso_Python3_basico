## Introducción y advertencia

Python es un lenguaje interpretado, y como tal, lo que se instala es una aplicación que necesitarás cargar cada vez que quieras ejecutar un programa en tal lenguaje. No es un entorno de programación; es decir, no es un entorno completo que te permita editar, ejecutar, depurar el programa y demás. Para eso existen diferentes opciones que veremos más adelante.

Con esto lo que quiero decir es que, una vez instalado, al pinchar en el icono que diga "Python" no va a hacer nada salvo sacar una línea de órdenes (dependiendo del sistema operativo); sí se ejecutará el intérprete automáticamente cuando se pulse el ratón sobre un programa escrito en Python (con la extensión .py), pero lo más probable es que, tratándose de programas que se ejecutan en el intérprete de órdenes, no se vea nada. Concluyendo: una vez instalado no te lances a ejecutar nada, espera a escribir tu primer programa en Python y entonces comprobarás si funciona todo correctamente (que debería hacerlo).

## ¿Qué versión debería instalar?

En la [página de descarga de Python](https://www.python.org/downloads/) hay dos versiones principales: la 2.7 y la 3.1. Este curso está hecho principalmente con la 2.6, así que la que más se le acerca es la 2.7. Puedes instalar cualquiera de ellas, o las dos, pero aconsejamos para evitar diferencias que se instale la 2.7. En todo caso, actualmente es la versión más usada.

Otra opción que te puedes instalar en un dispositivo portátil para usar en diferentes ordenadores es la [Portable Python](http://portablepython.com/). En este caso las versiones disponibles están basadas en la 2.6 o 3.0; aconsejamos que se instale la primera.

[](/Curso_Python_basico/blob/master/img/python-windows-menui.png)

## ¿Cómo instalo Python en mi ordenador?

Si usas Linux ya sabes como hacerlo; usa tu programa favorito para descargártelo de los repositorios e instalarlo; es posible, de todas formas, que ya esté instalado en la distribución base; Ubuntu, Fedora, Guadalinex y otras ya lo incluyen por ser el lenguaje con el que se escriben muchas de las aplicaciones base que llevan. Para ver si está instalado abre un intérprete de órdenes (que también es posible que sepas como hacer, pero si no `Aplicaciones -> Accesorios -> Terminal`) y escribe `python --version` que debería devolver algo así `Python 2.6.5` Si no es así, tendrás que instalarlo.

En Windows o Macintosh hay que [descargar alguna de las opciones que se presentan en la página de descargas](https://www.python.org/downloads/), teniendo en cuenta las observaciones hechas anteriormente.

En Windows se sigue el proceso habitual en las instalaciones: ir haciendo click sobre "Next" hasta que se indique que se ha instalado. El sistema operativo te hará diferentes advertencias sobre que estás instalando un programa, a las que contestarás que sí, que por supuesto, que faltaría más. Si contestas que no, no te lo va a instalar, así que tendrás que contestar que sí.

Os mostramos a continuación un screencast sobre la instalación en Ms Windows:

<iframe width="560" height="315" src="https://www.youtube.com/embed/Q4prb42X7N8" frameborder="0" allowfullscreen></iframe>

Lo que instalarás en Windows será un intérprete de línea de comandos, que aparecerá en el menú como se muestra en la ilustración adjunta, con el texto Python (command line); es decir, Python (línea de órdenes). 

[!](/oslugr/Curso_Python_basico/blob/master/img/python-ventana-windows.png)

El resultado de la ejecución aparece arriba. Desde ahí se pueden ejecutar directamente órdenes en Python, como veremos más adelante. También se instala un fichero de ayuda al que se puede acceder desde el menú -> Todos los programas -> Python 2.7 -> Python Manuals (o Manuales de Python).

El paquete indicado anteriormente instala también un mini-entorno de desarrollo llamado IDLE, que se puede ejecutar desde el menú anterior eligiendo IDLE. Es un pequeño envoltorio de la línea de comandos, pero te permite cargar ficheros y salvarlos, al menos. Aunque no permite editar programas, sí permite probar órdenes y tiene alguna facilidad adicional como la expansión del nombre de las órdenes (pulsando tabulador). Se puede usar para hacer pruebas, o cuando se conozca más el lenguaje, depurar programas.

En cuanto a otras plataformas, [este wikilibro describe como hacerlo en un Mac](https://es.wikibooks.org/wiki/Python/Instalaci%C3%B3n_de_Python/Python_en_Mac_OS_X); lo más probable es que esté ya instalado (y que la versión sea la correcta), pero si no, puedes instalártelo desde la página de descargas indicada anteriormente.

Finalmente, y como curiosidad, [puedes instalártelo dentro del "Android Scripting Environment" en tu teléfono Android](http://www.xatakamovil.com/aplicaciones/android-scripting-environment-programa-con-scripts), tal como los HTC que tan célebres se han hecho últimamente. Así puedes hacer los ejercicios que te planteemos en cualquier lugar, incluso en el bus.

## Otros programas

Como se ha dicho más arriba, la instalación de Python proporciona sólo el intérprete que permite ejecutar los programas escritos en él; pero para escribir estos programas hará falta un editor. Todos los sistemas operativos tienen un editor de textos básico, pero se es más productivo usando editores de textos específicos de programadores. En Linux se puede usar emacs, vi, kate, Geany o cualquiera de los múltiples programas que existen, en el Mac hay también buenas opciones.

En Windows se puede descargar [Geany de su página web](http://www.geany.org/Download/Releases), e instalarse con las opciones básicas. Al final de la instalación te ofrece la posibilidad de ejecutarlo.

La ventaja que tiene este tipo de programa es que te colorea las palabras clave y te detecta algunos errores de sintaxis básicos, permitiendo que uno sea más productivo.

Para usuarios de entornos de desarrollo tales como NetBeans o Eclipse, hay un plugin denominado PyDev que se puede instalar para editar este tipo de programas. Se puede instalar desde el menú correspondiente, o descargándoselo de la [página correspondiente](http://pydev.sourceforge.net/). En [esta página instruyen sobre cómo instalárselo en Eclipse, por ejemplo](http://www.pythondiario.com/2013/06/eclipse-y-pydev-configuracion-del-ide.html).
