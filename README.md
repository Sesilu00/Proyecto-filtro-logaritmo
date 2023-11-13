# Proyecto-filtro-logaritmo
Creación de una interfaz visual utilizando PyQT6 que permita aplicar la transformación logaritmo a las imágenes que se deseen, aplicando esta transformación con las funciones de la paquetería OpenCV2.

## Introducción
Con la realización de este programa se espera obtener una herramienta que pueda ser útil a la hora de trabajar con visión por computadora, por lo que se empezará definiendo este concepto. La visión por computadora o visión artificial es una rama de la inteligencia artificial que se encarga del análisis de imágenes digitales, videos y otros medios visuales utilizando computadoras y sistemas informáticos. La visión digital se inspira en la visión humana, pero con la diferencia de la capacidad de las computadoras de analizar datos de forma extremadamente rápida a comparación del tiempo que le toma a un humano, por lo que se pueden analizar miles de imágenes por minuto. 

Para que la computadora sea capaz de recibir la información visual necesaria se necesita de dispositivos como cámaras fotográficas o de vídeo, sensores de diversos tipos, procesadores y software especializado en este tipo de técnicas. En suma a esto, se necesita una gran cantidad de datos para entrenar a la computadoras. Actualmente existen una gran cantidad de aplicaciones para estas tecnologías, destacando el reconocimiento facil con propósitos de seguridad o de autenticación, por ejemplo, el sistema Face ID de Apple que le permite a un usuario desbloquear su iPhone simplemente escaneando su rostro.

Otro elemento importante en el desarrollo de este proyecto fueron las interfaces gráficas de usuario o GUI por sus siglas en inglés. Estos son programas que permiten la interacción entre un usuario y su computador de forma sencilla, ya que se basa en el uso de imágenes y elementos gráficos para la interacción con el programa. Son considerados como una evolución de las interfaces basadas en líneas de comando. Se suelen utilizar diferentes widgets que permiten la interacción "correcta" entre el usuario y el programa, por ejemplo, una caja de texto para ingresar un nombre de usuario, spinboxes para elegir entre una cantidad determinada de datos númericos, etc.

El uso de interfaces visuales permite hacer más accesibles las aplicaciones para personas con poco conocimiento del uso de computadoras, debido a su uso de elementos visuales fáciles de entender (suponiendo que se hayan desarrollado de forma adecuada).

## Materiales
El lenguaje de programación con el que se desarrollo este programa fue Python 3.11, eligiendo un enfoque de programación de objetos ya que este permite un mejor desarrollo de la GUI. El uso de este lenguaje se debe a la facilidad para programar en este lenguaje, su enfoque multiparadigma y la existencia de muchas paqueterías para el desarrollo de IA. Se utilizó el entorno de programación PyCharm 2023.2.3 con una licencia de estudiante, lo que permitió un desarrollo más eficaz del programa, aunque se encontraron algunos errores a la hora de utilizar algunas librerías.

Para el desarrollo de la GUI se ocupó la paqueteria PyQt6, que permite utilizar el software Qt con el lenguaje de Python. Se utilizaron muchos de los widgets disponibles, como Qlabel para mostrar texto e imágenes, QDoubleSpinBox para permitir la selección de un parámetro numérico, y también se utilzaron las QAction para desarrollar una barra de herramientas con muchos atajos de teclado para un uso más rápido del programa.

OpenCV2 fue la librería que se utilizó para aplicar el filtro a las imágenes. Su uso fue limitado, ya que solamente se necesitó para poder abrir las imágenes como una lista de vectores. Para aplicar la transformación en sí se utilizó la función logaritmo de la librería numpy. Un problema importante a la hora de leer imágenes es que OpenCV2 no soporta rutas de imágenes que contengan tildes, lo que no permite utilizar las imágenes que se encuentran en la carpeta "Imágenes" del computador.

Finalmente, aunque se permitió abrir imágenes con otros formatos, las imágenes con las que se puso a prueba el programa se encuentran en formato TIFF. La ventaja de este formato comparado con otros es que mantiene la imagen con una calidad muy alta y no tiene ninguna perdida, lo que es importante para la visión por computadora. Sin embargo, tiene la desventaja de que es mucho más pesado que otros formatos como el .jpg o .png, lo que impide su uso para conjuntos muy grandes de datos visuales.
