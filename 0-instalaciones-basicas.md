# Introducción a Minería de textos con Python

[![Python](https://img.shields.io/badge/python-3.12.5-blue.svg)](https://www.python.org/ftp/python/3.12.5/python-3.12.5-amd64.exe)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rominicky/mineria-texto-python/main)

#### Romina De León
##### rdeleon@gmail.com

## Instalaciones previas

Este repositorio contiene Jupyter notebooks q son utilizadas para la enseñanza de Minería de texto en Python en la materia "Gestión de datos en contextos organizacionales" de la Maestría y Especialización en Métodos Cuantitativos para la Gestión y Análisis de Datos en Organizaciones, de la Facultad de Ciencias Económicas (UBA).

Una **notebook** es un entorno virtual, un documento computacional interactivo, que se utiliza en programación combinando código, visualizaciones y documentación. Estas son diseñadas, en este repositoio, para el trabajo a propio ritmo. Tienen como objetivo presentar los conceptos básicos en un flujo de trabajo de minería de texto, dirigido a principiantes.

### Contenido

* Python básico (cadenas, listas, comprensión de listas, importaciones, funciones, abrir/leer/guardar archivos)
* Pasos en una secuencia de minería de texto
* Conceptos básicos de minería de texto (tokenización, normalización, limpieza, palabras vacías)
* Creación de una distribución de frecuencia y representación gráfica de los resultados

### Ejecutar notebooks en línea

#### Vista rápida en Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rominicky/mineria-texto-python/main)

Puede ingresar rápidamente a las notebooks hacer click en el botón **"Launch Binder"**. Se iniciará un entorno virtual en su navegador, allí se podrá abrir y ejecutar las notebboks sin instalar nada.

#### ¿Qué es Binder? ¿Cuáles son sus limitaciones?

Binder es una herramienta en línea que permite a los usuarios crear y compartir entornos interactivos y reproducibles.

Sus limitaciones:
  * Algunas celdas pueden utilizar más memoria de la que permite Binder, provocando el bloqueo de la notebook.
  * Puede cerrarse luego de unos 10 minutos de inactividad, se deberá recargar la notebook.
  * Binder **no guarda** los cambios que se realicen en la notebook.

### Ejecución en Local

Instrucciones para instalar Jupyter y Python en su propia computadora. Recomiendo hacerlo con Anaconda, ya que simplifica la instalación de varios paquetes. 

**Anaconda** es una distribucación de software libre y de código abierto para los lenguajes Python y R; ​ampliamente utilizada en Ciencia de Datos y Aprendizaje automático (Machine Learning) debido a su facilidad en la gestión e implementación de paquetes.​ Su uso incluye el procesamiento de grandes volúmenes de información, análisis predictivo y cómputos científicos.

#### Instalación de Jupyter Notebooks y Python con Anaconda

[![Anaconda (Python 3.12)](https://www.anaconda.com/wp-content/uploads/2022/12/anaconda_secondary_logo.svg)](https://www.anaconda.com/download/success)

La instalación de Anaconda incluye Python, Jupyter y varios módulos de Python que son necesarios para realizar análisis.

Una vez instalado, abra el navegador de Anaconda 

[![Anaconda Navigator](https://docs.anaconda.com/_images/nav-tabs1.png)](http://docs.anaconda.com/anaconda/user-guide/getting-started/#open-navigator)

Desde allí abrir la interfaz **Jupyter Lab** o **Notebook**.

##### Diferencias entre JupyterLab y Jupyter Notebook

JupyterLab y Jupyter Notebook difieren principalmente en su interfaz de usuario, funcionalidad y flexibilidad. Jupyter Notebook tiene una interfaz más simple y ligera, mientras que JupyterLab ofrece una interfaz más versátil y rica en funciones.

### Descargue las notebooks de GitHub

Vaya a la [página de GitHub](https://github.com/rominicky/mineria-texto-python/)
donde se almacenan las notebooks de este repositorio, se podrán descargar desde el botón verde **Code** en la parte superior derecha de la página.

![](https://docs.github.com/assets/cb-60499/mw-1440/images/help/repository/https-url-clone-cli.webp)

Si no tiene experiencia en el uso de control de versiones `git`, recomiendo descargar con la opción **Download ZIP**.

Si ya está familiarizado con `git`, puedes clonar el repositorio con este comando:

`git clone https://github.com/rominicky/mineria-texto-python.git`

### Ejecutar las notebooks en Anaconda

Una vez abierto JupyterLab o Jupyter Notebook, navegue a la carpeta donde guardó las notebooks descargadas. Puede hacerlo desde la interfaz de usuario de Jupyter, que muestra un explorador de archivos en el lado izquierdo de la pantalla.

  * JupyterLab: En el panel de archivos a la izquierda, navegue a la ubicación donde están guardadas las notebooks (*.ipynb). Haga doble clic en el archivo que desea abrir.    
  * Jupyter Notebook: En la interfaz principal, verá un listado de archivos y carpetas en su directorio de trabajo actual. Navegue hasta la carpeta donde guardó las notebooks y haga clic en el archivo *.ipynb que desea abrir.

**Nota** 
Si no recuerda dónde guardó las notebooks, puede verificar la ubicación predeterminada en la que se abrió Jupyter. Esta suele ser la carpeta que estaba abierta en su sistema cuando ejecutó Jupyter desde Anaconda Navigator o la línea de comandos.

[Introducción a Python y minería de textos](1-introduccion-python-texto.ipynb)
[Procesamiento de textos y Visualización de los resultados](2-procesamiento-texto-corpus.ipynb)


### Licencia

El texto está licenciado bajo Creative Commons
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

¡Gracias por leer!