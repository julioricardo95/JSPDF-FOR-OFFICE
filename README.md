# Fichas municipales

Aplicación Astro para completar fichas municipales y descargarlas como PDF.

## Estructura

- `src/pages/ficha/`: rutas para cada ficha.
- `src/components/FichaF*.astro`: contenido específico de cada ficha.
- `src/components/FichaForm.astro`: estructura común del formulario, título y botón de descarga.
- `src/components/DatosPropietario.astro` y `DatosEncuesta.astro`: grupos de campos reutilizados.
- `src/components/FichaPropietarioComun.astro`: campos compartidos por las fichas 4 y 5.
- `src/components/JsPdf.astro`: generación del PDF.

Para añadir una ficha, crea su componente específico dentro de `src/components/`, envuelve los campos con `FichaForm` y agrega una página en `src/pages/ficha/`. Reutiliza los grupos de campos existentes cuando correspondan; conserva en el componente específico las opciones que sean propias de esa ficha.

## Comandos

| Comando | Acción |
| --- | --- |
| `npm install` | Instala las dependencias |
| `npm run dev` | Inicia el servidor local de Astro |
| `npm run build` | Genera el sitio estático en `dist/` |
| `npm run preview` | Previsualiza el sitio generado |
