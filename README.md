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

### Cosas que fastidian

Hay que evitar espacios en blanco superfluos en las siguientes situaciones:

* En medio de paréntesis redondos o cuadrados, o llaves.
**Correcto**
```python
spam(ham[1], {eggs: 2})
```
