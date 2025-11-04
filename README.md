# Airbnb-Investment-Calculator-DS
Sistema predictivo de precios para alquileres de Airbnb en Nueva York, utilizando Python, Scikit-Learn y RandomForest.
Este proyecto analiza más de 100,000 registros para construir un modelo `RandomForestRegressor` que no solo estima precios, sino que también identifica las propiedades subvaluadas y las oportunidades de mercado.

---

### 🚀 El Modelo en Acción: Casos de Uso Prácticos

El verdadero valor de este modelo es su aplicación en el mundo real. Aquí hay dos simulaciones que demuestran su impacto:

#### 💼 Caso 1: Asesor para Anfitriones (Detectando Oportunidades)
Un anfitrión tiene un apartamento cerca de Central Park listado a un precio bajo para atraer reservas rápidas.

| Descripción | Valor |
| :--- | :--- |
| **Precio Actual** | **$55.00** / noche |
| **Precio Sugerido por el Modelo** | **$538.82** / noche |
| **Oportunidad Detectada** | **+$483.82 (+879.7%)** |

> **Insight:** El modelo detecta que la propiedad está severamente subvaluada. Al ajustar el precio, el anfitrión podría incrementar sus ingresos potenciales en más de **$14,000 al mes**.

#### 🏡 Caso 2: Asesor para Huéspedes (Validando Ofertas)
Un huésped encuentra una oferta que parece "demasiado buena para ser verdad" en Brooklyn.

| Descripción | Valor |
| :--- | :--- |
| **Precio Listado** | **$60.00** / noche |
| **Valor de Mercado Estimado** | **$593.80** / noche |
| **Análisis del Modelo** | **-$533.80 (-89.9%)** |

> **Insight:** El modelo confirma que es una oferta excepcional, casi un 90% por debajo de su valor de mercado. Esto le da al huésped la confianza para reservar inmediatamente.

---

### 📂 El Proyecto Completo: Elige tu Camino

Este `README` es solo la superficie. Para explorar el proyecto a fondo, tienes dos opciones:

| Documento | Audiencia | Propósito |
| :--- | :--- | :--- |
| ➡️ **[Ver el Dosier Ejecutivo (PDF)](./airbnb-investment-dossier.pdf)** | Reclutadores, Managers, Audiencia no técnica | Un resumen visual y de negocio de los hallazgos, el impacto y las conclusiones. |
| ➡️ **[Explorar el Notebook Técnico (`.ipynb`)](./airbnb-investment-calculator.ipynb)** | Data Scientists, Líderes Técnicos | El análisis completo, con todo el código, la metodología detallada y cada paso de la construcción del modelo. |

---

### 🎯 Resultados y Métricas Clave

| Métrica | Valor | Descripción |
| :--- | :--- | :--- |
| **R² (Test Set)** | **0.346** | El modelo explica el 34.6% de la variabilidad del precio. |
| **RMSE** | **$269.43** | En promedio, el error de predicción del modelo es de ~$269 por noche. |
| **Mejora vs. Baseline** | **-19.1%** | Reducción del error en un 19.1% comparado con una Regresión Lineal. |
| **OOB Score** | **0.3394** | Similar al R² del test, confirmando que el modelo no sufre de overfitting. |
