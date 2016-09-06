## ARRAYS ASOCIATIVOS

### ARRAYS ASOCIATIVOS O MAPAS

Los diccionarios, también llamados matrices asociativas, deben su nombre a que son colecciones que relacionan una clave y un valor.

El primer valor se trata de la clave y el segundo del valor asociado a la clave. Como clave podemos utilizar cualquier valor inmutable: podríamos usar números, cadenas, booleanos, tuplas, … pero no listas o diccionarios, dado que son mutables.

Esto es así porque los diccionarios se implementan como tablas hash, y a la hora de introducir un nuevo par clave-valor en el diccionario se calcula el hash de la clave para después poder encontrar la entrada correspondiente rápidamente.

Si se modificara el objeto clave después de haber sido introducido en el diccionario, evidentemente, su hash también cambiaría y no podría ser encontrado.

La diferencia principal entre los diccionarios y las listas o las tuplas es que a los valores almacenados en un diccionario se les accede no por su índice, porque de hecho no tienen orden, sino por su clave, utilizando de nuevo el operador **[]**.
Por ejemplo:
```python
mydict = {"altura" : "media", "habilidad" : "alta", "salario" : 999} print mydict {"altura" : "media", "habilidad" : "alta", 
"salario" : 999} print mydict ["habilidad"] alta 
```
También podemos comprobar la existencia de una clave en un diccionario usando has_key:
```python
if mydict.has_key ('altura'):

print 'Nodo encontrado'

También podríamos hacer :

if 'altura' in mydict:

print 'Nodo encontrado'
```
