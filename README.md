# KMeans_Segmentacion_Clientes
Implementación de algorítmo no supervisado KMeans para segmentación de clientes

#  Segmentación de Clientes con K-means  
### *Mall Customers Dataset — Machine Learning No Supervisado*

Este proyecto aplica el algoritmo **K-means** para segmentar clientes de un centro comercial en grupos basados en variables demográficas y de comportamiento. Es un caso clásico de *Customer Analytics* y *Marketing Data Science*.

---

##  Dataset

El dataset utilizado es el *Mall Customers Dataset*, disponible públicamente en múltiples repositorios (como Kaggle).

Incluye las siguientes variables:

- `genero`
- `edad`
- `ingreso_anual_k`  
- `puntaje_gasto`  
- `id_cliente` (eliminado para el modelo)

---

##  Objetivo

Identificar **grupos naturales de clientes** mediante *clustering*, con el fin de:

- Comprender patrones de comportamiento.
- Identificar segmentos de alto valor.
- Proponer estrategias de marketing dirigidas.
- Visualizar la estructura interna de los clientes del centro comercial.

---

##  Tecnologías utilizadas

- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- plotly (visualizaciones 3D)

---

##  Flujo del análisis

1. **Carga y exploración del dataset (EDA)**  
   - Distribuciones de variables  
   - Boxplots  
   - Pairplot  
   - Correlaciones  
   - Análisis por género  

2. **Preprocesamiento**  
   - Renombrado de columnas a español  
   - Eliminación de `id_cliente`  
   - Selección de variables numéricas  
   - Normalización con `StandardScaler`

3. **Selección del número óptimo de clusters**  
   - Método del Codo (Elbow Method)  
   - Silhouette Score  

4. **Entrenamiento del modelo K-means**  
   - Obtención de etiquetas  
   - Cálculo de centroides  
   - Análisis de resultados  

5. **Visualizaciones profesionales**  
   - Scatter 2D:  
     - Ingreso vs Gasto  
     - Edad vs Gasto  
   - Gráfico 3D interactivo (Plotly)  
   - Visualización comparativa por cluster  

6. **Interpretación de los clusters**  
   - Perfil promedio  
   - Análisis de gasto  
   - Identificación de segmentos clave

7. **Conclusiones y posibles mejoras**

---

## Resultados principales

- Se determinaron **{k_optimo} clusters óptimos** usando Silhouette Score.
- Los clientes se organizaron en grupos bien diferenciados por ingreso, edad y gasto.
- Se identificaron segmentos como:  
  - Clientes de alto valor (alto ingreso + alto gasto)  
  - Clientes jóvenes con tendencia a mayor gasto  
  - Clientes de bajo ingreso y bajo gasto  
  - Clientes de ingreso medio con bajo puntaje de gasto  

---

