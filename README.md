# `mpss` - Modelos Probabilísticos de Señales y Sistemas

Estos son los archivos ejecutables tipo "notebook" de Jupyter, que llamaremos **PyX**, y que acompañan los subtemas del curso. Son una introducción a Python como lenguaje de programación y la presentación de algunas de sus herramientas más importantes para utilizar en problemas relacionados con la probabilidad, la estadística y el manejo de datos.

## Lista de tutoriales

Estos son los temas que son o serán cubiertos por cada archivo (*trabajo en progreso*).

| Nombre | Tema |
| ------ | ---- |
| `Py0`  | Introducción a Python    |
| `Py1`  | Funciones y librerías estándar de Python |
| `Py2`  | Librerías de computación científica  |
| `Py3`  | Librerías de manipulación de datos I |
| `Py4`  | Introducción al módulo de funciones estadísticas |
| `Py5`  | Curvas de ajuste de datos |
| `Py6`  | Módulo de estadística para cálculo de momentos |
| `Py7`  | Graficación avanzada     |
| `Py8`  | Simulaciones aleatorias  |
| `Py9`  | Documentación de código |
| `Py10` | Librerías de manipulación de datos II  |
| `Py11` | Programación orientada a objetos I  |
| `Py12` | Programación orientada a objetos II  |
| `Py13` | Programación orientada a objetos III |
| `Py14` | Formatos de intercambio de datos  |
| `Py15` | Conexión con bases de datos externas  |
| `Py16` | Módulo de análisis espectral  |
| `Py17` | Interfaces gráficas de usuario de Python  |
| `Py18` | Graficación avanzada HTML  |
| `Py19` | TBD  |
| `Py20` | TBD  |

## Algunos consejos de la *Guía de estilo para código de Python* (PEP 8)

Nadie menos que Guido van Rossum (creador de Python) y otras personas, crearon una guía para que el código escrito en Python tenga una consistencia agradable a la vista. Pueden hacer lectura completa en la página oficial de [PEP 8](https://www.python.org/dev/peps/pep-0008/).

Aquí mostraremos solamente la síntesis de unas cuantas recomendaciones que serán **regla** para el curso.

### Cosas que fastidian (*pet peeves*)

Hay que evitar espacios en blanco superfluos en las siguientes situaciones:

* En medio de paréntesis redondos o cuadrados, o llaves.

*Correcto*
```python
spam(ham[1], {eggs: 2})
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* Entre una coma final y un paréntesis cerrado siguiente:

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
bar = (0, )
```

* Inmediatamente antes de una coma, punto y coma o dos puntos:

*Correcto*
```python
if x == 4: print x, y; x, y = y, x
```
**Incorrecto**
```
if x == 4 : print x , y ; x , y = y , x
```

* Sin embargo, en un segmento, el colon actúa como un operador binario y debe tener cantidades iguales en ambos lados (tratándolo como el operador con la prioridad más baja). En un corte extendido, ambos dos puntos deben tener la misma cantidad de espacio aplicado. Excepción: cuando se omite un parámetro de segmento, se omite el espacio:

*Correcto*
```python
ham[1:9], ham[1:9:3], ham[:9:3], ham[1::3], ham[1:9:]
ham[lower:upper], ham[lower:upper:], ham[lower::step]
ham[lower+offset : upper+offset]
ham[: upper_fn(x) : step_fn(x)], ham[:: step_fn(x)]
ham[lower + offset : upper + offset]
```
**Incorrecto**
```
ham[lower + offset:upper + offset]
ham[1: 9], ham[1 :9], ham[1:9 :3]
ham[lower : : upper]
ham[ : upper]
```

* Inmediatamente antes del paréntesis abierto que inicia la lista de argumentos de una llamada de función:

*Correcto*
```python
spam(1)
```
**Incorrecto**
```
spam (1)
```

* Inmediatamente antes del paréntesis abierto que comienza una indexación o corte:

*Correcto*
```python
dct['key'] = lst[index]
```
**Incorrecto**
```
dct ['key'] = lst [index]
```

* Más de un espacio alrededor de un operador de asignación (u otro) para alinearlo con otro:

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

#### Otras recomendaciones

* Evite dejar espacios en blanco en cualquier lugar. Debido a que generalmente es invisible, puede ser confuso: por ejemplo, una barra invertida seguida de un espacio y una nueva línea no cuentan como un marcador de continuación de línea. Algunos editores no lo conservan y muchos proyectos (como el propio CPython) tienen ganchos de confirmación previa que lo rechazan.

* Siempre rodear estos operadores binarios con un solo espacio a cada lado: asignación ( = ), la asignación aumentada ( + = , - = , etc.), las comparaciones ( == , < , > , ! = , <> , <= , > = , in , not in , is , is not ), Booleans ( and , or , not ).

* Si se utilizan operadores con diferentes prioridades, considere agregar espacios en blanco alrededor de los operadores con las prioridades más bajas. Usa tu propio juicio; sin embargo, nunca use más de un espacio y siempre tenga la misma cantidad de espacios en blanco en ambos lados de un operador binario:

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* Las anotaciones de funciones deben usar las reglas normales para los dos puntos y siempre tener espacios alrededor de la flecha -> si está presente. (Consulte las anotaciones de funciones a continuación para obtener más información sobre las anotaciones de funciones):

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* No use espacios alrededor del signo = cuando se usa para indicar un argumento de palabra clave, o cuando se usa para indicar un valor predeterminado para un parámetro de función no anotado:

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* Sin embargo, cuando combine una anotación de argumento con un valor predeterminado, use espacios alrededor del signo = :

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* Las declaraciones compuestas (declaraciones múltiples en la misma línea) generalmente se desaconsejan:

*Correcto*
```python
foo = (0,)
```
**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

* Más bien no:

**Incorrecto**
```
spam( ham[ 1 ], { eggs: 2 } )
```

### Comentarios

El código, desde un inicio, estará comentado ampliamente.

Los comentarios tendrán el siguiente formato:

* Una línea en blanco encima (excepto si siguen la norma de *docstrings*)
* Un espacio entre \# y la primera letra
* Primera letra mayúscula
* Texto en español con toda la puntuación y acentos necesarios (el código fuente de Python acepta UTF-8, entre otras codificaciones internacionales)

**Ejemplo**

```python
import numpy as np
from scipy import stats

# Número de muestras
N = 500

# ¿Variable aleatoria de la simulación?
X = stats.norm(0, 1)
```
