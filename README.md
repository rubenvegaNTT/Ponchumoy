# Ponchumoy para iPad

Versión PWA del juego **Ponchumoy Ponchumaniano** preparada para Safari/iPadOS.

## Publicarla en GitHub Pages

1. Crea un repositorio en GitHub, por ejemplo `ponchumoy`.
2. Sube **todo el contenido de esta carpeta** a la raíz del repositorio.
3. En GitHub entra en **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Elige la rama `main` y la carpeta `/ (root)` y pulsa **Save**.
6. GitHub mostrará la URL pública del juego.

## Instalarla en el iPad

1. Abre la URL de GitHub Pages en **Safari**.
2. Pulsa **Compartir**.
3. Elige **Añadir a pantalla de inicio**.
4. Activa **Abrir como app web** si aparece la opción.
5. Pulsa **Añadir**.

A partir de ese momento Ponchumoy tendrá icono propio y se abrirá como una app. Tras cargarla una vez con conexión, el service worker permite volver a abrir los archivos esenciales del juego sin conexión.

## Cambios incluidos

- PWA instalable en iPad.
- Icono propio.
- Modo standalone/pantalla completa.
- Orientación horizontal recomendada.
- Aviso al girar el iPad en vertical durante la partida.
- Controles táctiles mejorados con pointer capture.
- Prevención de scroll, selección y gestos accidentales durante la partida.
- Compatibilidad con safe areas del iPad.
- Récord guardado mediante localStorage.
- Caché offline con service worker.

## Nota

El `service-worker.js` necesita que el juego se abra desde `https://` o `http://localhost`; no funciona abriendo `index.html` directamente desde la app Archivos del iPad.
