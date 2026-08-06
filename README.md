# Proyecto Red de Distribución · 4100730

Simulador interactivo de una red eléctrica de distribución para el curso **Sistemas de Distribución (4100730)** — Universidad Nacional de Colombia, Sede Manizales.

Es un **archivo único autocontenido** (`index.html`) con tres vistas navegables por pestañas:

- **Vista 3D física.** Modelo físico navegable (Three.js) con simulación cualitativa de energización y coordinación de protecciones. Incluye vistas **Planta** y **Perfil**, panel **unifilar** IEEE/ANSI sincronizado, recorrido en **primera persona**, maniobras y eventos (falla, rayo, caída de árbol).
- **Planta · convenciones.** Plano cenital esquemático sobre la traza física, con símbolos IEEE/ANSI y su recuadro de convenciones.
- **SmartGrid · autorreparación.** Unifilar de cinco alimentadores (reproducción del esquema S&C) con la operación de autorreparación (FLISR): aislar la falla y restaurar desde alimentadores vecinos, con rayo y carro canasta. Conserva la operación de los fusibles.

## Uso

Abrir la URL de GitHub Pages del repositorio (ver más abajo cómo activarla), o descargar `index.html` y abrirlo en un navegador moderno.

> Requiere conexión a internet la primera vez que se abre la vista 3D, porque carga Three.js y las tipografías desde CDN. Para el recorrido en primera persona el navegador pedirá permiso de bloqueo de puntero.

## Publicar con GitHub Pages

1. Sube estos archivos al repositorio (al menos `index.html` y `.nojekyll`).
2. En el repositorio: **Settings → Pages**.
3. En *Build and deployment*, *Source*: **Deploy from a branch**; *Branch*: `main` y carpeta `/ (root)`. Guardar.
4. En 1–2 minutos, el sitio queda en `https://<usuario>.github.io/<repositorio>/`.

## Archivos

- `index.html` — proyecto completo (las tres vistas embebidas). Punto de entrada.
- `.nojekyll` — evita el procesamiento Jekyll de GitHub Pages para sitios estáticos.
- `smartgrid-selfhealing.html`, `planta-convenciones.html`, `red-distribucion-sim.html` — vistas individuales (opcionales; útiles para enlace directo a una vista).

## Créditos

Material docente. Símbolos según convenciones IEEE/ANSI. Reproducción del esquema de autorreparación inspirada en el material de S&C Electric con fines educativos.
