## EJEMPLO COMBINADO

Vamos a ver un pequeño caso real de cómo se usan algunos de los elementos viastos hasta ahora.

Estudia atentamente el siguiente ejemplo de código (basado en un ejemplo oficial de `Python`).

Se trata de un programa que explora los primeros 100 números naturales y examina cada uno de ellos para ver si es primo o no. En el caso de que sea primo, lo indica, y si no lo es muestra dos de sus divisores (los primeros que ha encontrado).

```python
#!/usr/bin/python3
for numero in range(2,100):
    for divisor in range(2,numero):
    	if numero % divisor == 0:
        	print (numero, 'es múltiplo de', divisor, 'y', numero/divisor)
        	break
    else:
	    print (numero, 'es un número primo')
```
[Números primos](https://gist.github.com/psicobyte/6179816#file-numeros-primos) hosted with ❤ by [GitHub](https://github.com/)


Fíjate bien en la indentación (sobre todo la de ese "else" ¿corresponde a uno de los "for" o al "if"?) y en cómo se usan unas estructuras de control dentro de otras.
