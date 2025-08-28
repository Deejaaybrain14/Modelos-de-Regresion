# 🚗 Proyecto Final — Regresión con mtcars

Este proyecto corresponde al trabajo final del curso **Regression Models** (Data Science Specialization, Johns Hopkins / Coursera).

## 📌 Objetivo
Explorar si los autos con transmisión **manual** (`am = 1`) tienen mejor rendimiento de combustible (`mpg`) que los **automáticos** (`am = 0`) y cuantificar la diferencia, usando el dataset clásico **mtcars**.

## 🛠️ Metodología
- **Exploratory Data Analysis (EDA):** boxplots de `mpg` según tipo de transmisión.  
- **Modelos de regresión lineal:**
  - Modelo crudo: `mpg ~ am`
  - Modelo ajustado: `mpg ~ am + wt`
  - Modelo extendido: `mpg ~ am + wt + cyl`
- **Diagnósticos:** gráficos de residuos y comprobación de supuestos.  
- **Inferencia:** estimación de intervalos de confianza e interpretación de coeficientes.

## 📊 Resultados
- Los autos **manuales** presentan un promedio de **+7.2 mpg** frente a los automáticos (modelo crudo).  
- Ajustando por **peso**, la ventaja se reduce a **+3 mpg** (IC95% ≈ 0–6).  
- Con más covariables (`wt + cyl`), el efecto se mantiene positivo pero con menor precisión.  
- Los diagnósticos no muestran violaciones serias de los supuestos de regresión.

## ⚠️ Limitaciones
- Tamaño muestral pequeño (32 autos).  
- Dataset antiguo (1974), no refleja autos actuales.  
- Posibles confusores no incluidos (potencia `hp`, engranajes `gear`, carburadores `carb`).  

## ✅ Conclusión
La transmisión **manual** ofrece una ventaja en eficiencia de combustible, especialmente al comparar vehículos de peso similar.

---

## 📂 Archivos
- `Regresion-Models.Rmd` → código en R Markdown.  
- `Modelos.pdf` → reporte final en PDF (knit desde Rmd).

---

✍️ *Autora: Bea Herrera*  
