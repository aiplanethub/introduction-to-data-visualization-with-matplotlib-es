## Objetivos de aprendizaje

* Importación de bibliotecas
* Sobre el conjunto de datos
* Cargando el conjunto de datos

## Importación de bibliotecas

Todas las capacidades de Python no se cargan en nuestro entorno de trabajo de forma predeterminada (incluso si ya están instaladas en su sistema). Entonces, importamos todas y cada una de las bibliotecas que queremos usar.

Importaremos numpy, pandas y matplotlib con sus respectivos alias: **np, pd y plt.**






![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_4cbfb8081ca44de7b679b1f58e5a9144.png)






## Acerca del conjunto de datos

**Nombre del conjunto de datos:** Conjunto de datos metropolitano estándar

**Descripción del conjunto de datos:**

* Contiene datos de 99 áreas metropolitanas estándar en los EE. UU., es decir, 99 entradas de fila.
* El conjunto de datos proporciona información sobre 11 variables para cada área para el período 1976-1977.
* Las áreas se han dividido en 4 regiones geográficas: 1=Noreste, 2=Norte-Central, 3=Sur, 4=Oeste.
* Las variables proporcionadas se enumeran en la siguiente tabla:








![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_0ffc57b6c31f48ff800b37f81f0cd107.png)






### Objetivo

El objetivo del problema es encontrar la tasa de criminalidad de cada área.

### Cargando el conjunto de datos

Para cargar el conjunto de datos, usaremos el método Pandas **read_csv**.

Aquí está el CSV del conjunto de datos: [Conjunto de datos de áreas metropolitanas estándar] (https://raw.githubusercontent.com/dphi-official/Datasets/master/Standard_Metropolitan_Areas_Data-data.csv)

![imagen.png](https://dphi-live.s3.amazonaws.com/media_uploads/image_7ffa3304d85343ae8fba3b9acff4d605.png)