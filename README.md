# Vertex AI: ¿Cómo hacer ciencia de datos en la nube de Google?

## Intro
Este es el repo del workshop **Vertex AI: ¿Cómo hacer ciencia de datos en la nube de Google?**. En el contexto del uso de Vertex AI como solución para la puesta productiva de modelos de machine learning, la idea es empezar a amigarnos con la nube de forma amena y lo más sencilla posible. A lo largo del taller vamos a introducir algunos servicios de Google Cloud Platform (GCP) tales como BigQuery (data warehousing), Google Cloud Storage (almacenamiento de objetos) y Container Registry (repositorio de imágenes de Docker).

En ambos casos, los modelos toman datos de público acceso mediante BigQuery, específicamente el dataset *Dry Bean Dataset*.

## ¿Cómo lo corro?
Primero, ejecutar la notebook **00_cloud_setup.ipynb**. Contiene la configuración de la infraestructura que será utilizada (los buckets de GCS que se usarán en los ejercicios y las librerías necesarias). Luego, dentro de cada carpeta hay dos notebooks con los casos que se van a revisar.

### 01_automl
Este caso utiliza AutoML para la clasificación. El otro aspecto interesante es que utiliza un componente custom de Kubeflow para la evaluación de la performance del modelo, decidiendo de forma automatizada si generar un endpoint con el modelo entrenado. Se busca ilustrar la sencillez en el armado de pipelines con componentes out of the box (y en este caso, inclusive mediante la interfaz gráfica, si se quisiera).

### 02_customtrain
En este caso se construye un container custom de Docker para el entrenamiento de modelos que requieran una complejidad superior. Cuando los componentes prefabricados no son suficientes, esta es una de las técnicas posibles para construir una infraestructura de forma relativamente sencilla.

## Consideraciones y recomendaciones
A la nube no hay que tenerle miedo, hay que tenerle respeto :) 

Si es tu primera vez con estos servicios, ¡paciencia! Con los créditos gratuitos de Google te alcanza y sobra para estos ejercicios (las cuentas nuevas reciben 300 dólares que pueden usar en un lapso de 90 días), pero de todas formas, los costos aproximados de ambos son:

- 01_automl: $25 dólares. AutoML es sencillo, pero no es tan económico como otras alternativas, tales como...
- 02_customtrain: $3 dólares. Acá la ventaja es que al hacer algunas cosas más a mano se pueden abaratar los costos.

De todas formas están las celdas ejecutas (y revisadas) para que veas lo que pasa en cada paso, por lo que si no podés correrlo en algún entorno cloud podés entender lo que se vio a lo largo del workshop.

## ¿Qué puedo hacer con esto?
Compartirlo, usarlo, desarmarlo... ¡lo que quieras! Si llegás a usarlo de alguna manera y te resulta de utilidad, siempre podés mencionarnos en cualquiera de nuestras redes: nos pondría muy contentos saber si esto te sirvió y cumplió con su cometido pedagógico :)

## Video de la charla
[Workshop - Vertex AI: ¿Cómo hacer ciencia de datos en la nube?](https://youtu.be/3ZGJ88cEeSc)

