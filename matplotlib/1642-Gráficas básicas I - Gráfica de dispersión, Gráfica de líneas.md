* Los términos Diagrama, Cuadro y Gráfico se superponen parcialmente, se usan de forma un tanto imprecisa, y en esa superposición, en realidad no hay ninguna diferencia significativa que necesite saber en este momento.
* Por lo tanto, no hay necesidad de confundirse si encuentra que diagrama de barras, gráfico de barras y cuadro de barras se usan indistintamente en algunos lugares.
* Echemos un vistazo a las gráficas comúnmente utilizadas en Matplotlib ahora.







## Gráfico de dispersión

### ¿Qué es el diagrama de dispersión?

* Un diagrama de dispersión (también conocido como gráfico de dispersión, cuadro de dispersión) usa puntos para representar valores para diferentes variables numéricas.
* La posición de cada punto en el eje horizontal y vertical indica valores para un punto de datos individual.
* Los diagramas de dispersión se utilizan para observar las relaciones entre las variables.









![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5f5dd9dc082849309f19d4c7542ed3f5.png)








### Creación de un diagrama de dispersión

Para crear un diagrama de dispersión en Matplotlib podemos usar el método .scatter():







![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_eb846dc1ed204e4e8013db2215a9f675.png)






### ¿Siempre se requiere plt.show()?

Es posible que haya observado la línea plt.show() después de plt.scatter(). ¿Es necesario usar?

* Si Matplotlib se usa en una terminal, scripts o IDE especializados como Spyder, Pycharm o VS Code, plt.show() es imprescindible.
* Si Matplotlib se usa en un shell de iPython o en un cuaderno como Jupyter Notebook o Colab Notebook, plt.show\(\) generalmente no es necesario.

El comando plt.show() hace mucho bajo el capó, ya que debe interactuar con el backend gráfico interactivo de su sistema. Los detalles de esta operación pueden variar mucho de un sistema a otro e incluso de una instalación a otra, pero matplotlib hace todo lo posible para ocultarle todos estos detalles.

En la siguiente celda estamos ejecutando el mismo script que arriba, eliminando la instrucción plt.show():




![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_955a071b23c747ccb9e06a71835cae3e.png)





Si desea evitar que esto se incluya como resultado de una celda, use plt.show() al final de cada instrucción de trazado.

### Aplicaciones del diagrama de dispersión

* Un diagrama de dispersión puede ser útil para identificar otros patrones en los datos.
* Podemos dividir los puntos de datos en grupos en función de qué tan cerca se agrupan los conjuntos de puntos.
* Los diagramas de dispersión también pueden mostrar si hay brechas inesperadas en los datos y si hay puntos atípicos. (Mire los 2 puntos alejados del resto de los datos en el diagrama de dispersión. Esos son valores atípicos).
* Esto puede ser útil si queremos segmentar los datos en diferentes partes, como categorizar a los usuarios en diferentes grupos.




## Gráfico de líneas

### ¿Qué es el diagrama de líneas?

Un gráfico de líneas se utiliza para representar datos durante un período de tiempo continuo. Generalmente se utiliza para mostrar la tendencia de una variable a lo largo del tiempo. Los valores de los datos se trazan como puntos que se conectan mediante segmentos de línea.

### Creación de un diagrama de líneas (con 2 argumentos)

* En Matplotlib podemos crear un gráfico de líneas llamando al método plot.
* plot() es un comando versátil y puede tomar un número arbitrario de argumentos.








![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_66da213cfc0e402890a57b7582ce8c48.png)







Debido a que es un gráfico de líneas, matplotlib dibuja automáticamente una línea para conectar cada par de puntos consecutivos que representan coordenadas en el gráfico.

### Creación de un diagrama de líneas (con un solo argumento)

* Podemos hacer un gráfico con una simple línea de código como se menciona en la imagen:









![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5498e847bafa4baabed998c816311f1d.png)









* Quizás se pregunte por qué el eje x varía de 0 a 3 y el eje y de 1 a 4.
* Si proporciona una lista de n elementos a la función .plot(), matplotlib asumirá que es una secuencia de valores y, y generará automáticamente los valores x como un rango de n elementos a partir de 0.
* Dado que los rangos de Python comienzan con 0, la lista predeterminada x tiene la misma longitud que y. Por lo tanto, los datos de x serán [0,1,2,3]. (Longitud igual que y(4) pero comienza desde 0 en su lugar).

### Aplicaciones del gráfico de líneas

Con un gráfico de líneas, se puede ver el patrón de cualquier variable dependiente a lo largo del tiempo, como el precio de las acciones, los registros meteorológicos (como la temperatura, la precipitación o la humedad), etc.

Veamos un ejemplo de la representación gráfica del crecimiento del número de suscriptores de pago de Netflix de 2012 a 2018:

![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f1729089bc8746e49b8d6744b0c66f07.png)