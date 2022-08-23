## Histograma

### ¿Qué es un histograma?

Un histograma es una representación gráfica de datos utilizando barras (rectángulos) de diferentes alturas.

### Partes de un histograma

* **El título:** El título describe la información incluida en el histograma.
* **Eje X:** El eje X son intervalos que muestran la escala de valores en la que se encuentran las medidas. Estos intervalos también se denominan bins.
* **Eje Y:** El eje Y muestra la cantidad de veces que ocurrieron los valores (frecuencia) para cada intervalo en el eje X.
* **Las barras:** La altura de la barra muestra la cantidad de veces que ocurrieron los valores dentro del intervalo, mientras que el ancho de la barra muestra el intervalo cubierto.



### Ejemplo: Altura de los naranjos

* La altura de cada árbol de la huerta la mides en centímetros (cm)
* Las alturas varían de 100 cm a 340 cm
* Decides poner los resultados en grupos de 50 cm:
  * El rango de 100 a justo por debajo de 150 cm,
  * El rango de 150 a poco menos de 200 cm, Etc...
* Entonces, un árbol que mide 260 cm de altura se agrega al rango "250-300".











![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_d5d586fd4a2e47daa555be899b531aca.png)














* **Y aqui esta el resultado:**






![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2f22bdd00d5341adb508d41986111197.png)






* Puedes ver (por ejemplo) que hay 30 árboles de 150 cm a poco menos de 200 cm de altura. ¡Acabas de crear un histograma!
* Fuente: https://www.mathsisfun.com/data/histograms.html



### Creación de un histograma

Matplotlib se puede usar para crear histogramas usando el método hist().

**Parámetros:**

* x(n,): esto toma una sola matriz o una secuencia de matrices que no se requiere que tengan la misma longitud.
* bins: intervalos de cualquier cantidad

Si los contenedores son:

[1, 2, 3, 4]

entonces el primer contenedor es [1, 2) (incluyendo 1, pero excluyendo 2) y el segundo [2, 3]. Sin embargo, el último contenedor es [3, 4], que incluye 4.






![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_63e97e1cab1547bbb0ac9e72357fb840.png)






### Aplicaciones del histograma

* Los histogramas son un tipo de gráfico muy común cuando se analizan datos como la altura y el peso, los precios de las acciones, el tiempo de espera de un cliente, etc., que son de naturaleza continua.
* Los histogramas son buenos para mostrar las características generales de distribución de las variables del conjunto de datos. Puede ver aproximadamente dónde están los picos de la distribución, si la distribución es sesgada o simétrica y si hay valores atípicos.

## Gráfica de barras

### ¿Qué es el gráfico de barras?

Los gráficos de barras son uno de los gráficos más comunes utilizados para mostrar datos asociados con variables categóricas.

Veamos algunas formas de mostrar un gráfico de barras con matplotlib:






![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f6582cfb0ad94fa8bbd6c1a5caa48686.png)





### Creación de un gráfico de barras verticales

Pyplot proporciona un método bar() para hacer gráficos de barras que toman los siguientes argumentos: variables categóricas, sus valores y color (si desea especificar alguno).








![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_21c6bb192e6b4cd2b42179ac53b0dfd9.png)










### Creación de un diagrama de barra horizontal

Hacer un gráfico de barras horizontales también es muy simple usando el método plt.barh().









![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_5f02309e817b4caeacc3515946d57b14.png)








### Gráficos de barras con múltiples cantidades

Al comparar varias cantidades y cambiar una variable, es posible que deseemos un gráfico de barras con barras de un color para un valor de cantidad.

Podemos trazar múltiples gráficos de barras jugando con el grosor y las posiciones de las barras.





![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_ac9c91b9bdaa488ea6670e133440dedc.png)





### Gráficos de barras apiladas

El gráfico de barras apiladas apila barras que representan diferentes grupos una encima de la otra. La altura de la barra resultante muestra el resultado combinado de los grupos.






![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_f2cfb1391fc7464a925f36ba15e8b6a7.png)





### Aplicaciones de los gráficos de barras

Los gráficos de barras se utilizan para hacer coincidir cosas entre diferentes grupos o para rastrear cambios a lo largo del tiempo. Mire el siguiente gráfico de barras que representa las habilidades tecnológicas más demandadas para los ingenieros de datos.







![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7efdb65711b44d47b19cf579b6519c62.png)







### Gráfico de barras frente a histograma

Los histogramas son una excelente manera de mostrar resultados de datos continuos, como:

* peso
* altura
* cuanto tiempo etc

Pero cuando los datos están en categorías (como país o película favorita), debemos usar un gráfico de barras. Eche un vistazo a la siguiente parte que describe la diferencia entre histograma y gráfico de barras:








![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_2f1be5631f5242b8bc28e05a1e66fd3f.png)








## Gráfico circular

### ¿Qué es un gráfico circular?

* Un gráfico de pastel (o gráfico circular) es un gráfico estadístico circular, que se divide en porciones (cuñas) para ilustrar la proporción numérica.
* * Imagina una pizza en la que diferentes rebanadas contienen diferentes ingredientes. Cuanto más grande sea la rebanada, mayor será la cantidad de esa cobertura presente.








![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_22c4c086041540838c428ed1ed0bd044.png)







### Parámetros de un gráfico circular

* x: Los tamaños de cuña.
* etiquetas: una secuencia de cadenas que proporciona las etiquetas para cada cuña.
* Colores: una secuencia de colores a través de la cual se desplazará el gráfico circular. Si es Ninguno, usará los colores en el ciclo actualmente activo.
* Autopct: cadena, utilizada para etiquetar las cuñas con su valor numérico. La etiqueta se colocará dentro de la cuña. La cadena de formato será fmt%pct.

¡También podemos pasar argumentos para personalizar nuestro gráfico circular para mostrar sombras, explotar una parte de él, inclinarlo en ángulo o hacer muchas cosas más emocionantes!

**No se abrume con los términos que se utilizan, todo quedará claro en la siguiente sección.**

### Creación de un gráfico circular

El gráfico circular se puede hacer usando el método pie().




![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_c0b0e09c28364ca8a7ea866745736123.png)





### Aplicaciones de los gráficos circulares

* Un gráfico circular se utiliza mejor cuando se trata de calcular la composición de algo. Si tiene datos categóricos, usar un gráfico circular funcionaría muy bien, ya que cada sector puede representar una categoría diferente. Un buen ejemplo de un gráfico circular se puede ver a continuación.





![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_08352ad4b0414f1da1e11e3839c5be69.png)





* Otro buen uso para un gráfico circular sería comparar áreas de crecimiento dentro de un negocio, como facturación, ganancias y exposición.
* Intente crear un gráfico circular para ver cuánto dinero gasta en diferentes áreas.