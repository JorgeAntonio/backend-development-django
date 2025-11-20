# Backend Sessions · Python & Django

Landing page + curriculum hub inspired by Guillermo Rauch's portfolio to showcase the “Backend Sessions” professional course (Python, Django, DRF, Deploy). Every session has space for its own recap page and links to the materials used in class.

## Overview
- **Home (`index.html`):** Vercel-like list of the 8 sessions. Only completed sessions are clickable, upcoming ones stay muted.
- **About (`about.html`):** Detailed syllabus describing duration, docentes and resultados por sesión.
- **Session Detail Pages:** e.g. `sessions/session-1.html` centralizes objetivos, agenda y recursos (slides + workshop) for each class.
- **Slides & Workshops:** Reveal.js decks plus cURL labs stored under `sessions/fundamentals/`.

## Tech Stack
- HTML5 + custom CSS (Inter typography, Vercel palette)
- [Reveal.js](https://revealjs.com/) for presentations
- [Highlight.js](https://highlightjs.org/) for code snippets within slides

## Project Structure
```
.
├── index.html                # Portada estilo Guillermo Rauch
├── about.html                # Plan de las 8 sesiones
├── favicon.svg               # Identidad visual del curso
├── css/
│   └── style.css             # Sistema de diseño y componentes
└── sessions/
    ├── session-1.html        # Detalle de la Sesión 1
    └── fundamentals/
        ├── fundamentals.html # Slides (Reveal.js)
        └── curl.html         # Workshop práctico con cURL
```

## Getting Started
1. Clona o descarga este repositorio.
2. Abre `index.html` en tu navegador para ver la portada.
3. Haz clic en las sesiones habilitadas para ir a su página de resumen y desde ahí a los recursos utilizados.

## Session Roadmap
| Sesión | Estado | Descripción | Recursos |
| --- | --- | --- | --- |
| 1. Fundamentos de la Web | ✅ Publicada | HTTP, status codes, JSON vs HTML, DevTools, APIs públicas | [Detalle](sessions/session-1.html) · [Slides](sessions/fundamentals/fundamentals.html) · [Workshop cURL](sessions/fundamentals/curl.html) |
| 2. Python aplicado a Backend | 🛠 En curso | Colecciones, excepciones, microservidor JSON | _Pendiente de publicación_ |
| 3. Git & GitHub para equipos | 🗂 Próxima | Branching, PRs, issues, GitHub Actions | _Pendiente_ |
| 4. Django: Fundamentos + Auth | 🧭 Planeada | Proyecto base, vistas, forms, login/logout, CSRF | _Pendiente_ |
| 5. Modelos & Bases de Datos | 🗄 Planeada | ORM, relaciones, consultas con SQLite/PostgreSQL | _Pendiente_ |
| 6. API REST con DRF | 🔌 Planeada | Serializers, ViewSets, routers, auth JWT/Token | _Pendiente_ |
| 7. Testing & Performance | 🚀 Planeada | pytest-django, optimización, pruebas de carga | _Pendiente_ |
| 8. Deploy AWS + Nginx + Gunicorn | ☁️ Próxima | EC2, Gunicorn, Nginx, SSL, automatización | _Pendiente_ |

## Contributing / Extending
- Para agregar una nueva sesión, duplica `sessions/session-1.html`, actualiza el contenido y habilita el enlace en `index.html`.
- Añade nuevos recursos (slides, workshops, repos) dentro de `sessions/<topic>/` y enlázalos desde la página de detalle.
- Mantén los estilos consistentes en `css/style.css`; la tipografía y la paleta están definidas al inicio del archivo.

## Credits
Diseño inspirado en el portafolio de [Guillermo Rauch](https://rauchg.com/) y el sistema visual de Vercel. Contenido del curso por Jorge Antonio Del Aguila y equipo docente.
