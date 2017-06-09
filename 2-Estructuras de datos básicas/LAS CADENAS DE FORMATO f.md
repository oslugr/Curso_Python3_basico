Desde, o partir de Python3.6, las cadenas f proporcionan de manera sencilla el integrar variables y expresiones dentro
de una cadena con una reducida sintaxis.
 
 Las cadenas f nos ofrecen una forma concisa de construir cadenas formateadas de fácil lectura. Pero no sustiutye ni elimina 
 las opciones de formateo de cadenas que ya existían.
 
 Ejemplos del nuevo metodo de formateo de cadenas, conociendo así las ventajas que aporta:
 
 ```python
 # Una cadena f se presenta como un literal
 # entrecomillado precediendole el caracter "f" o "F"
 
 f'cadena'
 
# El resultado de evaluar una cadena "f" se puede 
# asignar a una variable:

cadenaf = f'cadena'

# También, se puede extender a varias líneas utilizando
# las triples comillas:

cadenaf = f'''línea1
línea2
línea3'''

# Dentro de una cadena "f" se pueden insertar
# variables y expresiones escribiéndolas entre
# llaves {}:

modelo = 'Orbea Alma'
precio = 650
impuestos = precio * 21/100
print(f'Bicicleta {modelo}: {precio+impuestos} euros')
# Bicicleta Orbea Alma: 786.5 euros

# Las dobles llaves se utilizan para expresar el
# nombre de una variable o mostrar literalmente una
# expresión y no el valor resultante de su evaluación:

nombre = 'Claudia'
cadena = f'La variable {{nombre}} contiene {nombre}'
print(cadena)  
# La variable {nombre} contiene Claudia

# Para concatenar o unir cadenas de textos con 
# cadenas "f" se utiliza el espacio o el signo '+'.
# Los espacios en blanco dentro de una expresión
# son ignorados:

arbol = 'secuoya'
alt = 115
print(f'Una {arbol}' ' mide ' f'{alt} metros')
# La secuoya mide hasta 115 metros

print(f'Una { arbol }' + ' mide ' + f'{ alt } metros')
# La secuoya mide hasta 115 metros

# En la declaración de una cadena el carácter "f" 
# se puede combinar con el carácter "r" de las
# cadenas row (crudas) para que no se interpreten
# las secuencias de escape (caracteres especiales 
# precedidos de la barra invertida "\"):
# "\n" (salto de línea), "\t" (tabulador), etc. 
# Sin embargo, "f" no se puede combinar con "b" o
# "u" que se utilizan para representar cadenas de
# Bytes o caracteres Unicode, respectivamente:

cadenacruda = fr'la línea finaliza con \n'
print(cadenacruda)  # la línea finaliza con \n

# Las secuencias de escape no se pueden incluir
# en una expresión:

print(f'Esta cadena genera un {\"error\"}')
print(f'Esta cadena no genera un {"error"}')

# Después de cada expresión se puede indicar un
# especificador para establecer algún tipo de
# conversión. Las conversiones permitidas se expresan
# con '!s' , '!r' y '!a' que son equivalentes a las
# funciones str(), repr() y ascii(), respectivamente:

novela = 'En busca del unicornio'
cadena = f'La novela se llama {novela!r}'
print(cadena) 

# La novela se llama 'En busca del unicornio'

# Los especificadores de formato permiten fijar 
# el espacio reservado para la parte entera de 
# una expresión numérica y su precisión decimal:

ancho = 10
precision = 5
numpi = 3.14159265358979323846
print(f"Número PI: {numpi:{ancho}.{precision}}")
# Número PI:     3.1416

# Los especificadores que se utilizan para
# formatear fechas y horas se pueden utilizar
# en una cadena "f":

from datetime import datetime
fecha = datetime.now()
print(f'El partido de tenis se jugará el día {fecha:%d}')
# El partido de tenis se jugará el día 10

# Una expresión de una cadena "f" puede incluir
# llamadas a funciones:

def suma(a,b):
    return a+b
    
a = 10
b = a * 12  
rtdo = f'La suma total es {suma(a,b)}'
print(rtdo)  # La suma total es 130

# ...Y la función Lambda es una función más:

b = 10
h = 5
print(f'Área triángulo: {(lambda b,h: b*h/2)(b,h)}')
# Área triángulo: 25.0

# Con las cadenas "f" la alineación y el rellenado
# se expresa de manera más simple:

blog = 'Python para impacientes'
print(f'{blog:_^30}')  # ___Python para impacientes____
print(f'{blog:_<30}')  # Python para impacientes_______ 
print(f'{blog:_>30}')  # _______Python para impacientes

# Dentro de una cadena "f" cuando se evalúa una 
# expresión el valor obtenido se convierte de forma
# automática a cadena de texto (str) para facilitar
# su inserción:

import time
v1 = 10  # Número entero
v2 = 12.34  # Número con decimales (float)
v3 = 'abc'  # Cadena de texto
v4 = 0xF  # Número hexadecimal
v5 = time.localtime().tm_hour  # Horas
v6 = time.localtime().tm_min  # Minutos
v7 = True  # Valor booleano
v8 = (1, 2, 3)  # Tupla
v9 = {'x':0, 'y':0}  # Diccionario
print(f'{v1+v2} {v3} {v4} {v5}:{v6} {v7} {v8} {v9}')
# 22.34 abc 15 11:31 True (1, 2, 3) {'x': 0, 'y': 0}

# Por último, comentar un detalle importante: las 
# expresiones de una cadena "f" se evalúan de 
# izquierda a derecha:

# Reloj binario de dos dígitos
def cuenta(cnts):
    if cnts[0]==1 and cnts[1]==1:
        cnts[0]=0
        cnts[1]=0    
    elif cnts[1] < 1:
        cnts[1]+=1
    elif cnts[0] < 1:
        cnts[0]+=1
        cnts[1]=0
    else:
        cnts[0]=1
        cnts[1]=1
    return cnts

cnts = [0, 0]
print('Reloj binario:')
print(f'{cnts}, {cuenta(cnts)},')
print(f'{cuenta(cnts)}, {cuenta(cnts)},')
print(f'{cuenta(cnts)}, {cuenta(cnts)}...')

# Reloj binario:
# [0, 0], [0, 1],
# [1, 0], [1, 1],
# [0, 0], [0, 1]...

``` 
