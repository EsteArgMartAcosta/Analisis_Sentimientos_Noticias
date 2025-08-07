# Análisis de Sentimientos de Noticias Locales (Colombia)


Repositorio para un pipeline reproducible de recolección de titulares/noticias locales y análisis de sentimientos con modelos de *transformers*. Incluye un cuaderno ejecutable en Google Colab y soporte para ejecución local con Selenium/ChromeDriver.

---

## Objetivos

* Capturar titulares/noticias de fuentes locales seleccionadas.
* Evaluar el sentimiento de cada texto con un modelo multilingüe preentrenado.
* Generar salidas tabulares y visualizaciones rápidas (distribución de sentimiento, nube de palabras).
* Dejar una base sólida para extender a más fuentes, métricas y despliegues.

## Alcance actual

* **Fuentes de ejemplo:** Telegram (canal público de Boyacá 7 Días) y sección Medellín de El Tiempo.
* **NLP:** `nlptown/bert-base-multilingual-uncased-sentiment` vía `transformers.pipeline("sentiment-analysis")`.
* **Visualizaciones:** Nube de palabras y conteos por etiqueta.
* **Cuaderno:** `Analisis_Sentimientos_Noticias.ipynb` (Colab-ready).



## Requisitos

* **Python** 3.10+
* **Google Chrome** instalado (ejecución local con Selenium). En Colab no es necesario instalar Chrome manualmente.
* **Sistema operativo:** Windows, macOS o Linux.

Paquetes (mínimos):

```
selenium
webdriver-manager
pandas
transformers
wordcloud
matplotlib
```


