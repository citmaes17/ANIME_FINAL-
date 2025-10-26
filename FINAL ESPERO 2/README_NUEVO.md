# 📊 Análisis Exploratorio de Anime - MyAnimeList

![Python](https://img.shields.io/badge/python-3.11+-blue.svg)
![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?logo=plotly&logoColor=white)

## 🎯 Resumen Ejecutivo

Análisis de **15,000 anime** de MyAnimeList para identificar qué combinaciones de formato (TV/Movie/OVA) y género maximizan las calificaciones de usuarios.

**Hallazgo principal:** Las series TV superan a las películas en calidad (+0.25 puntos) y concentran el 73% de los anime excepcionales.

---

## 📂 Navegación Rápida

### ⭐ Para Reclutadores (recomendado)

**👉 [Ver Notebook Completo](notebooks/anime_eda_ejecutivo.ipynb)** (5-7 min)
- Análisis completo con visualizaciones
- Conclusiones y recomendaciones
- Todo ejecutado y renderizado

**📝 [Leer Resumen Ejecutivo](docs/ANALYSIS_EXECUTIVE.md)** (3 min)
- Solo hallazgos principales
- Sin código
- Lectura rápida

---

## 🔍 Preguntas de Investigación

1. **¿El formato afecta las calificaciones?** → Sí, TV supera a Movies (+0.25 puntos)
2. **¿Qué géneros funcionan mejor?** → Misterio/Terror lidera (mejor score)
3. **¿Existen combinaciones ganadoras?** → Sí, TV + Misterio = mejor combinación
4. **¿Qué caracteriza a los masterpieces?** → 73% son series TV

---

## 💡 Hallazgos Principales

### 1️⃣ TV es el formato premium
- ✅ Score más alto: **6.87/10**
- ✅ Genera **73% de masterpieces** (score ≥ 8.94)
- ✅ Supera a Movies por +0.25 puntos

### 2️⃣ Misterio domina en calidad
- ✅ Mejor score de todos los géneros
- ✅ Funciona bien en TV y Movies
- ✅ Solo 5% del mercado pero máxima calidad

### 3️⃣ Las combinaciones importan
- 🏆 **Top:** TV/Movie + Misterio
- ❌ **Evitar:** ONA/OVA + géneros adultos (<6.30)
- 📊 Efecto sinérgico (no aditivo)

### 4️⃣ La audiencia influye
- **Correlación positiva:** members (0.42), scored_by (0.38)
- Mayor audiencia → mejores scores
- Invertir en marketing ayuda

---

## 🛠️ Tecnologías Utilizadas

- **Python 3.11+**
- **Pandas** - Manipulación de datos
- **NumPy** - Operaciones numéricas
- **Plotly** - 12 visualizaciones profesionales
- **SciPy** - Análisis estadístico
- **Jupyter Notebook** - Desarrollo interactivo

---

## 📁 Estructura del Proyecto

```
anime-eda-analysis/
│
├── README.md                              ⭐ Estás aquí
├── requirements.txt                       📦 Dependencias
│
├── notebooks/
│   └── anime_eda_ejecutivo.ipynb         ⭐ Notebook completo
│
├── data/
│   └── anime.csv                         📊 Dataset (15,000 anime)
│
├── images/
│   ├── 01_score_distribution.png         📈 12 visualizaciones
│   ├── 02_type_distribution.png
│   └── ...
│
└── docs/
    └── ANALYSIS_EXECUTIVE.md             📝 Resumen ejecutivo
```

---

## 🚀 Instalación y Uso

### 1. Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/anime-eda-analysis.git
cd anime-eda-analysis
```

### 2. Crear entorno virtual (recomendado)
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 4. Abrir Jupyter Notebook
```bash
jupyter notebook
```

### 5. Abrir `notebooks/anime_eda_ejecutivo.ipynb`

---

## 📊 Visualizaciones Destacadas

### Distribución de Scores
![Score Distribution](images/01_score_distribution.png)

### Score por Formato
![Score by Type](images/05_score_by_type.png)

### Heatmap: Formato × Género
![Heatmap](images/09_type_category_heatmap.png)

---

## 💼 Recomendaciones de Negocio

### Para Productores - Alta Calidad:
✅ Producir **TV series** de **Misterio/Terror**  
✅ Combinar formatos largos con géneros complejos  
✅ Invertir en marketing (aumentar audiencia)  

### Para Productores - Alto Volumen:
✅ Enfocarse en **Acción/Aventura** (30% del mercado)  
✅ Usar formato **TV** (mayor alcance)  
✅ Diversificar con **Comedia** (audiencia amplia)  

---

## 📈 Metodología

1. **Carga de datos** - 15,000 anime de MyAnimeList
2. **Limpieza** - Manejo de nulos (<20% threshold) y duplicados
3. **Categorización** - 43 géneros → 6 categorías temáticas
4. **Análisis Univariado** - Distribuciones individuales
5. **Análisis Bivariado** - Relaciones tipo/categoría vs score
6. **Análisis Multivariado** - Interacciones tipo × categoría
7. **Análisis de Outliers** - Identificación de masterpieces (IQR)
8. **Conclusiones** - Hallazgos y recomendaciones

---

## 🎓 Habilidades Demostradas

- ✅ Análisis Exploratorio de Datos (EDA)
- ✅ Limpieza y preprocesamiento
- ✅ Visualización de datos (12 gráficas profesionales)
- ✅ Pensamiento estadístico
- ✅ Business Intelligence & Analytics
- ✅ Storytelling con datos
- ✅ Documentación técnica

---

## 🔗 Fuente de Datos

**Dataset:** [MyAnimeList Dataset on Kaggle](https://www.kaggle.com/)  
**Tamaño:** 15,000 anime (top por members)  
**Período:** 1917 - 2024  
**Variables:** 24 columnas (score, type, genres, members, etc.)

---

## 👤 Autor

**[Tu Nombre]**

🔗 LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)  
💼 GitHub: [@tu-usuario](https://github.com/tu-usuario)  
📧 Email: tu.email@ejemplo.com  

---

## 📜 Licencia

Este proyecto está bajo la Licencia MIT - ver [LICENSE](LICENSE) para detalles.

---

## 📌 Nota para Reclutadores

Este proyecto demuestra:

- ✅ **Análisis end-to-end** - Desde datos crudos hasta recomendaciones
- ✅ **Business acumen** - Hallazgos traducidos a acciones de negocio
- ✅ **Comunicación clara** - Notebook estructurado y resumen ejecutivo
- ✅ **Visualización profesional** - 12 gráficas con Plotly
- ✅ **Documentación completa** - README, notebook comentado, resumen

**Tiempo de revisión:** 5-7 minutos con el [Notebook Ejecutivo](notebooks/anime_eda_ejecutivo.ipynb)

---

⭐ **Si este proyecto te resultó útil, considera darle una estrella!**

📊 **Última actualización:** Octubre 2025
