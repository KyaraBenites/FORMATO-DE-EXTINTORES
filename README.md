# Inspección mensual de extintores – SDE

Aplicación estática para GitHub Pages, adaptable a celular y laptop. Sin servidores ni compilación. Incluye `index.html`, `app.js`, `styles.css` y `logo-sde.png`.

## Actualizar GitHub Pages

1. Abre tu repositorio `KyaraBenites/inspeccion-extintores`.
2. En **Add file → Upload files**, sube **los cuatro archivos** de esta carpeta a la raíz del repositorio y reemplaza los existentes.
3. Haz **Commit changes** en `main`.
4. Verifica **Settings → Pages → Deploy from a branch → main / (root)**.
5. Abre https://kyarabenites.github.io/inspeccion-extintores/ y fuerza recarga si tienes una versión en caché.

## Uso

- En móvil, se muestra solo un extintor a la vez con selector, anterior/siguiente, casillas grandes, observación y cámara; los datos técnicos se despliegan bajo demanda.
- En escritorio, se dispone de tabla editable horizontal.
- Añade extintores individualmente o por cantidad.
- El PDF se descarga directamente como archivo, con una tabla en A3 apaisado distribuida en **1 o 2 páginas**. Las imágenes PNG representan las mismas páginas; Word compatible `.doc` es un documento con tabla en orientación horizontal A3.
- Las observaciones largas se acortan en la tabla; aparece una miniatura por extintor. Todas las observaciones y fotos se conservan completas en el JSON y el historial local. Muchos extintores implican texto más pequeño dentro del máximo de dos páginas.
- El historial se almacena con IndexedDB en el navegador. No es un historial compartido entre celulares ni sustituye a un servidor de respaldo.

## Limitación importante

No es físicamente posible mostrar una cantidad ilimitada de filas, textos e imágenes completos en solo dos hojas y a la vez mantener letras legibles. Este programa respeta el límite de hojas para la **tabla de resumen**, ajustando tamaño y abreviando contenido. Guarda y comparte el JSON como evidencia completa. Word es HTML compatible con Word (.doc); distintos programas pueden paginarlo de modo distinto, mientras que el PDF conserva exactamente 1 o 2 páginas.
