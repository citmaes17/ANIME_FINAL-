# 🎯 Análisis Ejecutivo: Anime Dataset

**Autor:** [Tu Nombre]  
**Fecha:** Octubre 2025  
**Tiempo de lectura:** 3 minutos  

---

## 📊 Resumen

Análisis de **15,000 anime** de MyAnimeList para identificar qué factores (formato y género) influyen en las calificaciones de usuarios.

**Hallazgo principal:** Las series TV superan a las películas en calidad (+0.25 puntos promedio) y concentran el 73% de los anime excepcionales.

---

## 🎯 Preguntas Investigadas

1. ¿El formato (TV/Movie/OVA) afecta las calificaciones? → **SÍ**
2. ¿Qué géneros obtienen mejores scores? → **Misterio/Terror y Drama**
3. ¿Las combinaciones formato×género importan? → **SÍ, efecto sinérgico**
4. ¿Qué caracteriza a los masterpieces? → **TV + géneros emocionales**

---

## 📈 Hallazgos Clave

### 1️⃣ TV domina en calidad y excelencia

- **Score promedio:** TV (6.87) > Movie (6.62) > OVA (6.35)
- **Masterpieces:** 73% son series TV (solo 0.1% del dataset alcanza score ≥ 8.94)
- **Razón:** Permite mejor desarrollo narrativo y de personajes

### 2️⃣ Trade-off entre volumen y calidad

- **Alto volumen:** Acción/Aventura (30% del mercado)
- **Alta calidad:** Misterio/Terror (score promedio más alto)
- **Insight:** Popularidad ≠ calidad necesariamente

### 3️⃣ Las combinaciones importan

- **Mejores:** TV + Misterio, Movie + Fantástico
- **Evitar:** OVA/ONA + géneros adultos (score < 6.3)
- **Efecto:** No es aditivo, es sinérgico

### 4️⃣ La audiencia importa

- Correlación positiva: members (0.42), scored_by (0.38)
- Mayor audiencia → mejores scores
- Posible sesgo de selección (títulos populares)

---

## 💡 Recomendaciones

### Para Productores:

**Alta Prioridad:**
- ✅ Producir **series TV** (mayor potencial)
- ✅ Combinar TV con **Misterio/Terror** o **Drama**
- ✅ Invertir en marketing (aumentar members)

**Evitar:**
- ❌ OVA/ONA para géneros que requieren desarrollo
- ❌ Apostar por cantidad sin calidad

### Para Analistas:

**Próximos pasos:**
1. Análisis temporal (tendencias por año)
2. Modelado predictivo (Random Forest/XGBoost)
3. NLP en sinopsis (palabras que correlacionan con alto score)
4. Clustering de audiencias

---

## 🔍 Metodología

- **Dataset:** 15,000 anime (top por members)
- **Fuente:** MyAnimeList via Kaggle
- **Período:** 1917-2024
- **Limpieza:** Eliminadas columnas con >20% nulos, imputación con mediana/moda
- **Categorización:** 43 géneros → 6 categorías temáticas
- **Outliers:** Método IQR (Q3 + 1.5×IQR)

---

## 📊 Variables Clave

| Variable | Impacto | Correlación |
|----------|---------|-------------|
| Type (formato) | **Alto** | Diferencias de +0.5 puntos |
| Categoría género | **Moderado** | Consistente entre tipos |
| Members | **Moderado** | +0.42 con score |
| Scored_by | **Moderado** | +0.38 con score |
| Episodios | **Bajo** | +0.05 con score |

---

## 📁 Archivos del Proyecto

### Para Reclutadores (inicio aquí):
- **[anime_eda_ejecutivo.ipynb](../notebooks/anime_eda_ejecutivo.ipynb)** ⭐ - Notebook completo (5-7 min)
- **ANALYSIS_EXECUTIVE.md** (este archivo) - Resumen sin código (3 min)

### Para Análisis Detallado:
- **[anime_eda_complete_static.ipynb](../notebooks/anime_eda_complete_static.ipynb)** - Metodología completa
- **[ANALYSIS_STATIC.md](ANALYSIS_STATIC.md)** - Documentación extensa

### Visualizaciones:
- 12 gráficas PNG en [/images](../images/)

---

## 🛠️ Tecnologías

- Python 3.11+ (Pandas, NumPy, Plotly, SciPy)
- Jupyter Notebook
- Análisis estadístico: IQR, correlaciones, distribuciones

---

## 👤 Contacto

**[Tu Nombre]**

- 🔗 LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)
- 💻 GitHub: [@tu-usuario](https://github.com/tu-usuario)
- 📧 Email: tu.email@ejemplo.com

---

## 🎓 Habilidades Demostradas

- ✅ Análisis Exploratorio de Datos (EDA)
- ✅ Limpieza y preprocesamiento
- ✅ Visualización de datos
- ✅ Pensamiento estadístico
- ✅ Business Intelligence
- ✅ Storytelling con datos

---

**📊 Última actualización:** Octubre 2025  
**⏱️ Tiempo invertido:** ~8 horas de análisis  
**🎯 Orientado a:** Reclutadores y Data Scientists
