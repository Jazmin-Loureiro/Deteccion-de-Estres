# 🧠 Detector de Estrés (NLP)

Este proyecto implementa un modelo de **Inteligencia Artificial** basado en Procesamiento de Lenguaje Natural (NLP) capaz de clasificar textos de redes sociales para detectar niveles de estrés. 

Desarrollado como proyecto para la **Diplomatura en Programación de IA (IFES)**.

---

## 🚀 Resumen Técnico / Technical Overview

### 🇦🇷 Español
* **Objetivo:** Identificar indicadores de estrés en mensajes relacionados con salud mental extraídos de Reddit.
* **Modelo:** Clasificador probabilístico **Bernoulli Naive Bayes**.
* **Procesamiento de Datos:** Traducción automatizada (Inglés -> Español) mediante `deep-translator` con ejecución en paralelo (`ThreadPoolExecutor`).
    * Limpieza de texto profunda usando **Regex** (eliminación de URLs, puntuación y números).
    * Normalización y eliminación de *stopwords* con la librería **NLTK**.
* **Resultados:** El modelo permite predecir la presencia de estrés en frases nuevas ingresadas por el usuario con un alto grado de coherencia.

### 🇺🇸 English
* **Objective:** Identify stress indicators in mental health-related social media posts from Reddit.
* **Model:** **Bernoulli Naive Bayes** probabilistic classifier.
* **Data Processing:**
    * Automated English-to-Spanish translation using `deep-translator` with parallel execution.
    * Deep text cleaning using **Regex** (removal of URLs, punctuation, and numbers).
    * Stopword removal and normalization using the **NLTK** library.

---



## 🛠️ Tecnologías / Tech Stack
* **Lenguaje:** ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
* **Librerías principales:** `Pandas` & `Numpy` (Manipulación de datos)
    * `Scikit-learn` (Machine Learning & Vectorización)
    * `NLTK` (Procesamiento de lenguaje)
    * `Matplotlib` & `WordCloud` (Visualización de datos)

---

## 📂 Estructura del Repositorio
* `deteccion-de-estres.ipynb`: Notebook principal que contiene todo el flujo de trabajo: carga, traducción, limpieza, entrenamiento y pruebas.
* **`Data/`**:
    * `stress.csv`: Dataset original en inglés.
    * `stress_spanish.csv`: Dataset ya procesado y traducido (incluido para permitir una ejecución inmediata sin tiempos de espera).

---

## 💻 Instalación y Uso
1. Clona el repositorio.
2. Asegúrate de tener instaladas las dependencias:
   ```bash
   pip install pandas numpy scikit-learn nltk deep-translator matplotlib wordcloud