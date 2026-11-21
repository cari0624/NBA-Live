# NBA Live Center

Comparador de triples NBA 2026–27. Muestra fecha, rival, 3PM y 3PA, sin porcentajes.

## Instalación

Sube `index.html`, `scripts/update.py` y `.github/workflows/update.yml` a la raíz del repositorio, conservando las carpetas. Activa GitHub Pages desde la rama `main` y carpeta `/ (root)`.

En GitHub, abre **Actions → Actualizar estadísticas NBA → Run workflow** para crear el primer archivo `data/nba.json`. Espera a que finalice en verde y actualiza la página publicada. Para que Actions pueda guardar datos, verifica **Settings → Actions → General → Workflow permissions → Read and write permissions**.

El workflow está programado para 2:00 a. m. America/Chicago, con comprobación de zona horaria y ajuste automático de horario de verano. GitHub puede retrasar u omitir ejecuciones programadas. La fuente ESPN no es oficial y sus endpoints pueden cambiar; en ese caso habría que ajustar el script. Los jugadores seleccionados se guardan localmente en cada navegador, no se sincronizan entre dispositivos.
