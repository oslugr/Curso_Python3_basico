## TEOREMA DE LA PROGRAMACIÓN ESTRUCTURADA

El teorema de la programación estructurada afirma (y demuestra) que toda función computable puede codificarse usando sólo combinaciones de tres tipos de estructuras básicas:

### SECUENCIA:

Se ejecuta una orden y despues otra, secuencialmente, en lo que viene a ser el flujo "natural" de un programa.

### CONDICIONAL:

Se ejecuta una de dos órdenes, dependiendo de un valor lógico boolenao ("cierto" o "falso"). Naturalmente, esto puede combinarse para multiplicar las diversas opciones, y unirse a lo anterior para elegir entre bloques completos de código.

### BUCLE:

Se ejecuta una orden mientras una condición sea cierta. O (lo que viene a ser lo mismo) se ejecuta hasta que deje de serlo.

Cualquier otra estructura (como, por ejemplo y sobre todo, el famoso -e infame- GOTO) es prescindible o sustituible por las anteriores y, en general, sólo contribuye a dificultar la legibilidad del código.

Respecto a esto último, el polémico y genial Edsger Dijkstra dijo del lenguaje BASIC y su uso extensivo de la sentencia GOTO que "[...] la enseñanza de BASIC debería ser considerada un delito penal: Mutila la mente más allá de toda recuperación".
