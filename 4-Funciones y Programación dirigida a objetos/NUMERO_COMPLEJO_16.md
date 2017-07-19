## NÚMERO COMPLEJO

```python
#!/usr/bin/pyhton3

class Complejo:

	def __init__(self, parteReal, parteImaginaria):
		"""Constructor de la clase Complejo"""
		self.r = parteReal
		self.i = parteImaginaria
		
	def getReal(self):
		return self.r
		
	def getImag(self):
		return self.i
		
num = Complejo(3.0, -4.5)
print ("Parte Real ", num.getReal())
print ("Parte Imaginaria ", num.getImag())
```