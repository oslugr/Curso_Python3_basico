## PyMorfeando

Es muy simple, el polimorfismo viene a significar que puedes tener dos (o más) métodos con el mismo nombre para diferentes clases. Estos métodos pueden comportarse de diferente manera dependiendo de la clase en que se apliquen.

Por ejemplo, para practicar la geometría decides escribir un programa que calcule el área de diferentes figuras, como triángulos o rectángulos.

Para el ejemplo se crean dos clases y las dos tienen el mismo método *getArea()* pero se implementa de forma diferente para cada clase. Esto es polimorfismo.
```python

!#/usr/bin/env python
# -*- coding: utf-8 -*-
 
class Triangulo:
    def __init__(self, ancho, alto):
        self.ancho = ancho
        self.alto = alto
     
    def getArea(self):
        area = self.ancho * self.alto / 2.0
        return area
        
class Rectangulo:
    def __init__(self, lado):
        self.lado = lado
        
    def getArea(self):
        area =self.lado * self.lado
        return area
        
miTriangulo = Triangulo(3,6)
miRectangulo = Rectangulo(5)
 
print miTriangulo.getArea()
print miRectangulo.getArea()
```
