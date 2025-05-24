# Trabajo Final - Herramientas de Inteligencia Artificial

## 1. Introducción
Este proyecto tiene como objetivo implementar un sistema que permita identificar, a partir de una observación escrita, qué Norma de Control Interno (NCI) podría estar siendo incumplida. Utiliza modelos de lenguaje natural para calcular la similitud semántica entre la observación y las descripciones de las NCI.

## 2. Marco teórico de las tecnologías/librerías usadas
- **Google Colab**: plataforma colaborativa para la ejecución de notebooks.
- **Pandas**: manipulación de datos tabulares.
- **SQLAlchemy**: conexión a base de datos PostgreSQL.
- **Sentence-Transformers**: modelos de lenguaje preentrenados para cálculo de similitud semántica.
- **Matplotlib**: visualización de datos en gráficos.
- **Render.com**: hosting gratuito de base de datos PostgreSQL.

## 3. Descripción del dataset usado
- **nci_titulos.sql**: contiene los títulos y códigos de las Normas de Control Interno (NCI), almacenados en PostgreSQL.
- **nci_descripciones.csv**: contiene las descripciones completas de cada NCI.
- Ambos datasets son combinados en el notebook para analizar y visualizar resultados.

## 4. Descripción de los pasos realizados en el proyecto
1. Instalación de librerías necesarias
2. Carga del dataset en CSV
3. Conexión a la base de datos PostgreSQL
4. Combinación de datos con Pandas
5. Ingreso de observación desde pantalla
6. Cálculo de similitud semántica con modelo `sentence-transformers`
7. Visualización de resultados en un gráfico de barras horizontales

### 4.1. Breve descripción de las visualizaciones generadas
Se genera una visualización que muestra las 5 normas más similares a la observación ingresada, junto con su nivel de similitud.

## 5. Conclusiones
“Aunque el modelo muestra similitudes algo bajas en algunos casos, se debe a la brevedad de la observación y la diferencia entre lenguaje natural y normativo. Sin embargo, el sistema funciona correctamente y sería factible mejorar el rendimiento semántico aplicando técnicas de expansión léxica, clasificación temática o fine-tuning en etapas futuras.”

## 6. Bibliografía
- [Sentence Transformers - HuggingFace](https://www.sbert.net/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [SQLAlchemy Documentation](https://docs.sqlalchemy.org/)
- [Render PostgreSQL](https://render.com/docs/databases)
