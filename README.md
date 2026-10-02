# Kiwi Adventures - Update Checker

Archivos que lee el mod **Modpack Update Checker** para avisar a los jugadores cuando sale una versión nueva de Kiwi Adventures.

## Cómo publicar una versión nueva (ej. 1.0.1)
1. Crear la carpeta `versions/1.0.1` con un `changelog.txt` adentro (los cambios de esa versión).
2. Agregar la versión al final de la lista `versions` en `meta.json`:
   `{ "id": "1.0.1", "releasedAt": <fecha en milisegundos> }`
3. Subir los cambios a GitHub (commit + push).
4. En el modpack que se distribuye, cambiar `currentVersion` a `1.0.1` en `config/modpack-update-checker/config.json`.

Los jugadores con una versión anterior verán el aviso "Update Available" en el menú.