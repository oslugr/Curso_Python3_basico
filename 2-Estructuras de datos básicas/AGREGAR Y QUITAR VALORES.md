## Agregar y quitar valores

### Metiendo Datos

La instrucción básica para añadir elementos a una lista es append(), que agrega un nuevo elemento al final de esta.

Su uso sería:

`MiLista.append(NUevoElemento)`

Donde **NUevoElemento** es lo que queremos agregar a la lista **MiLista**.

Este tipo de notación, con un elemento seguido de un punto y la función a aplicarle, es propia de los objetos y se verá con algo más de detalle en temas siguientes.

Como nota, para ir abriendo boca, agregaremos que en Python todo dato, función, estructura, etc, puede ser manipulado como un objeto.

También se puede introducir un dato "en medio" de la lista, usando insert() del siguiente modo:

`MiLista.insert(Posicion,NuevoElemento)` 

Donde **Posicion** es el número de posición donde se insertará, y **NuevoElemento** el elemento introducido.

Es importante recordar que el nuevo elemento no reemplaza el contenido anterior, si no que el dato que anteriormente hubiera en esa posición se desplazará un paso más adelante.

### Sacando Datos

La forma más simple de eliminar datos de una lista es por medio de la función pop().

Esta función es muy útil, porque elimina el último elemento de una lista y lo retorna. De modo que se puede usar del siguiente modo:

`ValorExtraido= MiLista.pop()` 

Esto eliminaría el último elemento de **MiLista** y lo asignaría a la variable **ValorExtraido**.

Intuitivamente, puede verse que el manejo básico de una lista como buffer es a base de append() y pop().
