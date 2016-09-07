## DOCUMENTACIÓN

En Python, la documentación de una función se escribe tras la definición, como la primera cadena literal del bloque (si es que hay una).
Por lo general se utilizan cadenas largas (admiten saltos de lineas),
que se delimitan por triples comillas simples o dobles. La herramienta
pydoc o epydoc, entre otras, (similares a javadoc) permiten generar salida en HTML, PDF, LATEX, groff, etc. El marcado es similar a javadoc, por ejemplo:

* @param <nombre_param\> especifica un parámetro.
* @returns hace referencia a lo que retorna la función.
* @precondition se utiliza para definir una precondición.
* @postcondition se utiliza para definir una postcondición.