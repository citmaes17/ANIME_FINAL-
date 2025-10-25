# 📓 Visualización del Notebook en GitHub

## Problema: Plotly no se renderiza en GitHub

GitHub no puede renderizar gráficas interactivas de Plotly directamente en los archivos `.ipynb`.

---

## ✅ Soluciones Recomendadas

### Opción 1: NBViewer (Más Fácil)

**NBViewer** renderiza notebooks con gráficas de Plotly de forma interactiva.

1. **Sube el notebook a GitHub**
2. **Copia la URL del archivo `.ipynb`** en tu repositorio
   ```
   https://github.com/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb
   ```
3. **Pega la URL en NBViewer:**
   - https://nbviewer.org/
4. **Comparte el enlace de NBViewer** en tu README

**Enlace ejemplo:**
```markdown
🔗 [Ver Notebook Interactivo en NBViewer](https://nbviewer.org/github/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb)
```

---

### Opción 2: Exportar a HTML

Convierte el notebook a HTML para visualización completa con Plotly.

#### Pasos:

1. **Instalar nbconvert (si no está instalado):**
   ```bash
   pip install nbconvert
   ```

2. **Ejecutar el comando:**
   ```bash
   jupyter nbconvert --to html notebooks/anime_eda_analysis.ipynb --output-dir docs/
   ```

3. **Resultado:**
   - Se genera `docs/anime_eda_analysis.html`
   - Este archivo se puede abrir en cualquier navegador
   - Mantiene las gráficas de Plotly interactivas

4. **Subir a GitHub:**
   - Sube el archivo HTML a tu repositorio
   - Usa GitHub Pages para publicarlo online

5. **Enlazar en README:**
   ```markdown
   📊 [Ver Análisis Completo (HTML)](docs/anime_eda_analysis.html)
   ```

---

### Opción 3: GitHub Pages (Más Profesional)

Publica el notebook HTML como una página web.

#### Pasos:

1. **Exportar a HTML** (ver Opción 2)

2. **Activar GitHub Pages:**
   - Ve a Settings → Pages
   - Selecciona branch `main` y carpeta `/docs`
   - Guarda

3. **Acceder a la página:**
   ```
   https://tu-usuario.github.io/anime-eda-project/anime_eda_analysis.html
   ```

4. **Agregar badge en README:**
   ```markdown
   [![Website](https://img.shields.io/website?url=https%3A%2F%2Ftu-usuario.github.io%2Fanime-eda-project)](https://tu-usuario.github.io/anime-eda-project/anime_eda_analysis.html)
   ```

---

### Opción 4: Google Colab (Para Ejecución Interactiva)

Permite ejecutar y visualizar el notebook directamente en Google Colab.

1. **Sube el notebook a GitHub**

2. **Crea enlace de Colab:**
   ```
   https://colab.research.google.com/github/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb
   ```

3. **Agregar badge en README:**
   ```markdown
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb)
   ```

---

## 🎯 Recomendación

**Para reclutadores y portafolio:**

1. ✅ Usa **NBViewer** (fácil, sin configuración)
2. ✅ Exporta a **HTML** y súbelo a `/docs`
3. ✅ Activa **GitHub Pages** para publicar el HTML
4. ✅ Agrega badge de **Open in Colab** para interactividad

**Tu README debe incluir:**
```markdown
## 📓 Ver el Análisis

- 🔗 [Notebook Interactivo (NBViewer)](https://nbviewer.org/github/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb)
- 📊 [Análisis Completo (HTML)](https://tu-usuario.github.io/anime-eda-project/anime_eda_analysis.html)
- [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tu-usuario/anime-eda-project/blob/main/notebooks/anime_eda_analysis.ipynb)
```

---

## 🛠️ Script Automatizado

Puedes usar este script para exportar automáticamente:

```bash
#!/bin/bash
# export_notebook.sh

# Exportar notebook a HTML
jupyter nbconvert --to html \
    notebooks/anime_eda_analysis.ipynb \
    --output-dir docs/ \
    --no-input  # Opcional: oculta código, solo muestra outputs

echo "✅ Notebook exportado a docs/anime_eda_analysis.html"
```

**Ejecutar:**
```bash
chmod +x export_notebook.sh
./export_notebook.sh
```

---

## 📌 Notas Importantes

- **NBViewer:** Funciona inmediatamente, sin configuración
- **HTML:** Requiere exportación manual, pero funciona offline
- **GitHub Pages:** Más profesional, pero requiere configuración
- **Google Colab:** Mejor para permitir ejecución interactiva

**Todas las opciones mantienen las gráficas de Plotly interactivas!** ✨
