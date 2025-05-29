
# 🛒 Predicción de Demanda en E-Commerce

## Acerca del Dataset

Este dataset contiene datos sintéticos de ventas de comercio electrónico con 2,000 registros únicos, diseñados para predecir los niveles de demanda (alta/baja) de productos. Incluye diversas características como el precio del producto, descuentos promocionales, niveles de inventario, condiciones climáticas e historial de ventas, con el objetivo de predecir la variable objetivo, que es una clasificación binaria de la demanda (alta o baja).

Cada registro representa una transacción o escenario único de comercio electrónico con factores relevantes de ventas y del entorno. El dataset está diseñado para apoyar el análisis de factores que afectan la demanda de productos y la eficiencia de la cadena de suministro.

## Objetivo del Proyecto

Desarrollar un modelo de Machine Learning que prediga si la demanda de un producto será **alta o baja**, utilizando un conjunto de datos sintéticos con características de ventas, inventario, promociones y factores externos.


## Flujo de Trabajo

### 1. Exploración del Dataset

* Dataset con **2,000 registros** de transacciones simuladas.
* Variables incluyen precio, descuentos, promociones, clima, inventario, ventas previas, etc.
* La variable objetivo (`target`) es binaria: **1 = alta demanda**, **0 = baja demanda**.

### 2. Limpieza y Preprocesamiento

* No se encontraron valores nulos ni duplicados.
* Se estandarizaron los nombres de columnas (`snake_case`).
* Todas las variables estaban **normalizadas entre 0 y 1**, lo que facilitó el modelado.

### 3. Análisis Exploratorio

* Se analizó la distribución de la demanda: solo **10.3%** de los casos tienen alta demanda.
* Se identificaron variables clave:

  * **Precio bajo** y **ventas altas del día anterior** favorecen la demanda alta.
  * Se identificó cierta **estacionalidad** (relacionada a una semana del año).
  * Se observó que **inventario suficiente también es relevante**.

### 4. Modelado Predictivo

* División de datos: **75% entrenamiento / 25% prueba** con `stratify` para balance de clases.
* Se aplicó **SMOTE** para balancear el conjunto de entrenamiento debido al desbalance de clases en `target`.
* Modelos entrenados:

  * **Logistic Regression** (modelo base interpretable)
  * **Random Forest** (modelo más robusto y preciso)
  * **DummyClassifier** como referencia.

### 5. Evaluación de Modelos

* Métricas utilizadas:

  * **AUC-ROC** (principal)
  * **F1-Score** y **matriz de confusión**.
* El modelo **Random Forest** superó a los demás en capacidad para detectar correctamente los casos de alta demanda.



##  Conclusiones Clave

* El modelo es útil para **anticipar escenarios de alta demanda** y tomar decisiones sobre inventario, precios y promociones.
* Variables más influyentes: **precio**, **ventas previas**, **stock disponible** y **estacionalidad**.
* Este proyecto demuestra habilidades en análisis de datos, manejo de desbalance, selección de modelos y evaluación con métricas relevantes para negocio.

