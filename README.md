# RAG Tourism Destination Recommender

Sistema de recomendación de destinos turísticos europeos basado en **Retrieval-Augmented Generation (RAG)**, desarrollado como trabajo práctico para la materia **Inteligencia Artificial** de la carrera Ingeniería en Sistemas de Información.

## Objetivo
Diseñar e implementar un sistema inteligente capaz de recomendar destinos turísticos en Europa a partir de consultas en lenguaje natural, combinando recuperación de información y generación de texto mediante modelos de lenguaje.

## Descripción del sistema
El sistema utiliza un enfoque RAG, donde:
1. Se recupera información relevante desde una base de datos vectorial.
2. Se utiliza un modelo de lenguaje para generar recomendaciones contextualizadas y coherentes.

## Tecnologías utilizadas
- Python
- LangChain
- LLaMA 3 (Groq)
- HuggingFace Embeddings
- ChromaDB
- Google Colab

## Arquitectura
- **Embeddings**: generación de representaciones vectoriales de destinos turísticos.
- **Vector Store**: almacenamiento y búsqueda semántica con ChromaDB.
- **Retriever**: recuperación de documentos relevantes según la consulta del usuario.
- **LLM**: generación de recomendaciones personalizadas utilizando LLaMA 3.

## Dataset
- Información de destinos turísticos europeos.
- Datos preprocesados y vectorizados para permitir búsqueda semántica.

## Flujo de funcionamiento
1. El usuario realiza una consulta en lenguaje natural.
2. El sistema recupera destinos relevantes desde la base vectorial.
3. El modelo LLM genera una recomendación basada en la información recuperada.

## Configuración de la API Key

Para ejecutar el proyecto es necesario contar con una API Key de Groq.

1. Obtener una API key gratuita en: https://console.groq.com
2. Configurar la variable de entorno antes de ejecutar el notebook:

```python
import os
os.environ["GROQ_API_KEY"] = "TU_API_KEY"
