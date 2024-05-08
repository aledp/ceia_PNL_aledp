
* [Resolución del desafío 1](https://github.com/aledp/ceia_PNL_aledp/blob/ae185b76984d3a152eb3f0a46224aedd4881e623/Resolucion_Desafio_1_AlejandraDelPorto.ipynb)

Vectorización de documentos y medición de similaridad  ( usando cosine_similarity) entre documentos.

Se probaron distintos vectorizadores y modelos de clasificación cuyos resultados fueron comparados mediante F1-Score.

Para las distintas categorías de palabras, se presentó el listado de las 5 palabras con mayor similitud (a fin de evaluar la correcta pertenencia de tales palabras).

Principal librerías utilizadas:  sklearn, NLTK.


* [Resolución del desafío 2](https://github.com/aledp/ceia_PNL_aledp/blob/e189aafcd311070aaab098f10509ad77998aa971/Resolucion_Desafio_2_AlejandraDelPorto.ipynb)

Se entrenaron (utilizando Gensim) embedings a partir del corpus de letras de canciones de Natalia Laforucade.  Se probaron distintos modelos variando parámetros: tipo de modelo (cbow/skipgram), tamaño de vocabulario, tamaño de ventana de contexto.
Se realizaron mapas 2D y 3D para visualizar los vectores que respresentan las palabras, pudiendo visualizar la cercanía entre ellas de acuerdo al contexto en cual son utilizadas.

* [Resolución del desafío 3](https://github.com/aledp/ceia_PNL_aledp/blob/main/Resolucion_Desafio_3_AlejandraDelPorto.ipynb)

A partir de un corpus (el contenido de un libro) se entrenaron modelos con diferentes arquitecturas (GRU, LSTM, Bidireccionales, Cantidad de capas y neuronas, tamaño de contexto máximo) a fin de evaluar la perplejidad del entrenamiento para de cada uno.
Con el modelo seleccionado (el mejor perplejidad) se generaron secuencias de palabras (output) a partir de un input de palabras.

* [Resolución del desafío 4](https://github.com/aledp/ceia_PNL_aledp/blob/main/Resolucion_Desafio_4_bot_qa_AlejandraDelPorto.ipynb)
Se construyó un bot de preguntas y respuestas (Bot QA) .

El BotQA utiliza un dataset de conversaciones en inglés obtenido del challenge ConvAI2 (Conversational Intelligence Challenge 2). El proceso de entrenamiento del modelo incluye los siguientes pasos: Se realiza un preprocesamiento de las conversaciones para obtener las secuencias de entrada y salida necesarias para el entrenamiento del modelo, se utilizan embeddings pre-entrenados de Glove para transformar los tokens de entrada en vectores, se entrena el modelo utilizando la arquitectura encoder-decoder. Durante el entrenamiento, se optimizan los hiperparámetros como el tamaño máximo del vocabulario, la longitud máxima de las secuencias, el número de unidades LSTM, entre otros. Una vez entrenado el modelo, se puede utilizar para responder preguntas del usuario. Se realiza la inferencia por separado utilizando los modelos de encoder y decoder.

* [Resolución del desafío 5](https://github.com/aledp/ceia_PNL_aledp/blob/main/Resolucion_Desafio_5_AlejandraDelPorto.ipynb)
Se abordó la construcción de un modelo para el análisis de sentimientos utilizando BERT como codificador para un conjunto de datos de reseñas de aplicaciones. Se utilizó TensorFlow, Transformers (para acceder a modelos pre-entrenados de BERT y realizar el procesamiento del lenguaje natural), se entrenaron diversos modelos y se evaluó su desempeño utilizando el F1-score en un conjunto de datos de prueba.
