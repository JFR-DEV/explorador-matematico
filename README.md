# Explorador matemático

Biblioteca educativa interactiva en español para aprender, experimentar y contrastar propuestas de solución de la colección de OpenAI.

**Abrir la biblioteca:** https://jfr-dev.github.io/explorador-matematico/

## Primera edición

- Catálogo de **372 familias y 719 manuscritos**, conservando títulos e identificadores originales.
- **Solo el capítulo 001 está desarrollado**: conjetura de racionalidad de Milne y especialización algebraica.
- Tres profundidades de lectura; historia, mapa del argumento, dos actividades y tres retos con pistas.
- Glosario de 16 conceptos, metodología, fuentes y registro de correcciones.
- Evaluación de evidencia provisional: no se certificó el teorema ni se ejecutó una formalización Lean.
- La consecuencia de especialización algebraica incorpora el 032; no se desarrolla ni audita ese capítulo.

Fecha de corte: **8 de octubre de 2026**. Versión de la colección: `fd4aeeb2ee4fc729c18d98444fed42fd0529eeeb`.

Los originales permanecen en [JFR-DEV/math](https://github.com/JFR-DEV/math). La biblioteca enlaza a esa versión, sin duplicar los manuscritos.

## Contenido y estructura

Sitio estático sin dependencias, cuentas de lector, base de datos, API de IA ni analítica.

- `index.html`, `styles.css`, `app.js`: interfaz accesible con rutas por fragmento.
- `data/catalog.json`: índice, áreas, estado editorial y todos los enlaces.
- `data/001.json`: capítulo, línea de tiempo, mapa y retos.
- `data/glossary.json`, `data/sources.json`, `data/method.json`: contenido separado.
- `editorial/families.json`: fichas para continuar el trabajo.
- `editorial/research-001.md`: alcance de lectura y preguntas abiertas.
- `.nojekyll`: publicación directa en GitHub Pages.

## Publicar

GitHub Pages: Settings → Pages → Deploy from a branch → `main` → `/(root)`.

Compatible con Vercel como proyecto estático: importar este repositorio, preset **Other**, sin comando de compilación, directorio de salida **.**. La primera entrega utiliza únicamente GitHub Pages; no requiere activar Vercel.

No hay un proceso de compilación. Se utilizan rutas relativas y fragmentos para funcionar bajo el subdirectorio de GitHub Pages y en la raíz de otros alojamientos estáticos.

## Mantener la biblioteca

Añadir cada capítulo como datos; registrar fuentes, hipótesis, dependencias y revisión por separado. No marcar una familia como desarrollada antes de completar contenido y comprobaciones. Los huecos 045, 061, 070, 123 y 163 pertenecen al catálogo fuente; no se inventaron familias para rellenarlos.

Registrar correcciones fechadas en `data/method.json` y `CHANGELOG.md`. Primero ajustar el piloto con las preguntas del lector; después continuar con el 002.

Esta biblioteca es independiente y no representa una revisión oficial de OpenAI o de los autores citados. Las analogías y actividades ilustran conceptos y explicitan sus límites.
