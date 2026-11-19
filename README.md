# MAESTROS DEL CRIMEN — Balas y Estrellas

Reservorio de datos para la página MAESTROS DEL CRIMEN de https://balasyestrellas.blogspot.com/.

- `mc-indice.json`: índice ligero para la búsqueda de autores, personajes, series y novelas.
- `fichas/<autor>.json`: expedientes completos con biografía, EL APUNTE, personajes y sinopsis.

Datos migrados del HTML facilitado por el autor el 19 de noviembre de 2026. La página Blogger conserva el diseño y el motor de búsqueda.

## Publicación

En GitHub: Settings > Pages > Deploy from a branch > main > /(root). Solo después de activar Pages y verificar `https://davidrubiosanchez76-bot.github.io/maestros-del-crimen/mc-indice.json` se debe sustituir el código publicado en Blogger por su versión de reservorio externo.

## Nuevos expedientes

Agregar o actualizar `fichas/<id>.json`, actualizar también los registros y relaciones de `mc-indice.json`, y aumentar `version` para refrescar caché. Mantener los identificadores estables, evitar duplicados y verificar vínculos entre autores, personajes, series y obras.
