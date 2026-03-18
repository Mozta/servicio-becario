# Laboratorio de IA y Realidad Extendida — Servicio Becario

> **Prototipo base** para el programa de servicio becario del Laboratorio de Inteligencia Artificial y Realidad Extendida.

## Descripción

Este repositorio contiene un prototipo de la página web  del laboratorio. Sirve como punto de partida para que los alumnos de servicio becario practiquen y aprendan desarrollo web, completando y mejorando el sitio como parte de sus actividades.

El sitio está construido con HTML, CSS y JavaScript puro, sin frameworks ni herramientas de compilación, para que sea accesible a alumnos que están comenzando en desarrollo web.

## Estructura del proyecto

```
index.html              ← Página principal
css/
  ├── styles.css        ← Estilos generales del sitio
  └── project.css       ← Estilos para páginas de detalle de proyecto
js/
  └── main.js           ← JavaScript (scroll suave, interacciones)
pages/
  └── proyecto.html      ← Página de ejemplo de un proyecto (por completar)
assets/
  └── images/           ← Imágenes del sitio y proyectos
```

## Cómo visualizar el sitio

Abrir `index.html` directamente en el navegador o usar un servidor local:

```bash
python3 -m http.server
```

Luego visitar `http://localhost:8000` en el navegador.

## Secciones del sitio

- **Inicio** — Presentación del laboratorio con mensaje principal y botones de navegación.
- **Nosotros** — Áreas de trabajo: Inteligencia Artificial, Realidad Extendida, Prototipado y Sistemas.
- **Proyectos** — Tarjetas con los proyectos del laboratorio. Cada una enlaza a su página de detalle en `pages/`.
- **Contacto** — Correo, ubicación y horario del laboratorio.

## Cómo agregar un nuevo proyecto

1. Crear una nueva página en `pages/` (puedes copiar `tutorai.html` como base).
2. Agregar una tarjeta dentro del bloque `<!-- INICIO/FIN TARJETAS DE PROYECTOS -->` en `index.html`:

```html
<div class="project-card">
  <div class="project-image">Imagen del proyecto</div>
  <div class="project-content">
    <h4>Nombre del proyecto</h4>
    <p>Descripción breve del proyecto.</p>
    <a href="pages/nombre-proyecto.html" class="project-link">Ver proyecto</a>
  </div>
</div>
```

3. Colocar las imágenes del proyecto en `assets/images/`.

## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
