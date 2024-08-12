# Introducción a Minería de textos con Python

[![Python](https://img.shields.io/badge/python-3.12.5-blue.svg)](https://www.python.org/ftp/python/3.12.5/python-3.12.5-amd64.exe)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rominicky/materiales/main)

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

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rominicky/materiales/main)

Puede ingresar rápidamente a las notebooks hacer click en el botón **"Launch Binder"**. Se iniciará un entorno virtual en su navegador, allí se podrá abrir y ejecutar las notebboks sin instalar nada.

#### ¿Qué es Binder? ¿Cuáles son sus limitaciones?

Binder es una herramienta en línea que permite a los usuarios crear y compartir entornos interactivos y reproducibles.

Sus limitaciones:
  * Algunas celdas pueden utilizar más memoria de la que permite Binder, provocando el bloqueo de la notebook.
  * Puede cerrarse luego de unos 10 minutos de inactividad, se deberá recargar la notebook.
  * Binder **no guarda** los cambios que se realicen en la notebook.

### Ejecución en Local

Instrucciones si no se ha instalado previamente Jupyter o Python en su propia computadora. Mi recomendación es realizarlo con Anaconda, porque evita hacer varias instalaciones. 

**Anaconda** es una distribucación de software libre y de código abierto de los lenguajes Python y R; ​muy utilizada en Ciencia de datos y Aprendizaje automático (Machine Learning), debido a su simplificación en la gestión e implementación de paquetes.​ Su trabajo incluye procesamiento de grandes volúmenes de información, análisis predictivo y cómputos científicos.

#### Instalación de Jupyter Notebooks y Python con Anaconda

[![Anaconda (Python 3.12)](https://www.anaconda.com/wp-content/uploads/2022/12/anaconda_secondary_logo.svg)](https://www.anaconda.com/download/success)

Una vez instalado, abra el navegador de Anaconda [![Anaconda Navigator](https://docs.anaconda.com/_images/nav-tabs1.png)](http://docs.anaconda.com/anaconda/user-guide/getting-started/#open-navigator). 

### Descargue las notebooks de GitHub

Vaya a la [página de GitHub](https://github.com/rominicky/materiales/mineria-texto)
donde se guardan las notebooks de este repositorio, se podrán descargar cada unas de ellashaga clic en el botón verde "Código" en la parte superior derecha de la página.

![](assets/download-or-clone.png)

Si nunca ha usado el control de versiones `git` antes, le recomiendo que simplemente descargue los cuadernos con la opción
"Descargar ZIP". En la mayoría de los sistemas operativos, esto lo descomprimirá automáticamente en archivos individuales. Mueva
la carpeta a algún lugar donde desee conservarla, como "Mis documentos".

Si ha usado `git` antes, puede clonar el repositorio con este comando:

`git clone https://github.com/mchesterkadwell/intro-to-text-mining-with-python-2020.git`

### Ejecute cuadernos en un entorno dedicado

En términos simples, un entorno es como una caja aislada en la que se ejecuta un cuaderno a salvo de la interferencia de otros cuadernos. Anaconda proporciona un entorno predeterminado, llamado 'root', en el que puede comenzar a funcionar rápidamente. Sin embargo, debería crear un nuevo entorno para cada proyecto (que puede tener uno o más cuadernos relacionados).

En **Anaconda Navigator > Entornos**, haga clic en el botón "Crear" en la parte inferior izquierda de la lista de Entornos.

![](assets/create.png)

Escriba un nombre, por ejemplo, "intro-to-text-mining", asegúrese de que "Python" esté _marcado_
y en el menú desplegable seleccione **'3.9'**. Asegúrese de que "R" esté _desmarcado_.

Luego, haga clic en el botón "Crear".

![](assets/new-env.png)

Tomará unos segundos configurarlo...

Luego, en **Anaconda Navigator > Entornos**, asegúrese de haber seleccionado su
nuevo entorno.

A la derecha del nombre del entorno hay una pequeña flecha verde de reproducción. Haga clic en ella y seleccione "Abrir terminal" en el
menú desplegable.

En la terminal que se abre, escriba lo siguiente y presione Enter:

`conda install pip`

![](assets/conda-install-pip.png)

Si aún no tiene pip instalado, lo instalará. De lo contrario, mostrará un mensaje:

`# Todos los paquetes solicitados ya están instalados.`

Luego, cambie el directorio a donde haya guardado la carpeta de cuadernos escribiendo algo como:

`cd path\to\notebooks`

donde `path\to\notebooks` es la ruta del archivo donde haya colocado la carpeta de cuadernos.

Si está en una **Mac**, asegúrese de usar barras diagonales en la ruta del archivo, por ejemplo `path/to/notebooks`

![](assets/cd-directory.png)

Luego, instala todas las dependencias escribiendo:

`pip install -r requirements.txt`

Luego:

`pip install jupyter`

Esto debería iniciar una gran lista de descargas y tardará un tiempo en finalizar. Ten paciencia.

Por último, para iniciar el servidor de Jupyter Notebook, escribe:

`jupyter notebook`

Esto abre una página web que muestra el proyecto:

![](assets/jupyter-notebooks.png)

Si no, puedes copiar y pegar una de las URL en la ventana de la Terminal en tu navegador, por ejemplo:

http://localhost:8888/?token=ddb27d2a1a6cb29a3483c24d6ff9f7263eb9676f02d71075
(Este no funcionará en su máquina, ya que el token es único cada vez).

Cuando haya terminado con el notebook, presione **ctrl+c** para detener el servidor notebook.

Puede cerrar la ventana de Terminal.

### Iniciar el servidor notebook nuevamente

La próxima vez que desee iniciar el servidor notebook:

En **Anaconda Navigator > Environments** asegúrese de haber seleccionado su nuevo entorno.

A la derecha del nombre del entorno hay una pequeña flecha verde de reproducción. Haga clic en ella y seleccione "Abrir terminal" en el
menú desplegable.
Para iniciar el servidor notebook Jupyter, escriba:

`jupyter notebook`

Cuando haya terminado con el notebook, presione **ctrl+c** para detener el servidor notebook. Puede cerrar la ventana de Terminal.

### Licencia

El texto está licenciado bajo Creative Commons
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

¡Gracias por leer!