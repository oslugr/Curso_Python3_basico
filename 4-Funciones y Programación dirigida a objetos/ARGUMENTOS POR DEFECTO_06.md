## ARGUMENTOS POR DEFECTO

```python
#!/usr/bin/python3

# Nota que, en el valor que recibe la función, tiene 'cancion="lalala"'
# Canción es la variable, como siempre, y "lalala" es lo que se le asignará por defecto si no se le pasa ningún valor
def canta(cancion="lalala"):

    if cancion == "lalala":
        print ("Laaa, lala laaa,  lala laaa,  lala laaaaaaa...")
    elif cancion == "himno":
        print ("Naaana, naaana, nanana nana nana na na NA na NA...")
    elif cancion == "daisy":
        print ("Lo siento Dave, me temo que no puedo hacer eso.")
    else:
        print ("Esa no me la sé")

#Asignándole un valor hace lo previsible.
print ("Pasando \"daisy\" nos responde:")
canta("daisy")

# pero, si no le asignamos ningún valor, toma el que tiene por defecto en la función
print ("Pero, si no pasamos nada, dice:")
canta()
```
[ValorPorDefecto](https://gist.github.com/psicobyte/a26ea4ca7f77a7239d51#file-valorpordefecto) hosted with ❤ by [Gist](https://gist.github.com/)