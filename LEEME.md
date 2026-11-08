# Recetario de emergencia: versión de prueba

Desarrollado por DRAGUSTINOVIS Labs.

Esta carpeta es la app lista para subir a internet una sola vez. Después de abrirla e instalarla en el teléfono, funciona sin internet.

## 1. Subirla a GitHub Pages (gratis)

1. Crea una cuenta en github.com.
2. Toca "New repository". Ponle de nombre `recetario`, déjalo como **Public** y créalo.
3. En el repositorio, toca "Add file" y luego "Upload files". Sube **todos** los archivos de esta carpeta, sin meterlos en otra carpeta: `index.html`, `manifest.webmanifest`, `sw.js` y los cuatro íconos `.png`. Toca "Commit changes".
4. Ve a "Settings", luego "Pages". En "Branch" elige `main` y la carpeta `/ (root)`, y guarda.
5. Espera uno o dos minutos. Tu app quedará en: `https://TU-USUARIO.github.io/recetario/`

## 2. Instalarla en el teléfono

- **Android (Chrome):** abre el enlace, toca el menú de tres puntos y elige "Instalar app" o "Agregar a pantalla principal".
- **iPhone (Safari):** abre el enlace, toca el botón de compartir y elige "Agregar a inicio".

## 3. Probar que funciona sin internet

1. Abre la app instalada una vez con internet y navega un poco.
2. Pon el teléfono en modo avión.
3. Ciérrala por completo y vuelve a abrirla. Debe abrir normal, con todas las fichas.

Qué revisar en la prueba:

- El buscador, los asistentes de preguntas y las fichas.
- Mi plan familiar y Mi mochila: escribe algo, cierra la app y revisa que se haya guardado.
- SOS: pantalla, linterna (en Android pedirá permiso de cámara para prenderla) y silbato.

## 4. Cuando cambies el contenido

Sube el `index.html` nuevo y, en `sw.js`, cambia `recetario-v1` por `recetario-v2` (y así cada vez). Así los teléfonos bajan la versión nueva la próxima vez que abran la app con internet.

## 5. Opcional: una app de Android (APK) para pasarla

Con la app ya en GitHub Pages, entra a pwabuilder.com, pega tu enlace y genera el paquete de Android. Sirve para instalarla como app normal y para compartirla por archivo.

## Notas

- Los datos del plan familiar y la mochila se guardan solo en ese teléfono.
- En iPhone, Apple no deja que una página prenda la linterna; ahí el SOS usa la pantalla.
- El contenido es una guía básica: no sustituye a Protección Civil, la Cruz Roja ni al 911.
