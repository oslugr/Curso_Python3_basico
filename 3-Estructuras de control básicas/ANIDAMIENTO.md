## ANIDAMIENTO

Las instrucciones pueden "anidarse". Es decir, pueden incluirse unas dentro de otras para hacer dependiente su ejecución.

En otros lenguajes de programación es habitual anidar las sentencias por medio de símbolos como:
```python
Instruccion_Principal {
    instruccion_anidada
}
instruccion_independiente
```
[Anidamiento en otros lenguajes](https://gist.github.com/psicobyte/6163945#file-anidamiento-en-otros-lenguajes) hosted with ❤ by [GitHub](https://github.com/)

En Python, el anidamiento de instrucciones no se hace con llaves ni otros símbolos contenedores, sino por medio de la indentación. las instrucciones con un nivel de indentación (digamos que un tabulador, ver más abajo) estań contenidas en las que no están indentadas que les preceden, las instrucciones con dos tabuladores están incluidas en las anteriores, etc.
```python
Instruccion_Principal:
    instruccion_anidada
instruccion_independiente
```
[Anidamiento en Python](https://gist.github.com/psicobyte/6163957#file-anidamiento-en-python) hosted with ❤ by [GitHub](https://github.com/)

Se recomienda encarecidamente que no se use realmente el carácter tabulador **(ASCII 09)** para indentar, si no que se usen espacios. Lo recomendable, según Guido van Rossum, son cuatro espacios por cada nivel de indentación (Sin embargo, Linus Torvalds considera cualquier tabulación de menos de 8 caracteres como una herejía). Nunca mezcles indentados por espacios e indentados por tabulador.
