# Cómo utilizar estos tutoriales

Estos tutoriales son *notebooks* de [Jupyter](https://jupyter.org/):

> Jupyter Notebook es la aplicación web original para crear y compartir documentos computacionales. Ofrece una experiencia simple, optimizada y centrada en documentos.

Estos documentos combinan texto, escrito en [Markdown](https://www.markdownguide.org/) (igual que este documento), junto con fragmentos **ejecutables** de código en Python.

## Instalación local

Jupyter opera como un servidor web local que despliega en un navegador (Chrome, Firefox, etc.) el *notebook* como un sitio web. Una vez instalado, una forma de iniciarlo es en la terminal de comandos, haciendo:

```bash
$ jupyter notebook
```

La forma más sencilla de instalar Jupyter y los paquetes necesarios de Python necesarios para el curso es a través de la distribución de [Anaconda](https://www.anaconda.com/products/distribution):

> La distribución de Anaconda tiene todo lo que necesita para iniciarse en la ciencia de datos en su estación de trabajo: instalación gratuita, miles de los paquetes fundamentales en DS, AI y ML, administración de paquetes y entornos desde la aplicación de escritorio y más.

## Descargar los archivos PyX

Para descargar estos archivos desde GitHub en su computadora puede hacerlo ingresando a la siguiente sección del repositorio:

<img src="https://docs.github.com/assets/cb-20363/mw-1000/images/help/repository/code-button.webp"  width="300">

Y ahí:

- **Manualmente**: con la opción "Download ZIP".
- **Clonado con Git**: según las [instrucciones](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository) hay que copiar el link del repositorio 

<img src="https://docs.github.com/assets/cb-33207/mw-1000/images/help/repository/https-url-clone-cli.webp"  width="300">

y en la terminal de comandos hacer:

```bash
(directorio) $ git clone https://github.com/fabianabarca/python.git
```

que creará una copia en el `(directorio)` actual. Es necesario primero instalar [Git](https://git-scm.com/) en la computadora.

## Otras opciones de ejecución

### En el IDE

Algunos entornos integrados de desarrollo como [Visual Studio Code](https://code.visualstudio.com/) pueden ejecutar directamente el *notebook* de Jupyter sin necesidad de un navegador y del servidor local. Para esto es necesario algún soporte como un [paquete de extensión](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter).

### En la nube

También es posible ejecutar *notebooks* en la nube, sin instalar nada localmente, con varios sitios:

- [Google Colab](https://colab.research.google.com/) (opción popular)
- [Binder](https://mybinder.org/)
- [Datalore](https://datalore.jetbrains.com/)
- Otros

## Ejecutar el *notebook*

Una vez corriendo el *notebook*, para ejecutar una celda de código se debe usar el botón "Run" o bien hacer `Shift + Enter` en el teclado.
