# 📋 Resumen Ejecutivo del Proyecto

## Información del Proyecto

**Título:** Anime Success Factors: Exploratory Data Analysis  
**Autor:** [Tu Nombre]  
**Fecha:** Enero 2025  
**Herramientas:** Python 3.11, Pandas, Plotly, NumPy, SciPy  

---

## 🎯 Objetivo

Analizar 15,000 anime de MyAnimeList para identificar qué factores (formato y género) influyen en las calificaciones de usuarios.

---

## 📊 Datos

- **Dataset Original:** 15,000 anime, 24 columnas
- **Fuente:** MyAnimeList (MAL)
- **Variables Clave:** 
  - Score (1-10)
  - Type (TV, Movie, OVA, ONA, etc.)
  - Genres (22 géneros originales → 6 categorías)

---

## 🔬 Metodología

### 1. Procesamiento de Datos
- Limpieza: Eliminación de nulos (>20%), duplicados
- Imputación: Media (numéricos), moda (categóricos)
- Categorización: 22 géneros → 6 categorías temáticas

### 2. Análisis Estadístico
- **Univariado:** Distribuciones, tendencia central, dispersión
- **Bivariado:** Relaciones Type-Score, Categoría-Score
- **Multivariado:** Interacciones Type × Categoría
- **Outliers:** Identificación de masterpieces (IQR)

### 3. Visualización
- 12 gráficas interactivas con Plotly
- Histogramas, boxplots, heatmaps, barras agrupadas

---

## 🔑 Hallazgos Principales

### 1️⃣ Por Formato (Type)

| Formato | Score Promedio | % del Dataset | Insight |
|---------|----------------|---------------|---------|
| **TV** | **6.91** ⭐ | 33.7% | Formato premium, mejor calificado |
| Movie | 6.71 | 16.5% | Score medio-alto |
| TV Special | 6.63 | 3.6% | Formato nicho |
| Special | 6.54 | 9.5% | Score medio |
| ONA | 6.36 | 14.7% | Formato web, score bajo |
| OVA | 6.33 | 21.8% | Direct-to-video, peor calificado |

**Conclusión:** TV supera a Movies en promedio (contraintuitivo)

---

### 2️⃣ Por Categoría de Género

| Categoría | Score Promedio | % del Dataset | Emoji |
|-----------|----------------|---------------|-------|
| **🧩 Misterio y Terror** | **7.04** ⭐ | 5.1% | Género premium |
| 🎭 Emocionales y Humanistas | 6.92 | 16.8% | Alta calidad |
| ⚔️ Acción y Aventura | 6.81 | 26.6% | Mayor volumen |
| 🔮 Fantásticos y Experimentales | 6.69 | 22.6% | Score medio-alto |
| 😂 Comedia | 6.64 | 19.6% | Score medio |
| 💞 Íntimos y Adultos | 6.41 | 9.2% | Techo estructural |

**Conclusión:** Misterio domina en calidad, Acción en volumen

---

### 3️⃣ Interacciones Type × Categoría

**Top 3 Combinaciones (Score ≥ 7.0):**
1. 🏆 Movie + Misterio y Terror: **7.11**
2. 🏆 TV + Misterio y Terror: **7.11**
3. 🏆 TV + Emocionales y Humanistas: **7.07**

**Peores 3 Combinaciones (Score < 6.3):**
1. ❌ ONA + Íntimos y Adultos: **6.26**
2. ❌ OVA + Íntimos y Adultos: **6.28**
3. ❌ OVA + Misterio y Terror: **6.35**

**Conclusión:** Las interacciones son significativas

---

### 4️⃣ Análisis de Outliers (Masterpieces)

**Criterio:** Score ≥ 8.95 (método IQR)  
**Total de Outliers:** 39 anime

**Distribución por Formato:**
- TV: **72%** (28 anime) → Domina la producción de masterpieces
- Movie: 15% (6 anime)
- OVA: 5% (2 anime)
- TV Special: 5% (2 anime)
- ONA: 2.5% (1 anime)

