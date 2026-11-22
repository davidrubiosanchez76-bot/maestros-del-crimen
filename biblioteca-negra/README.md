# Biblioteca Negra · Balas y Estrellas

Almacén independiente del catálogo de novelas que consume la página estática de Blogger.

## Archivos
- `novelas.json`: fichas completas de las novelas, en el orden visible de «Todo el archivo», con sus seis facetas y lista de subgéneros.
- `generos.json`: definiciones de géneros y portadas ilustradas de sus tarjetas.

## Altas y modificaciones
1. Antes de dar de alta una novela, comprobar que no existe en `novelas.json` por título, título original y autor.
2. Añadir al principio del array `novelas` una ficha nueva para que sea la primera del archivo. El contador se calcula automáticamente.
3. Conservar estas propiedades: `id`, `title`, `author`, `original`, `year`, `synopsis`, `cover`, `review`, `buy`, `quien`, `que`, `como`, `porque`, `donde`, `cuando`, `generos`.
4. `id` es un identificador legible único; las seis facetas y `generos` son arrays con las claves ya utilizadas en el catálogo. No inventar opciones sin actualizar el selector y su taxonomía.
5. Para una nueva ficha se proporciona una URL de portada, que se guarda en `cover`. No inventar enlaces de reseña o compra; dejar `review` y `buy` vacíos si no están confirmados.
6. Mantener las 14 definiciones de `generos.json` separadas de los registros de novelas.
7. No modificar el diseño de Blogger ni sus funciones para una alta normal.

## Publicación
El HTML de Blogger descarga los archivos desde la rama pública `main` usando raw.githubusercontent.com con jsDelivr como recurso alternativo. Las nuevas fichas no requieren volver a publicar el HTML; puede existir un breve retraso por caché.

El repositorio es compartido con «Maestros del Crimen» únicamente por limitación para crear nuevos repositorios desde el conector. No modificar los archivos de «Maestros del Crimen» al gestionar Biblioteca Negra.
