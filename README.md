# Recursos interactivos de Epigenética — SPECTO PUCV

Aplicativos web autocontenidos (HTML/CSS/JS, sin backend ni build step) desarrollados para el **Taller de Formación Docente** del proyecto **Fondecyt 1211092 — "Ciencias para la ciudadanía en educación técnico profesional: diseño de secuencias de enseñanza y aprendizaje basadas en modelos con tecnologías inmersivas"**, Instituto de Química, Pontificia Universidad Católica de Valparaíso.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | Página de inicio con acceso a ambos aplicativos. |
| `taller-epigenetica.html` | Canvas interactivo del taller docente: conceptos clave, caso de gemelas, simulador de metilación/acetilación del ADN y actividades para el aula. |
| `compactacion-3d.html` | Visor 3D (Three.js) de los niveles de compactación del material genético: doble hélice, nucleosomas, solenoide y cromatina. |

Ambos archivos son independientes entre sí; cada uno puede abrirse directamente en el navegador o enlazarse por separado.

## Cómo publicarlo con GitHub Pages

1. Crea un repositorio nuevo en GitHub y sube todo el contenido de esta carpeta (incluye el archivo `.nojekyll`, necesario para que GitHub Pages sirva los HTML sin procesarlos con Jekyll).
2. En el repositorio, ve a **Settings → Pages**.
3. En **Source**, selecciona la rama `main` (o `master`) y la carpeta `/ (root)`.
4. Guarda. GitHub entregará una URL del tipo `https://<tu-usuario>.github.io/<nombre-repo>/`.
5. Desde esa URL, `index.html` se sirve automáticamente; los otros dos aplicativos quedan disponibles en:
   - `https://<tu-usuario>.github.io/<nombre-repo>/taller-epigenetica.html`
   - `https://<tu-usuario>.github.io/<nombre-repo>/compactacion-3d.html`

## Requisitos técnicos

- No requieren instalación ni build: son HTML autocontenidos que cargan sus dependencias (Tailwind CSS, Three.js, Font Awesome) desde CDN.
- Necesitan **conexión a internet** en el navegador del usuario final para cargar esas dependencias.
- Compatibles con navegadores modernos (Chrome, Edge, Firefox, Safari). El visor 3D requiere soporte de WebGL.

## Notas de mantenimiento

- `taller-epigenetica.html`: el modelo de doble hélice (Módulo 3, Nivel 1) fue corregido para que los puentes de hidrógeno coincidan matemáticamente con la curva de las hebras (antes, 10 de 12 puentes quedaban visualmente flotando y desconectados).
- Si necesitas editar cualquiera de los dos archivos, todo el HTML/CSS/JS vive en un único archivo por aplicativo — no hay assets externos que gestionar aparte de los CDN.

## Autoría y uso

Material docente elaborado por el equipo del proyecto SPECTO PUCV (Fondecyt 1211092). Uso educativo; si lo reutilizas o adaptas, por favor mantén la atribución al proyecto.
