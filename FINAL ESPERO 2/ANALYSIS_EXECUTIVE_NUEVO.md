# 🎬 Análisis de Anime: Resumen Ejecutivo

**Dataset:** 15,000 anime de MyAnimeList  
**Período:** 1917-2024  
**Tiempo de lectura:** 3 minutos  

---

## 🎯 Objetivo

Identificar qué combinaciones de **formato** (TV/Movie/OVA) y **género** maximizan las calificaciones de usuarios en MyAnimeList.

---

## 📊 Hallazgos Principales

### 1️⃣ TV domina en calidad y excelencia

- **Score promedio:** TV (6.87) > Movie (6.62) > OVA (6.35)  
- **Masterpieces:** 73% de anime excepcionales (score ≥ 8.94) son series TV  
- **Conclusión:** El formato TV permite mejor desarrollo narrativo

### 2️⃣ Misterio/Terror es el género premium

- Mejor score promedio de todas las categorías  
- Funciona bien en TV y Movies  
- Solo 5% del mercado pero máxima calidad

### 3️⃣ Las combinaciones importan (efecto sinérgico)

- **Mejores:** TV + Misterio, Movie + Fantástico  
- **Evitar:** OVA/ONA + géneros adultos (score < 6.3)  
- No es efecto aditivo: la combinación multiplica el impacto

### 4️⃣ La audiencia influye positivamente

- Correlación: members (0.42), scored_by (0.38)  
- Mayor audiencia → mejores scores  
- Invertir en marketing ayuda

---

## 💡 Recomendaciones

### Para Productores:

**✅ Alta Prioridad:**
- Producir series TV (mayor potencial de excelencia)
- Combinar TV con Misterio/Terror o Drama
- Invertir en marketing para aumentar audiencia

**❌ Evitar:**
- OVA/ONA para géneros que requieren desarrollo narrativo
- Apostar por cantidad sin calidad

### Para Analistas:

**Próximos pasos sugeridos:**
1. Análisis temporal (evolución de preferencias por año)
2. Modelado predictivo (Random Forest, XGBoost)
3. NLP en sinopsis (palabras correlacionadas con alto score)
4. Clustering de audiencias

---

## 🔍 Metodología

- **Datos:** 15,000 anime (top por members)
- **Fuente:** MyAnimeList via Kaggle
- **Limpieza:** Eliminadas columnas con >20% nulos, imputación con mediana/moda
- **Categorización:** 43 géneros → 6 categorías temáticas
- **Outliers:** Método IQR (Q3 + 1.5×IQR)
- **Herramientas:** Python (Pandas, NumPy, Plotly, SciPy)

---

## 📈 Variables de Mayor Influencia

| Variable | Impacto | Notas |
|----------|---------|-------|
| Type (formato) | **Alto** | Diferencias de +0.5 puntos |
| Categoría género | **Moderado** | Consistente entre tipos |
| Members | **Moderado** | Corr: +0.42 |
| Scored_by | **Moderado** | Corr: +0.38 |
| Episodios | **Bajo** | Corr: +0.05 |

---

## 📁 Archivos del Proyecto

- **[anime_eda_ejecutivo.ipynb](../notebooks/anime_eda_ejecutivo.ipynb)** ⭐ - Notebook completo (5-7 min)
- **ANALYSIS_EXECUTIVE.md** (este archivo) - Resumen sin código (3 min)
- **[Visualizaciones](../images/)** - 12 gráficas PNG

---

## 🎓 Habilidades Demostradas

- ✅ Análisis Exploratorio de Datos (EDA completo)
- ✅ Limpieza y preprocesamiento
- ✅ Visualización de datos (12 gráficas profesionales)
- ✅ Pensamiento estadístico (correlaciones, outliers, IQR)
- ✅ Business Intelligence (recomendaciones accionables)
- ✅ Storytelling con datos

---

## 👤 Contacto

**[Tu Nombre]**

- 🔗 LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)
- 💻 GitHub: [@tu-usuario](https://github.com/tu-usuario)  
- 📧 Email: tu.email@ejemplo.com

---

**📊 Última actualización:** Octubre 2025  
**⏱️ Tiempo invertido:** ~8 horas de análisis  
**🎯 Para:** Reclutadores y Data Scientists
