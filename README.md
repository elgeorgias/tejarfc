# E.F. Tejar

Web sencilla del equipo Benjamín: escudo del club, calendario de partidos y enlaces a los campos en Google Maps. Adaptable a móviles y sin dependencias.

## Probar en local

Desde esta carpeta, ejecuta:

```sh
python3 -m http.server 8000
```

Abre `http://localhost:8000` en el navegador.

## Publicar en internet

El workflow de GitHub Actions en `.github/workflows/pages.yml` publica el sitio automáticamente al subir cambios a `main`. En GitHub, abre **Settings → Pages** y elige **GitHub Actions** como fuente de publicación. Después de subir los archivos al repositorio, la dirección pública aparecerá en esa página de configuración.

El calendario contiene las cinco jornadas incluidas en el archivo facilitado por el club. El enlace de descarga genera el archivo `calendario-benjamin-ef-tejar.ics` con los partidos, sus horarios y ubicaciones. Para actualizarlo, edita la lista de partidos en `index.html` y los eventos correspondientes en el archivo `.ics`.
