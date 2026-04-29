Social Media Stress Detection (NLP)

Este proyecto implementa un modelo de Inteligencia Artificial capaz de clasificar textos de redes sociales (Reddit) para detectar niveles de estrés en los usuarios. Fue desarrollado como parte de la Diplomatura en Programación de IA (IFES).  

Resumen Técnico / Technical Overview
Español
Objetivo: Identificar indicadores de estrés en mensajes relacionados con salud mental.  
Modelo: Clasificador probabilístico Bernoulli Naive Bayes.  
Procesamiento de Datos: * Traducción automatizada del inglés al español mediante deep-translator con ejecución en paralelo.  Limpieza de texto (Regex) para eliminar URLs, puntuación y números.  
Eliminación de stopwords y normalización con la librería NLTK.  
Resultados: El modelo permite predecir la presencia de estrés en frases nuevas ingresadas por el usuario.

English
Objective: Identify stress indicators in mental health-related social media posts.  
Model: Bernoulli Naive Bayes probabilistic classifier.  
Data Processing:Automated English-to-Spanish translation using deep-translator with parallel execution.  
Text cleaning (Regex) to remove URLs, punctuation, and numbers.  
Stopword removal and normalization using the NLTK library.  

Tecnologías / Tech 
StackLenguaje: Python   
Librerías: Pandas, Numpy, Scikit-learn, NLTK, Matplotlib, WordCloud   

Estructura del Repositoriodeteccion-de-estres.ipynb: 
Notebook principal con el flujo de datos y modelo.  
Data/stress_spanish.csv: Dataset procesado y traducido para ejecución inmediata.  
