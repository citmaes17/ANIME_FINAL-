# 🚀 Guía para Subir el Proyecto a GitHub

## Paso 1: Crear Repositorio en GitHub

1. Ve a https://github.com/new
2. **Nombre del repositorio:** `anime-eda-project` (o el que prefieras)
3. **Descripción:** "Exploratory Data Analysis on 15K anime from MyAnimeList"
4. **Visibilidad:** Public (para portafolio)
5. ✅ **NO inicializar** con README (ya tenemos uno)
6. Clic en **"Create repository"**

---

## Paso 2: Configurar Git Local

### Si es tu primer proyecto en Git:

```bash
# Configurar tu nombre y email
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@ejemplo.com"
```

### Verificar configuración:
```bash
git config --global --list
```

---

## Paso 3: Inicializar Git en tu Proyecto

Abre tu terminal y navega a la carpeta del proyecto:

```bash
cd /ruta/a/anime-eda-project
```

Inicializa Git:

```bash
git init
```

---

## Paso 4: Agregar Archivos al Repositorio

```bash
# Agregar todos los archivos
git add .

# Verificar qué archivos se agregarán
git status
```

---

## Paso 5: Hacer el Primer Commit

```bash
git commit -m "Initial commit: Complete EDA project with 12 visualizations"
```

---

## Paso 6: Conectar con GitHub

Reemplaza `TU-USUARIO` con tu nombre de usuario de GitHub:

```bash
git remote add origin https://github.com/TU-USUARIO/anime-eda-project.git
```

Verificar la conexión:
```bash
git remote -v
```

---

## Paso 7: Subir el Proyecto a GitHub

### Opción 1: Branch `main` (recomendado para proyectos nuevos)

```bash
git branch -M main
git push -u origin main
```

### Opción 2: Branch `master` (si prefieres usar master)

```bash
git push -u origin master
```

---

## Paso 8: Verificar en GitHub

1. Ve a tu repositorio en GitHub: `https://github.com/TU-USUARIO/anime-eda-project`
2. Deberías ver todos tus archivos subidos
3. El README.md se mostrará automáticamente en la página principal

---

## 📝 Comandos Git Útiles para el Futuro

### Después de hacer cambios:

```bash
# Ver qué archivos cambiaron
git status

# Agregar archivos modificados
git add .

# O agregar archivos específicos
git add archivo.py

# Hacer commit con mensaje descriptivo
git commit -m "Add new visualization: X"

# Subir cambios a GitHub
git push
```

### Para actualizar tu repositorio local:

```bash
# Si trabajas desde múltiples computadoras
git pull
```

### Ver historial de commits:

```bash
git log
git log --oneline  # Versión compacta
```

---

## 🎨 Paso 9: Personalizar el Repositorio en GitHub

### 1. Agregar Topics (Etiquetas)

En tu repositorio de GitHub:
- Clic en el ícono de engranaje ⚙️ junto a "About"
- Agregar topics: `python` `data-analysis` `eda` `plotly` `pandas` `anime` `myanimelist` `data-science` `jupyter-notebook`

### 2. Editar la Descripción

- **Short description:** "📊 EDA on 15K anime from MyAnimeList | Python, Pandas, Plotly"
- **Website:** (si tienes GitHub Pages habilitado)

### 3. Actualizar README con tu información

Edita el README.md y reemplaza:
- `[@tu-usuario]` con tu usuario de GitHub
- `[Tu Perfil]` con tu LinkedIn
- `tuemail@ejemplo.com` con tu email
- Los links de badges y stars

---

## 🌐 Paso 10: Activar GitHub Pages (Opcional)

Para publicar tu notebook HTML:

1. Ve a **Settings** → **Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main`
4. **Folder:** `/docs`
5. **Save**

Tu análisis estará disponible en:
```
https://TU-USUARIO.github.io/anime-eda-project/
```

---

## 📊 Paso 11: Agregar Badges Actualizados al README

Después de subir, actualiza estos badges en el README:

```markdown
[![GitHub Stars](https://img.shields.io/github/stars/TU-USUARIO/anime-eda-project?style=social)](https://github.com/TU-USUARIO/anime-eda-project)
[![GitHub Forks](https://img.shields.io/github/forks/TU-USUARIO/anime-eda-project?style=social)](https://github.com/TU-USUARIO/anime-eda-project/fork)
[![GitHub Issues](https://img.shields.io/github/issues/TU-USUARIO/anime-eda-project)](https://github.com/TU-USUARIO/anime-eda-project/issues)
```

---

## 🎯 Checklist Final

Antes de compartir tu portafolio:

- [ ] ✅ Todos los archivos subidos correctamente
- [ ] ✅ README.md muestra las imágenes correctamente
- [ ] ✅ Información personal actualizada (nombre, email, LinkedIn)
- [ ] ✅ Links funcionales (NBViewer, Colab)
- [ ] ✅ Topics agregados al repositorio
- [ ] ✅ Descripción del repositorio personalizada
- [ ] ✅ LICENSE agregada
- [ ] ✅ GitHub Pages activado (opcional)
- [ ] ✅ Repositorio público

---

## 🚨 Solución de Problemas Comunes

### Problema: "Permission denied (publickey)"

**Solución:** Configura SSH o usa HTTPS:

```bash
# Cambiar a HTTPS
git remote set-url origin https://github.com/TU-USUARIO/anime-eda-project.git
```

### Problema: "Updates were rejected"

**Solución:** Primero haz pull:

```bash
git pull origin main --allow-unrelated-histories
git push origin main
```

### Problema: Archivos muy grandes (>100MB)

**Solución:** Usa Git LFS o sube solo los datasets procesados:

```bash
# Agregar a .gitignore
echo "data/raw/*.csv" >> .gitignore
git add .gitignore
git commit -m "Ignore raw dataset"
```

---

## 🎓 Recursos Adicionales

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)

---

## 💡 Tips para un Repositorio Profesional

1. ✨ **README atractivo:** Usa emojis, badges, y visualizaciones
2. 📊 **Muestra resultados:** Agrega las gráficas clave en el README
3. 📝 **Commits descriptivos:** "Add X" es mejor que "Update"
4. 🔖 **Tags:** Usa tags/topics para que sea fácil de encontrar
5. 📄 **Documentación:** Incluye cómo ejecutar y reproducir el análisis
6. 🌟 **README en inglés:** Máxima visibilidad internacional (opcional)

---

**¡Listo! Tu proyecto está ahora en GitHub y listo para impresionar a reclutadores! 🚀**
