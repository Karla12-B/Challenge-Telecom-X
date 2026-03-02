# 📊 Proyecto: Análisis de Evasión de Clientes (Churn) - Telecom X

Este repositorio contiene un análisis exhaustivo de ciencia de datos aplicado a la retención de clientes. A través de un pipeline **ETL** (Extracción, Transformación y Carga), identificamos los factores críticos que llevan a los usuarios a cancelar sus servicios.



## 🎯 Objetivo del Proyecto
El objetivo principal es reducir la tasa de **Churn** (evasión) de Telecom X mediante el análisis de patrones de comportamiento, demografía y servicios contratados.

## 🛠️ Fases del Desarrollo

### 1. Extracción y Limpieza (E & T)
* **Normalización:** Uso de `json_normalize` para aplanar estructuras JSON anidadas.
* **Depuración:** Tratamiento de 11 valores nulos en cargos totales y eliminación de duplicados.
* **Estandarización:** Traducción de variables clave al español y binarización de la variable `Evasion` (Yes=1, No=0).
* **Ingeniería de Variables:** Creación de la métrica `Gasto_Diario` para un análisis más granular.

### 2. Análisis Exploratorio (EDA)
* **Análisis Descriptivo:** Cálculo de medias, medianas y desviaciones estándar para entender la distribución de gastos.
* **Segmentación:** Evaluación de la evasión por tipo de contrato, género y métodos de pago.
* **Comportamiento Numérico:** Análisis de densidad para identificar el "mes crítico" de abandono.



### 3. Análisis de Correlación (Opcional/Extra)
* Cálculo de la matriz de correlación para identificar la relación entre la cantidad de servicios contratados y la lealtad del cliente.

## 📈 Hallazgos Principales (Insights)
1. **Contratos:** Los clientes con contrato "mes a mes" son los más propensos a la evasión.
2. **Antigüedad:** El riesgo de pérdida es crítico durante los primeros **12 meses**.
3. **Servicios:** Existe una correlación negativa entre el número de servicios (TV, Seguridad, etc.) y la evasión; a mayor ecosistema de servicios, mayor retención.

## 💻 Requisitos
Para ejecutar este notebook necesitas:
* `pandas`
* `requests`
* `matplotlib`
* `seaborn`
* `numpy`

```python
# Instalación rápida
pip install pandas requests matplotlib seaborn numpy


