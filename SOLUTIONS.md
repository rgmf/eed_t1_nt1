# Instrucciones
En este documento, en formato Markdown, tienes una serie de cuestiones a las que tienes que responder.

En todas ellas puedes leer la pregunta y verás, al final, un apartado llamado **Respuesta** en la que tendrás que escribir tu respuesta.

# Pregunta 1
Imagina que tienes un repositorio inicializado en una carpeta y al ejecutar el comando `git status` ves la siguiente información:

```
En la rama main

No hay commits todavía

Archivos sin seguimiento:
  (usa "git add <archivo>..." para incluirlo a lo que será confirmado)
	fic1.txt
	fic2.txt
	fic3.txt

no hay nada agregado al commit pero hay archivos sin seguimiento presentes (usa "git add" para hacerles seguimiento)
```

Explica el estado en el que está el repositorio.

**Respuesta**:
Se tienen tres ficheros que son `fic1.txt`, `fic2.txt` y `fic3.txt` que han sido creados pero que no están en Git. Por ese motivo, nos indica que son archivos sin seguimiento.

# Pregunta 2
Ahora, tras ejecutar el comando `git status` nos encontramos con esta información:

```
En la rama main

No hay commits todavía

Cambios a ser confirmados:
  (usa "git rm --cached <archivo>..." para sacar del área de stage)
	nuevos archivos: fic1.txt
	nuevos archivos: fic2.txt

Archivos sin seguimiento:
  (usa "git add <archivo>..." para incluirlo a lo que será confirmado)
	fic3.txt
```

Explica el estado en el que está el repositorio.

**Tu respuesta**:
El fichero `fic3.txt` es un fichero que está en el directorio de trabajo pero no está en Git. Y los ficheros `fic1.txt` y `fic2.txt` se han metido en el área de preparación o *stage* para el siguinete *commit*.

# Pregunta 3
Ha cambiado el estado del repositorio, al ejecutar `git status` vemos la siguiente información:

```
En la rama main
Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
	modificados:     fic1.txt
	modificados:     fic2.txt

Archivos sin seguimiento:
  (usa "git add <archivo>..." para incluirlo a lo que será confirmado)
	fic3.txt

sin cambios agregados al commit (usa "git add" y/o "git commit -a")
```

Explica el estado en el que está el repositorio indicando qué ficheros están en Git y qué otros no lo están.

**Tu respuesta**:
El fichero `fic3.txt` es un fichero que está en el directorio de trabajo pero no está en Git. Y los ficheros `fic1.txt` y `fic2.txt` han sido modificados y, por tanto, el contenido de ellos en Git es diferente al que se tiene en el directorio de trabajo.

# Pregunta 4
¿Qué comando de Git usarías para ver qué commits hay y quién los ha hecho?

**Tu respuesta**:
`git log`

# Pregunta 5
Escribe el nombre y apellidos de todas las personas que han colaborado en este repositorio.

**Tu respuesta**:
Han participado en el repositorio:
- Román Martínez
- Mona Lisa
- Repo Sitorio

# Pregunta 6
Indica, por cada commit, qué ficheros se han modificado (bien sea porque se han crado, modificado o borrado):

**Tu respuesta**:
- commit 1651176038c39964d9f391a4456bb5b90471f29c
  - AUTHORS: se ha insertado 1 línea
  - LICENSE: se ha insertado 1 línea
  - RADME.md: se han insertado 2 líneas
  
- commit 0228b695bcaa189e6367ab9e28bdf764222bffa9
  - src/hello.c: se han insertado 7 líneas
  - src/hello.py: se ha insertado 1 línea
  
- commit 4e4d5c928a641b218da43b2b1eb37c6ac77e1bdb
  - src/hello.py: se han insertado 5 líneas

- commit aee0d6c57273e97b58b992c781ab34a748052794
  - AUTHORS: se ha insertado 1 línea
  - tests/test_hello.py: se han insertado 3 líneas
  
- Hay un último commit en el que se han añadido los ficheros QUESTIONS.md y SOLUTIONS.md

# Pregunta 7
Crea, dentro de una carpeta llamada `docs`, los siguientes ficheros:

- `python.txt` y escribe en este fichero qué es Python en una línea
- `c.txt` y escribe en este fichero qué es C en una línea

Tras estos cambios, prepara un commit con un mensaje adecuado en el que se añadan estos dos nuevos ficheros.

¿Qué comandos Git has ejecutado?

**Tu respuesta**:
`git add docs/python.txt docs/c.txt`
`git commit -m "Dos nuevos ficheros dentro de docs."`
