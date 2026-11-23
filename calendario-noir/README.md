# Calendario Noir · Balas y Estrellas

## Base de datos única

Archivo principal: `efemerides.json` en la carpeta `calendario-noir/` del repositorio público `davidrubiosanchez76-bot/maestros-del-crimen`.

* Raw: https://raw.githubusercontent.com/davidrubiosanchez76-bot/maestros-del-crimen/main/calendario-noir/efemerides.json
* CDN alternativo: https://cdn.jsdelivr.net/gh/davidrubiosanchez76-bot/maestros-del-crimen@main/calendario-noir/efemerides.json

## Estructura

* `version`: versión del esquema.
* `daily`: efemérides documentadas con **día, mes y año exactos**, con claves `dia`, `mes`, `ano`, `nombre`, `tipo` y `desc`.
* `monthOnly`: hitos documentados solo con **mes y año**, sin `dia`, con claves `mes`, `ano`, `nombre`, `desc`.

El archivo alimenta el Calendario Noir (Blogger) y el recuadro de efemérides en la portada.
No se deben añadir efemérides de nueva creación en el HTML ni en el XML de Blogger.

## Protocolo de altas

1. Verificar fecha completa y fuentes fiables. No situar en el día 1 acontecimientos sin día comprobado.
2. Evitar duplicados (incluyendo nombres/seudónimos, estreno frente a publicación y mismo hecho en diferentes fechas).
3. Añadir objetos al array correspondiente y conservar su estructura.
4. Validar JSON y comprobar ambas vistas tras la publicación.
5. Para una fecha conocida **solo por el año** no utilizar este archivo; emplear Cronología Negra.

## Situación del repositorio

Se usa una carpeta independiente dentro del repositorio existente porque la conexión GitHub disponible no dispone de la operación de crear repositorios. La carpeta puede trasladarse después a `calendario-noir` sin cambios en el formato de datos; habrá que actualizar las URLs lectoras una sola vez.