# Detector de Fotografo en Flickr e Instagram
En este repositorio encontramos los archivos utilizados para la exploración de técnicas de desarrollo de modelos de detección de fotógrafos en las plataformas de Flickr e Instagram.

## Requisitos
Para replicar los experimentos llevados a cabo, es necesario disponer de los conjuntos de datos que se utilizan a los largo de estos. No obstante, dichos conjuntos de datos no se proporcionan en este repositorio. Si usted quiere replicar los experimentos del proyecto, contacte con jesus.v.c@um.es, y se considerará la proporción de estos.

## Flickr
En el notebook *Detector_Flickr*, desarrollamos dos modelos de detección de fotógrafos, a partir de dos etiquetas distintas, una obtenida de manera manual, y otra de manera automática, para usuarios de Flickr. Tras la obtención de dichos modelos, se procede a la realización de un test de la t de Student, para comparar la similitud de las predicciones.

## Instagram
En el notebook *Detector_Instagram, desarrollamos dos modelos de detección de fotógrafos, a partir de dos etiquetas distintas, una obtenida de manera manual, y otra de manera automática, para usuarios de Instagram. Tras la obtención de dichos modelos, se procede a la realización de un test de la t de Student, para comparar la similitud de las predicciones.

## Transfer Learning
El notebook *CreaciónDatos* indica la manera de obtener conjuntos de datos con dimensiones comunes, para cada plataforma, a partir de los datos de cada entorno por separado. La creación de estos datos es imprescindible para la aplicación del proceso detallado en el siguiente notebook.

El notebool *Detector_TL* indica el proceso llevado a cabo para la exploración de dos vías distintas de técnicas de aprendizaje por transferencia. 
* En la primera, nos entrenamos un modelo a partir de los datos de Instagra, y evaluamos el rendimiento que obtiene a la hora de predecir los datos de Flickr. También se entrena un modelo con los datos de Flickr, y se evalúa su capacidad de obtener predicciones a partir de los datos de Instagram.
* En la segunda, mostramos como obtener un modelo, a partir de combinar los datos procedentes de ambas redes sociales, y evaluamos su rendimiento con un conjunto de validación, procedente también de la combinación de los datos de ambas redes sociales.  
