## PyRencia

Otra característica que tiene que tener un lenguaje para considerarse orientado a objetos es la HERENCIA.

La herencia significa que se pueden crear nuevas clases partiendo de clases existentes, que tendrá todas los atributos y los métodos de su 'superclase' o 'clase padre' y además se le podrán añadir otros atributos y métodos propios.

En Python, a diferencia de otros lenguajes orientados a objetos (Java, C#), una clase puede derivar de varias clases, es decir, Python permite la herencia múltiple.

### Superclase

Clase de la que desciende o deriva una clase. Las clases hijas (descendientes) heredan (incorporan) automáticamente los atributos y métodos de la la clase padre.

### Subclase

Clase descendiente de otra. Hereda automáticamente los atributos y métodos de su superclase. Es una especialización de otra clase. Admiten la definición de nuevos atributos y métodos para aumentar la especialización de la clase.
 
[Ejemplo](https://gist.github.com/psicobyte/49cda1572b40bcfbefda#file-herencia-py):
```python
#!/usr/bin/python
#coding: utf-8

# Ejemplo de herencia.

class Mamifero():
    def __init__(self):
        descrpcion= "Los mamíferos son interesantes"

    def tiene_pelo(self):
        return "si"

# Al poner Mamifero en el paréntesis, le decimos que herede de esa calse
class Gato(Mamifero):
    def __init__(self):
        descrpcion= "Los gatos molan"

    def maulla(self):
        return "si"

# Mascota es una instancia de la clase Gato
Mascota = Gato()

# Estamos llamando a un método que, en realidad, pertenece a la clase mamífero
print Mascota.tiene_pelo()
```