# 📊 Análisis de Robos en la República Dominicana (2024–2025)

## 📌 Descripción del Proyecto
Este proyecto presenta un análisis estadístico de los robos generales registrados en la República Dominicana durante el período 2024–2025, utilizando datos oficiales del Ministerio de Interior y Policía (MIP).

El objetivo principal es identificar patrones geográficos y temporales en la incidencia delictiva, permitiendo generar insights que apoyen la toma de decisiones en materia de seguridad ciudadana.

---

## 🎯 Objetivos

- Analizar la distribución de robos por provincia
- Identificar patrones temporales (mensuales)
- Detectar valores atípicos (outliers)
- Simplificar categorías de robo para facilitar el análisis
- Generar recomendaciones basadas en datos

---

## 🗂️ Fuente de Datos

- Base de datos oficial del Ministerio de Interior y Policía (MIP)
- Período original: **2018 – 2026**
- Hoja utilizada: `ROBOS_GENERALES`
- Variables principales:
  - Tipo de robo
  - Provincia
  - Mes
  - Año
  - Cantidad de denuncias

---

## ⚙️ Metodología

### 🔹 1. Limpieza de Datos

Se aplicaron los siguientes procesos:

- **Estandarización de meses**
  - Conversión a mayúsculas
  - Creación de variable numérica (`MESES_NUM`) para orden cronológico

- **Manejo de valores faltantes**
  - Identificación de valores `#N/D`
  - Reemplazo por `"Desconocido"` sin eliminar registros

- **Detección de duplicados**
  - Validación de consistencia en todas las columnas

---

### 🔹 2. Normalización de Variables

Se redujeron 8 categorías originales de robos a 3 categorías principales:

| Categoría Original | Categoría Consolidada |
|------------------|---------------------|
| Arrebato / Asalto | Robo directo |
| Robo Simple / Agravado | Robo general |
| Roturas (residencia, negocio, vehículo) | Robo por rotura |

---

## 📊 Análisis Realizados

### 📍 1. Distribución Geográfica

- **Santo Domingo** lidera con ~52,000 robos
- **Santiago**: ~22,000 robos
- **Distrito Nacional**: ~14,000 robos

📌 Insight:
> Alta concentración delictiva en zonas urbanas y económicamente activas

---

### 📦 2. Análisis de Outliers

- **Robo general**
  - Mayor dispersión
  - Máximo: ~1,429 casos
- **Robo directo**
  - Menor dispersión, pero con picos (~920)
- **Robo por rotura**
  - Más estable (máx ~360)

📌 Insight:
> Existen zonas o períodos con comportamiento anómalo que requieren atención específica.

---

### 📅 3. Análisis Temporal (Mensual)

- 2024 presenta más robos que 2025
- Picos en:
  - Enero
  - Marzo
- Caída en 2025:
  - Junio → Septiembre (~5,500 casos)

📌 Insight:
> Existe estacionalidad clara en los robos

---

## 📈 Principales Hallazgos

- Alta concentración en:
  - Santo Domingo
  - Santiago
  - Distrito Nacional
- El tipo de robo más variable es:
  - **Robo general**
- Estacionalidad marcada:
  - Picos en enero y marzo
- Tendencia:
  - Disminución en 2025 (requiere validación completa)

---

## 💡 Recomendaciones

- Distribuir recursos de seguridad estratégicamente
- Priorizar zonas urbanas de alta densidad
- Reforzar operativos en meses críticos:
  - Enero
  - Marzo
- Incorporar variables adicionales en futuros análisis:
  - Factores económicos
  - Movilidad
  - Eventos sociales

---

## 🛠️ Herramientas Utilizadas

- Excel (limpieza y transformación de datos)
- Análisis estadístico descriptivo
- Visualización de datos:
  - Gráficos de barras
  - Boxplots
  - Series temporales

---

## 📁 Estructura del Proyecto
