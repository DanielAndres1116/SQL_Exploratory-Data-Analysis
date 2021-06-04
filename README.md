# EXPLORACIÓN DE BASES DE DATOS MEDIANTE SQL

### Descripción del conjunto de datos analizado

Fueron analizados tres conjuntos de datos disponibles en el Portal de la ciudad de Chicago con la finalidad de seleccionar y consultar ciertas características que resultan útiles en el estudio estadístico de la población. Fue utilizado el lenguaje de consulta estructurada SQL para llevar a cabo la observación de dichas características. 

El primer conjunto de datos se trata de una tabla que contiene una selección de seis indicadores socioeconómicos de importancia para el progreso poblacional y un "índice de dificultades" de cada área de la comunidad de Chicago. En esta tabla hay un listado de nombres de las areas comunitarias, porcentaje de viviendas concurridas, porcentaje de personas desempleadas, porcentaje de personas sin estudios, entre otros. A continuación una parte de la tabla con algunos de sus datos:

![imagen](https://user-images.githubusercontent.com/43154438/120733577-1b386880-c4ad-11eb-94a2-06cb55550759.png)

#### Tabla 1 - Indicadores Socioeconómicos
Enlace: https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2



El segundo conjunto de datos muestra todos los datos de rendimiento a nivel escolar que se utilizan para crear las boletas de calificaciones escolares. Esta tabla brinda una serie de datos que permite hacerse una idea del nivel de rendimiento escolar de cada escuela. Entre estos datos está el nivel de seguridad, número de familias que allí estudiaron, puntaje a los profesores, tasa de malas conductas en los estudiantes, etc. A continuación algunos de los datos dentro de la tabla:

![imagen](https://user-images.githubusercontent.com/43154438/120734688-efb67d80-c4ae-11eb-8906-1c0a95917858.png)

#### Tabla 2 - Indicadores Escolares
Enlace: https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t



El tercer conjunto de datos refleja los incidentes de delitos denunciados que ocurrieron en la ciudad de Chicago. Debido a que este último conjunto de datos es bastante más grande, para los propósitos de este ejercicio se utilizó una muestra mucho más pequeña del conjunto de datos original. Aquí hay datos como el tipo de lugar donde se perpetró el crimen, una breve descripción del crimen, localización, si hubo arresto o no, entre otros. Aquí un fragmento de la tabla:

![imagen](https://user-images.githubusercontent.com/43154438/120735106-9dc22780-c4af-11eb-80da-3d54e57a9903.png)

#### Tabla 3 - Indicadores de Crímenes
Enlace: https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2

De cada una de estas tablas se puede extraer variada cantidad de información con el fin de hacer estudios de diferente índole. 

### Objetivos

Comprender los 3 conjuntos de datos en cuestión, cargarlos en 3 tablas en una plataforma online, en este caso Watson Studio Platform de IBM en una sección destinada a bases de datos y ejecutar determinadas consultas SQL útiles a los diferentes conjuntos de datos ya cargados en la nube. Para comunicarse con bases de datos SQL desde dentro de un Notebook en JupyterLab fueron utilizados comandos de SQL-Magic proporcionados por la extensión ipython-sql. Cabe destacar que esta clase de consultas se pueden hacer en diferentes tipos de plataformas en la nube de diferentes páginas web. 

Para hacer la conexión con esta plataforma fue necesario por ejemplo crear una cuenta y obtener una Credencial de Servicios como es mostrado a continuación:

![imagen](https://user-images.githubusercontent.com/43154438/120737481-bfbda900-c4b3-11eb-969b-176e0a4a5493.png)

#### Imagen 1: Credenciales de servicio en la nube

Los diferentes tipos de consulta que se hicieron a los datos fueron:

- Conteo del número total de crímenes
- Conteo de la cantidad de crímenes que involucraron un arresto
- Averiguar cuántos crímenes registrados hubo de cada tipo en ubicaciones de gasolineras (robos, robos a mano armada, venta de carcóticos, etc.), esta clase de consulta puede aplicarse a cada tipo de local. 
- Extraer la información de Areas Comunitarias que inicien con cierta letra
- Obtain which schools in certain Community Areas are healthy school certified
- Consultar cuales escuelas en determinada area comunitaria tienen certificaciones en alta calidad
- Calcular el promedio de seguridad escolar. 
- Hacer una lista de las 5 areas comunitarias con mayor número de estudiantes. 
- Determinar cual area comunitaria tiene el menor valor de puntaje de seguridad escolar
- Hallar el ingreso Per-Cápita de las áreas comunitarias que tienen el mayor puntaje de seguridad escolar. 


### Conclusions

Cualquiera que sea el conjunto de datos y los tipos de datos guardados en su interior, es posible realizar consultas mediante comandos del lenguaje SQL permitiendo así su exploración y entendimiento, dentro o fuera de una nube en diferentes plataformas web. 

A continuación algunos de los resultados de las consultas:

- Conteo del número total de crímenes:

![imagen](https://user-images.githubusercontent.com/43154438/120738461-7f5f2a80-c4b5-11eb-8105-9460097f9346.png)

- Cantidad de crimenes que involucaron un arresto:

![imagen](https://user-images.githubusercontent.com/43154438/120738477-85eda200-c4b5-11eb-84c6-71c69abc9302.png)

- Crímenes registrados que hubo de cada tipo en ubicaciones de gasolineras:

![imagen](https://user-images.githubusercontent.com/43154438/120738492-8d14b000-c4b5-11eb-8acc-60ce372ef061.png)

- lista de las 5 areas comunitarias con mayor número de estudiantes:

![imagen](https://user-images.githubusercontent.com/43154438/120738511-930a9100-c4b5-11eb-93f1-0815af24b858.png)

En el Notebook (.ipynb) está mejor explicada cada parte del código de programación. 

#### Nota: también se puede ver el código acá: https://nbviewer.jupyter.org/github/DanielAndres1116/SQL_Exploratory-Data-Analysis/blob/main/SQL_Data_Analysis.ipynb
