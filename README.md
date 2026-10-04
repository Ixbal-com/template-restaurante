# Plantilla Ixbal · Restaurante

Plantilla para restaurantes, cafeterías, fondas y cocinas económicas. Estilo **cálido editorial**: fondo crema, terracota y oliva, con títulos en serif (Fraunces).

**Incluye:** hero con reservación por WhatsApp, especialidades con foto y precio, menú por categorías, historia del lugar, galería, opiniones, preguntas frecuentes, horario con indicador de “Abierto ahora”, mapa y datos estructurados de restaurante para Google.

## Uso

```bash
npm run dev     # servidor local en http://localhost:4321
npm run check   # valida el sitio (sin dependencias)
```

También puedes abrir `index.html` con cualquier servidor estático. No requiere compilación.

## Personalizar

1. **Identidad:** colores y tipografía en `assets/css/tokens.css`.
2. **Contenido:** textos, menú y precios en `index.html`, organizado por secciones.
3. **Imágenes:** la plantilla tiene 10 espacios de imagen listados en `imageSlots` de `template.json`. Mientras no tengan foto real, muestran una etiqueta con lo que va ahí. Ver [AGENTS.md](AGENTS.md#espacios-de-imagen).

Las reglas de arquitectura y la lista de datos que se repiten están en [AGENTS.md](AGENTS.md).

## Publicar

Es un sitio estático: sirve la raíz del repositorio en GitHub Pages, Netlify, Vercel o AWS Amplify.

> Antes de publicar, convierte `assets/img/og-image.svg` a PNG de 1200 × 630 y usa una URL absoluta en `og:image`: WhatsApp y Facebook no muestran vistas previas en SVG.
