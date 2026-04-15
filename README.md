# Presentación Seguridad Informática - Camping 44

Este repositorio publica una presentación HTML estática en GitHub Pages.

## Cómo visualizarla localmente

Abrí `index.html` directamente en el navegador o ejecutá un servidor local:

```bash
python -m http.server 8000
```

Luego ingresá a: `http://localhost:8000/`

## Publicación en GitHub Pages

Este repositorio incluye un workflow (`.github/workflows/deploy-pages.yml`) que publica automáticamente en GitHub Pages cuando hay push a `main`, `master` o `work`.

Si ves un **404** en GitHub Pages:

1. Verificá que el repositorio esté público (o que tu plan soporte Pages en privado).
2. En GitHub, andá a **Settings → Pages**.
3. En **Build and deployment**, elegí **Source: GitHub Actions**.
4. Hacé push de este branch y esperá a que finalice el workflow **Deploy static HTML to GitHub Pages**.
5. Confirmá la URL final en el resumen del job de deploy.

> Nota: la URL suele ser `https://<usuario>.github.io/<repositorio>/`.
