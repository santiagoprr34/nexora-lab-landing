# Nexora LAB · Landing

Landing page estática de Nexora LAB (anuncios para ecommerce por etapa del embudo: TOFU, MOFU, BOFU).

## Contenido

```
index.html        → la página completa (HTML + CSS, sin dependencias ni build)
assets/           → 6 videos .mp4 (540 px, comprimidos para web) y sus portadas .jpg
  tofu1, tofu2, mofu1, bofu1   → galería de anuncios
  testimonio1, testimonio2     → testimonios de clientes
```

- Fuentes: Space Grotesk e Inter desde Google Fonts.
- Todos los botones de llamada a la acción llevan a https://www.instagram.com/santiago423_/
- Funciona en móvil y escritorio.

## Instrucciones para Claude (subir a GitHub y publicar)

1. Crea un repositorio nuevo en la cuenta de GitHub de Santiago, por ejemplo `nexora-lab-landing` (público si se va a usar GitHub Pages en plan gratuito).
2. Sube TODO el contenido de esta carpeta a la raíz del repositorio, respetando la carpeta `assets/`. No cambies nombres de archivos: `index.html` los referencia con rutas relativas `assets/...`.
   ```bash
   git init
   git add .
   git commit -m "Landing Nexora LAB"
   git branch -M main
   git remote add origin https://github.com/<usuario>/nexora-lab-landing.git
   git push -u origin main
   ```
   (Con `gh`: `gh repo create nexora-lab-landing --public --source=. --push`.)
3. Activa GitHub Pages: Settings → Pages → Source: "Deploy from a branch" → Branch `main`, carpeta `/ (root)` → Save.
4. En uno o dos minutos la página queda en `https://<usuario>.github.io/nexora-lab-landing/`.
5. Comprueba que los 6 videos cargan y que los botones abren el Instagram.

## Cambios frecuentes

- **Enlace de los botones:** buscar `https://www.instagram.com/santiago423_/` en `index.html` y reemplazarlo en todas las apariciones.
- **Precios:** sección `<!-- PACKS -->`.
- **Marcas:** sección `<!-- PRUEBAS -->`.
- **Videos:** reemplazar el archivo en `assets/` con el mismo nombre, o cambiar `src` y `poster` en la etiqueta `<video>`.
- **Dominio propio (opcional):** Settings → Pages → Custom domain.
