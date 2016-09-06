## POR QUÉ USAR RAW_INPUT

Al usar input en lugar de raw_input, el tratamiento de datos se hace más cómodo, porque el propio intérprete se ocupa de averiguar qué es una cadena, qué es un entero, etc.

Pero la entrada de datos por parte del usuario se hace más incómoda, porque las cadenas de texto deben estar entrecomilladas para que Python sepa que lo son.

Si se introduce sin comillas, el intérprete creerá que es el nombre de una variable.

Esto, a su vez, plantea un problema de seguridad. Por ejemplo, en el siguiente código:
```python
#!/usr/bin/python 
#coding: utf-8 
clave= "secreto" 
entrada= input('Introduce la clave ') 
if entrada == clave: 
print "acertaste, la clave es ", entrada, ". " 
else: 
print "acceso no autorizado" 
```
Si, en la entrada, escribimos "clave" (sin las comillas), Python lo interpreta como el nombre de una variable, por lo que lo reemplaza con el contenido de la variable de ese nombre y, por tanto, lo da por bueno independientemente de cuál sea el valor de la clave realmente.

Es un ejemplo bastante simple, pero muestra claramente el peligro de permitir el acceso directo a las variables del programa.

Para eso se usa raw_input, que funciona igual que input pero asume, automáticamente, que toda entrada es una cadena.
