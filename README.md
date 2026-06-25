# 📚 Página de Publicaciones

Página de publicaciones académicas con **actualización automática** desde ORCID.

## ¿Cómo funciona?

- La página consulta la **API pública de ORCID** (`pub.orcid.org`) directamente desde el navegador del visitante.
- GitHub Actions la **re-despliega automáticamente cada lunes** para reflejar cualquier cambio.
- Cada vez que publiques algo nuevo y lo agregues a ORCID, aparecerá aquí solo.

---

## 🚀 Instrucciones de instalación (5 pasos)

### Paso 1 — Crear cuenta en GitHub
Ve a [github.com](https://github.com) y crea una cuenta gratuita si no tienes.

### Paso 2 — Crear un repositorio nuevo

1. Haz clic en **"New repository"**
2. Nombre: `publications` (o el que prefieras)
3. Marca **"Public"** (necesario para GitHub Pages gratis)
4. Haz clic en **"Create repository"**

### Paso 3 — Subir los archivos

Puedes hacerlo de dos formas:

**Opción A — Desde la web de GitHub:**
1. En tu repositorio vacío, haz clic en **"uploading an existing file"**
2. Arrastra los archivos `index.html` y la carpeta `.github/`
3. Haz clic en **"Commit changes"**

**Opción B — Con git (terminal):**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/publications.git
git push -u origin main
```

### Paso 4 — Activar GitHub Pages

1. En tu repositorio → **Settings** → **Pages**
2. En "Source" selecciona **"GitHub Actions"**
3. Guarda

### Paso 5 — Esperar el primer deploy (~2 min)

Ve a la pestaña **Actions** de tu repositorio. Verás el workflow corriendo.
Cuando termine, tu página estará disponible en:

```
https://TU_USUARIO.github.io/publications/
```

---

## 🔗 Enlazar desde tu Google Sites

En tu Google Site, puedes poner el enlace a esta página en la sección de publicaciones, o insertar un iframe:

1. En Google Sites → Insertar → **Insertar URL**
2. Pega tu URL de GitHub Pages

---

## 🔄 Actualización automática

- **Automática**: cada lunes a las 05:00 (Chile) el workflow se ejecuta solo.
- **Manual**: en GitHub → pestaña Actions → "Deploy Publications Page" → "Run workflow".
- **Al publicar algo nuevo**: solo agrega el trabajo a tu perfil ORCID en [orcid.org]. La siguiente actualización automática lo incluirá.

---

## ✏️ Personalización

El archivo `index.html` contiene todo. Si quieres cambiar algo:

- **Tu nombre en autores**: busca `MY_NAMES` en el script y agrega variantes de tu nombre.
- **Colores**: modifica las variables CSS en `:root { ... }`.
- **ORCID ID**: cambia `ORCID_ID` en el script si alguna vez necesitas actualizarlo.

---


