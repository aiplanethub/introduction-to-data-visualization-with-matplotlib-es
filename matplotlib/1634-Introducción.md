## Objetivos de aprendizaje

* Introducción a Matplotlib
* Ventajas
* Instalación
* Importación de Matplotlib
* Gráfico Matplotlib

## Introducción

* Matplotlib es la biblioteca de gráficos de Python más popular.
* Es una biblioteca completa para crear visualizaciones estáticas, animadas e interactivas en Python.
* Es útil para aquellos que trabajan con Python y NumPy.
* Es una biblioteca de bajo nivel con una interfaz similar a MATLAB que ofrece mucha libertad a costa de tener que escribir más código.

## Ventajas

* Extremadamente poderoso
* Rápido y eficiente
* Código abierto
* Funciona bien con muchos sistemas operativos y backends gráficos
* Gráficos y plots de alta calidad.
* Capacidad para generar y ver una gran variedad de gráficos
* Soporte de una gran comunidad y soporte multiplataforma
* Control total sobre gráficos o estilos de plots




## Instalación

* Antes de poder utilizar las funciones de trazado de Matplotlib, es necesario instalar Matplotlib.
* La distribución Anaconda de Python y Google Colab viene con Matplotlib preinstalado y no se necesitan más pasos de instalación.
* Sin embargo, si no está utilizando ninguno de ellos, puede instalarlo ejecutando un comando pip simple en su terminal: **`pip install matplotlib`**






### Pyplot

El módulo más utilizado de Matplotlib es Pyplot, que es el marco de trazado de Matplotlib.

Cada función de pyplot realiza algún cambio en una figura: por ejemplo, crea una figura, crea un área de trazado en una figura, traza algunas líneas en un área de trazado, decora el trazado con etiquetas, etc.

## Importando matplotlib

Hay muchos módulos en Matplotlib, pero para fines de trazado, solo importamos pyplot.

Así como usamos la abreviatura np para NumPy y la abreviatura pd para Pandas, usaremos la abreviatura estándar 'plt' para la importación de Matplotlib:

**`importar matplotlib.pyplot como plt`**



## Gráfico Matplotlib

Los gráficos de Matplotlib se componen de dos componentes principales:

* **Los ejes:** las líneas que delimitan el área del gráfico
* **La figura:** donde dibujamos los ejes, títulos y elementos que salen del área de los ejes.

Nota: A diferencia del plural de axis, axes en Matplotlib es en realidad el cuadro rectangular completo que contiene las líneas, marcas y etiquetas del eje.
![image.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_80a3f7287fc34c1b8320e7a8ce8618a5.png)