# FULLBODY — Plan de entrenamiento de 100 días

Versión 2 modificada a partir del ZIP original. Aplicación web progresiva (PWA), pensada para móvil, sin cuenta ni servidor: los registros se guardan en el navegador del dispositivo.

## Cambios de esta versión

- Vista principal simplificada: solo muestra los 7 días de la semana del día seleccionado. El botón **Ver calendario completo** despliega/oculta el calendario de 100 días.
- En cada serie puedes elegir las repeticiones con un selector numérico nativo (en iPhone abre el selector de rueda del sistema, según la versión de iOS). La selección se guarda por serie.
- Cronómetro de entrenamiento en formato **minutos:segundos.décimas**, con iniciar/pausar, vuelta y reinicio.
- Nuevo apartado **Ejercicios**, con el catálogo completo del PDF original: músculos trabajados y notas/variantes.
- Nueva paleta roja y negra; amarillo reservado para avisos.
- Se mantienen los registros, progreso, calendario de 100 días, exportación JSON y guardado local.

## Cómo probarla

1. Descomprime el ZIP.
2. Abre `index.html` en un navegador moderno. La interfaz usa Tailwind CSS desde CDN, así que la primera carga requiere conexión a internet.
3. Para instalarla como PWA y activar el modo sin conexión de los archivos principales, publícala mediante HTTPS.

## Publicar gratis con GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube **el contenido** de esta carpeta (index.html, manifest.webmanifest, sw.js e icon.svg) a la raíz del repositorio.
3. Abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main` y carpeta `/(root)`, y guarda.
5. Abre la URL que GitHub Pages te indique.

## Instalar en iPhone

1. Abre la URL publicada en Safari.
2. Pulsa **Compartir → Añadir a pantalla de inicio**.

## Datos y privacidad

No hay cuenta ni backend. Las series, repeticiones, notas y progreso se guardan en `localStorage` de ese navegador y dispositivo. No se sincronizan automáticamente entre dispositivos. Usa **Exportar copia** en Progreso para guardar un respaldo JSON.

## Archivos

- `index.html`: aplicación completa.
- `manifest.webmanifest`: metadatos PWA.
- `sw.js`: caché básica de la aplicación.
- `icon.svg`: icono.
