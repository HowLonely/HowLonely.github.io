# Imágenes de la landing page

Coloca aquí tus archivos con **exactamente estos nombres**. Mientras no exista un archivo,
la página muestra un marcador con el nombre esperado — no se rompe nada.

## Archivos esperados

| Ruta | Qué va ahí | Tamaño recomendado |
|---|---|---|
| `img/sala-control/01-dashboard.jpg` | Captura principal del dashboard | 1600 × 1000 px |
| `img/sala-control/02-telemetria.jpg` | Vista de telemetría / gráficos | 1600 × 1000 px |
| `img/sala-control/03-camaras.jpg` | Vista de cámaras en vivo | 1600 × 1000 px |
| `img/sala-control/04-dispositivo.jpg` | Foto del dispositivo IoT / ESP32 en faena | 1600 × 1000 px |
| `img/lavanderia/01-web.jpg` | Captura de la web administrativa | 1600 × 1000 px |
| `img/control-flota/01-mapa.jpg` | Captura de la plataforma de flota | 1600 × 1000 px |
| `img/importador/01-flujo.jpg` | Captura o diagrama del microservicio | 1600 × 1000 px |
| `img/og-cover.jpg` | Imagen de vista previa al compartir el link | 1200 × 630 px |

## Recomendaciones

- Proporción **16:10** para las capturas de proyecto (se recortan a esa forma).
- Usa `.jpg` para fotos y capturas; si prefieres `.png` o `.webp`, cambia también la
  extensión en `index.html` (busca `img/` para encontrar cada referencia).
- Comprime antes de subir (por ejemplo en https://squoosh.app) — apunta a menos de 300 KB
  por imagen para que la página cargue rápido.
- Si un proyecto es confidencial: difumina datos sensibles o usa capturas con datos de demo.

## Cómo agregar más imágenes a un proyecto

En `index.html`, dentro del proyecto destacado hay un bloque `<div class="thumbs">` con
tres miniaturas. Para agregar otra, duplica un bloque `<div class="shot" data-lightbox>…</div>`
y cambia el `src`, el `alt` y el texto del `<code>`.

## ¿Y la foto de perfil?

La landing **no usa foto de perfil**: en su lugar el hero muestra una tarjeta de
telemetría animada con datos simulados (`<div class="telemetry">` en `index.html`).

Si más adelante quieres poner tu foto, reemplaza ese bloque por:

```html
<div class="telemetry">
  <div class="tm-card" style="aspect-ratio:4/5">
    <img src="img/perfil.jpg" alt="Ellian Troncoso"
         style="width:100%;height:100%;object-fit:cover">
  </div>
</div>
```
