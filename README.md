# Trabajo Práctico de Procesamiento de Lenguaje Natural

![Project Image](path/to/project/image.png)

## Tabla de contenidos
- [Project Description](#project-description)
- [Installation](#installation)
- [Usage](#usage)


## Descripción de Proyecto

Este repositorio contiene el código y los recursos utilizados para el Trabajo Práctico de Procesamiento de Lenguaje Natural en el contexto de la Especialización en IA de la UBA. El trabajo práctico se centra en diversas técnicas y aplicaciones del procesamiento de lenguaje natural, como modelos de vectores de palabras, chatbots, análisis de sentimiento y más.

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/Oks11111/NLP_TP.git
   
## Uso
A continuación, se describen brevemente los cuadernos de Jupyter disponibles en este proyecto:

### 
1a - word2vec.ipynb
Descripción: 
El código proporcionado realiza las siguientes funciones:

obtener_vocabulario(corpus): Esta función toma un corpus de texto y devuelve una lista con todos los términos únicos presentes en el corpus. Utiliza un enfoque de "bolsa de palabras" para extraer los términos de cada documento del corpus.

texto_a_matriz_frecuencia(corpus, vocabulario): Esta función toma un corpus de texto y un vocabulario y devuelve una matriz de frecuencia de términos. Cada fila de la matriz representa un documento del corpus, y cada columna representa un término del vocabulario. La matriz contiene las frecuencias de los términos en cada documento.

texto_a_matriz_onehot(corpus, vocabulario): Esta función toma un corpus de texto y un vocabulario y devuelve una matriz codificada en one-hot. Al igual que la función anterior, cada fila de la matriz representa un documento del corpus y cada columna representa un término del vocabulario. Si un término está presente en un documento, se coloca un 1 en la matriz; de lo contrario, se coloca un 0.

calcular_idf(corpus, vocabulario): Esta función calcula el valor IDF (Inverse Document Frequency) para cada término del vocabulario en el corpus dado. El IDF es una medida de la importancia de un término en el corpus. Se utiliza el logaritmo natural y se realiza una suavización aditiva para evitar divisiones por cero.

texto_a_matriz_tfidf(corpus, vocabulario): Esta función combina las matrices de frecuencia de términos y los valores IDF para calcular la matriz TF-IDF (Term Frequency-Inverse Document Frequency). La matriz resultante representa la importancia de cada término en cada documento del corpus.

cosine_similarity(a, b): Esta función calcula la similitud del coseno entre dos vectores utilizando el producto escalar y las normas de los vectores.

ordenar_por_similitud_coseno(corpus, indice_documento): Esta función toma un corpus de texto y un índice de documento y ordena los documentos del corpus en función de su similitud de coseno con el documento dado. Utiliza la matriz TF-IDF y la función cosine_similarity para calcular las similitudes de coseno. Devuelve una lista de tuplas, donde cada tupla contiene el índice de un documento y su similitud de coseno con el documento dado.

El código proporcionado aplica estas funciones al corpus de ejemplo corpus y muestra los documentos ordenados por similitud de coseno con el documento en el índice 1 (segundo documento del corpus).

2c_bot_tfidf_nltk1.ipynb
Descripción: En este cuaderno de Jupyter, se implementa un chatbot utilizando el enfoque TF-IDF para la recuperación de información. Se utiliza la biblioteca NLTK para el procesamiento de texto y se crea un modelo simple de preguntas y respuestas.

3b_Custom_embedding_con_Gensim.ipynb
Descripción: En este cuaderno de Jupyter, se muestra cómo entrenar y utilizar embeddings personalizados utilizando la biblioteca Gensim. Se explora la creación de vectores de palabras a partir de un corpus de texto específico y se utilizan estos embeddings para tareas de clasificación de texto.

4d_predicción_palabra.ipynb
Descripción: En este cuaderno de Jupyter, se implementa un modelo de predicción de palabras utilizando una red neuronal recurrente (RNN). Se entrena el modelo con un corpus de texto y se evalúa su capacidad para predecir la siguiente palabra en una secuencia de texto.

5_clothing_ecommerce_reviews.ipynb
Descripción: Este cuaderno de Jupyter presenta un análisis de sentimiento de reseñas de productos de comercio electrónico de ropa. Se utilizan técnicas de procesamiento de texto y se entrena un modelo de aprendizaje

6_bot_qa.ipynb
Descripción: En este cuaderno de Jupyter, se desarrolla un chatbot de preguntas y respuestas utilizando técnicas de procesamiento de lenguaje natural. Se implementa un modelo de procesamiento de lenguaje natural basado en transformers para responder preguntas basadas en un corpus de texto previamente procesado.

