# Instalación — Hypomnemata moderno

Este paquete está pensado para el repositorio:
`FelipeHurtado-Drafts/Afelipehurtadoagudelo-md.github.io`

## Qué corrige

1. Actualiza `hugo.toml` al formato real de **Hugo Theme Stack v4**.
2. Sustituye los colores Solarized/terminal y Montserrat por una estética más limpia y editorial.
3. Mejora tarjetas, lectura, barra lateral, modo oscuro, etiquetas y adaptación móvil.
4. Coloca el avatar en `assets/img/avatar.png`, que es la ubicación compatible con el procesamiento de imágenes del tema actual.

## Instalación desde Pop!_OS

Abre una terminal dentro de la carpeta local del repositorio y ejecuta:

```bash
unzip -o ~/Downloads/hypomnemata_moderno.zip -d .
git add hugo.toml assets layouts
git commit -m "Moderniza diseño de Hypomnemata"
git push
```

GitHub Actions debería reconstruir la página automáticamente después del `push`.

## Importante

No copies la carpeta `hypomnemata_moderno` completa dentro del repositorio. El contenido del ZIP debe caer directamente en la raíz, de modo que queden estas rutas:

- `hugo.toml`
- `assets/scss/custom.scss`
- `assets/img/avatar.png`
- `layouts/partials/head/custom.html`

La carpeta antigua `static/img/avatar.jpg` puede quedarse; el nuevo diseño no la usa.
