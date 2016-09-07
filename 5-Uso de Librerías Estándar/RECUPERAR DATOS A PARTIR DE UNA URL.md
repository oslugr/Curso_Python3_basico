## RECUPERAR DATOS A PARTIR DE UNA URL

El módulo *urllib2* puede leer datos de una URL usando varios protocolos como HTTP, HTTPS, FTP o Gopher.

En el siguiente apartado aparece un ejemplo, en el que obtenemos el código html de un web.
```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

import urllib2

response = urllib2.urlopen('http://www.ugr.es/')
html = response.read()

print html
```

Veamos unos ejemplo ilustrativos sobre el uso de esta librería. ¿Está disponible en la web de gomiso el episodio 23 de la seria The big bang theory?, ¿La web de google contiene alguna imagen?, ¿Cuáles son los 10 primeros caracteres de python.org?

Una vez que recuperamos el código html a partir de una url, podemos obtener una respuesta rápida a estas preguntas, por ejemplo, mediante el uso de métodos para el tratamiento de cadenas. Observa el siguiente bloque de código.
```python
import urllib2

def search(url, cad):
    """Busca la cadena cad del código html que contiene url"""
    source = urllib2.urlopen(url).read()
    if source.find(cad) != -1:
        print "% aparece en la web %s" % (cad,url)
    else:
        print "%s No aparece en la web %s" % (cad,url)
            
if __name__ == '__main__':
    search('http://www.google.es','google')
```
El método *search* recupera el código html de la web indicada en el parámetro url. En segundo lugar comprueba si la variable source contiene la cadena cad, que se pasa como parámetro a la función. Por ultimo imprime un mensaje indicando el resultado de la búsqueda.

Para responder a la pregunta sobre una imagen en la web, simplemente la cadena a buscar sería el tag html para imágenes. En este caso en concreto sería *img*.