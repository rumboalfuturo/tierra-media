# Tierra Media — un mundo de bloques

Juego tipo Minecraft ambientado en El Señor de los Anillos, con **multijugador online**, **perfiles** y **mundos guardados**. Todo el juego vive en un único `index.html` (Three.js + PeerJS desde CDN).

**▶ Jugar:** https://rumboalfuturo.github.io/tierra-media/

## Jugar con otra persona

1. Uno de los dos pulsa **«Crear partida online»**, elige (o crea) un mundo y verá un **código de 5 letras** arriba a la derecha.
2. El otro abre el mismo enlace, pulsa **«Unirse con código»** y escribe el código.
3. ¡Ya estáis en el mismo mundo! Os veréis como muñecos con vuestro nombre encima.

La conexión es directa entre los dos navegadores (P2P con WebRTC); no hay servidor de juego. En algunas redes muy restrictivas la conexión puede fallar.

## Perfiles y guardado

- **Perfil**: nombre y color, se guarda en el navegador de cada jugador.
- **Mundos**: se guardan automáticamente en el navegador del anfitrión (cada 8 segundos y al salir). El invitado juega en el mundo del anfitrión y no necesita guardar nada.
- Cada mundo tiene su propia semilla: el terreno es distinto en cada uno.

## Controles

| Tecla | Acción |
|---|---|
| W A S D | moverte |
| Espacio | saltar / nadar |
| Shift | correr |
| Mantener clic izq | picar el bloque (barra de progreso) |
| Clic derecho | colocar material / abrir cofre |
| 1–5 | herramientas: mano, pico, pala, hacha, cubo |
| 6–9 | huecos de materiales |
| E | inventario y fabricación |
| R | volver a La Comarca |
| Esc | menú |

## Herramientas, inventario y cofres

- **Pico** para piedra, **pala** para tierra/arena, **hacha** para madera — con la herramienta adecuada picas 4 veces más rápido.
- Lo que picas va a tu **inventario** (tecla E); desde ahí asignas materiales a los huecos 6–9 y fabricas: 1 tronco → 4 tablones, 8 tablones → 1 cofre.
- Los **cofres** se colocan y se abren con clic derecho; guardan materiales y se comparten entre jugadores. El del agujero hobbit trae regalo.
- El **cubo** recoge agua y lava de lagos (clic izq) para colocarlas después como materiales.

## Reacciones realistas

- La **lava quema** la hierba que toca (la deja en tierra) y prende madera y hojas: los árboles arden con fuego que se propaga.
- El **agua enfría la lava** y la convierte en piedra.
- El fuego se puede apagar de un golpe de clic.

## El mundo

- **La Comarca** — colinas verdes y robles; hay un agujero hobbit cerca del punto de aparición (con un regalo dentro).
- **Lothlórien** — bosques de mallorn con copas doradas.
- **Montañas Nubladas** — picos de roca con cumbres nevadas.
- **Mordor** — roca negra, lagos de lava, niebla rojiza y **Barad-dûr** con el Ojo ardiente en lo alto (al sureste del spawn).
- Bajo tierra hay **mithril** si excavas.
- Ciclo completo de día y noche (5 minutos).

El mundo es procedural e "infinito": se generan chunks nuevos al explorar.

## Ejecutar en local

Doble clic en `index.html`, o con servidor local: `python -m http.server 8123` y abre http://localhost:8123 (requiere internet para los CDN).
