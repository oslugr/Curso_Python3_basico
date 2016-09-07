## ORDEN DE ARGUMENTOS

Los argumentos opcionales solo pueden ir al final ya que se acomodan de izquierda a derecha.
Observa el error que se produce si cambiamos el parametro por defecto de orden.

Presta atención al error que ocurrira con el argumento tasa, cuando esta fuera de su lugar.
```python
def funcion(tasa = 0.15, valor):

    print tasa, valor

File "<stdin>", line 1

SyntaxError: non-default argument follows default argument
```