**Distribución por Categoría:**
- ⚔️ Acción y Aventura: 23.1%
- 🔮 Fantásticos y Experimentales: 20.5%
- 🎭 Emocionales y Humanistas: 12.8%
- 🧩 Misterio y Terror: 5.1%

**Conclusión:** TV + Acción genera más masterpieces

---

## 💡 Recomendaciones

### Para Productores (Calidad):
1. ✅ Produce **TV Series** de **Misterio y Terror**
2. ✅ Considera **Movies** de **Fantásticos**
3. ❌ Evita **OVA/ONA** para géneros premium

### Para Productores (Volumen):
1. ✅ Enfócate en **Acción y Aventura**
2. ✅ Usa formato **TV** (mayor alcance)
3. ✅ Diversifica en **Comedia**

### Para Analistas:
1. Las interacciones Type × Categoría son significativas
2. Necesario análisis confirmatorio (ANOVA)
3. Potencial para modelado predictivo

---

## 📈 Impacto

- **Volumen de Datos:** 15,000 registros analizados
- **Visualizaciones:** 12 gráficas interactivas generadas
- **Insights Accionables:** 5 recomendaciones clave
- **Datasets Procesados:** 2 archivos listos para análisis posteriores

---

## 🛠️ Tecnologías

| Tecnología | Versión | Propósito |
|------------|---------|-----------|
| Python | 3.11+ | Lenguaje principal |
| Pandas | 2.2.0 | Manipulación de datos |
| Plotly | 5.18.0 | Visualización interactiva |
| NumPy | 1.26.3 | Operaciones numéricas |
| SciPy | 1.12.0 | Análisis estadístico |
| Jupyter | 7.0.6 | Notebook interactivo |

---

## 📁 Entregables

1. ✅ Notebook Jupyter completo (`anime_eda_analysis.ipynb`)
2. ✅ Dataset limpio (`anime_clean.csv`)
3. ✅ Dataset categorizado (`anime_categorized.csv`)
4. ✅ 12 visualizaciones en formato PNG
5. ✅ README profesional con documentación completa
6. ✅ Código reproducible con requirements.txt

---

## 📝 Limitaciones

1. **Sesgo de selección:** Solo top 15,000 por cantidad de miembros
2. **Causalidad:** Análisis correlacional, no causal
3. **Temporalidad:** No considera tendencias a lo largo del tiempo
4. **Studio Effect:** No analiza el impacto del estudio productor
5. **Variables omitidas:** Presupuesto, marketing, etc.

---

## 🚀 Próximos Pasos

1. [ ] Análisis confirmatorio (Two-way ANOVA)
2. [ ] Modelado predictivo (Random Forest, XGBoost)
3. [ ] Análisis temporal (tendencias por año)
4. [ ] Studio Effect (¿qué estudios dominan?)
5. [ ] Sentiment Analysis de reseñas

---

## 📚 Referencias

- **Fuente de datos:** MyAnimeList (https://myanimelist.net/)
- **Metodología EDA:** "Python for Data Analysis" (Wes McKinney)
- **Visualización:** Plotly Documentation
- **Análisis estadístico:** SciPy Documentation

---

## 🎯 Valor para Reclutadores

### Competencias Demostradas

1. **Python Avanzado:**
   - Pandas para manipulación de datos
   - NumPy para operaciones vectorizadas
   - SciPy para análisis estadístico

2. **Visualización de Datos:**
   - 12 gráficas profesionales
   - Plotly para interactividad
   - Storytelling con datos

3. **Pensamiento Analítico:**
   - Formulación de preguntas de investigación
   - Diseño de metodología
   - Interpretación de resultados

4. **Comunicación:**
   - README profesional
   - Documentación clara
   - Conclusiones accionables

5. **Reproducibilidad:**
   - Código documentado
   - Requirements.txt
   - Estructura organizada

---

## 📧 Contacto

**Autor:** [Tu Nombre]  
**Email:** tuemail@ejemplo.com  
**GitHub:** github.com/tu-usuario  
**LinkedIn:** linkedin.com/in/tu-perfil  

---

<p align="center">
  <b>Este proyecto demuestra competencias en Data Science, Python, y Storytelling con Datos</b>
</p>
