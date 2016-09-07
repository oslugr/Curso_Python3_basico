## LA SENTENCIA CLASS

La sentencia **class** es el modo habitual de crear un objeto de clase. **class** es una sentencia compuesta de cláusula única, con la sintaxis:
```python
class nombre_clase():
atributos
métodos
```
El cuerpo de la clase es donde especificamos por lo general los atributos de la clase; estos atributos pueden ser objetos (incluyendo las funciones) u objetos de datos normales: entero, cadena, lista, tupla...

Para declarar datos normales, escribimos el identificador del dato y su correspondiente valor, por ejemplo:
```python
class c1():

x= 25
```
En el caso de los métodos es necesario el uso de la sentencia def:
```python
class c1():

x=25

def doble(self):

return x * 2
```
En el ejemplo final, aparece un método especial \__init__ se le conoce en el ámbito de la [programación orientada a objetos](https://es.wikipedia.org/wiki/Programaci%C3%B3n_orientada_a_objetos) como el constructor de la clase.

[Ejemplo de declaración y uso de una clase sencilla](https://gist.github.com/psicobyte/dd5625426b4747319970#file-clase-py).
```python
#!/usr/bin/python
#coding: utf-8

# Ejemplo de clase.

class Acuario():

    #El método __init__ se ejecuta automáticamente al llamar a la clase
    def __init__(self, litros, tipo, num):
        self.capacidad = litros
        self.tipo = tipo
        self.total_peces = num

    def meter_pez(self):
        self.total_peces = self.total_peces + 1

    def sacar_pez(self):
        if ( self.total_peces > 0):
            self.total_peces = self.total_peces + 1

Mipecera= Acuario(100,"tropical",5)

print "La pecera tiene", Mipecera.capacidad, "litros"
print "Hay", Mipecera.total_peces, "peces"

print "Añadimos un pez"

Mipecera.meter_pez()

print "Ahora hay", Mipecera.total_peces, "peces"
```