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
| Clic izquierdo | un golpe por clic (mantén pulsado para golpear seguido) |
| Clic derecho | colocar material / abrir cofre |
| 1–5 | herramientas: mano, pico, pala, hacha, cubo |
| 6–9 | huecos de materiales |
| E | inventario y fabricación |
| M | mapa de la Tierra Media |
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

## 🌱 Vida y agricultura

- **Barra de vida** (corazones): recibes daño de la lava, el fuego, las caídas grandes y al ahogarte; te recuperas solo con el tiempo si estás a salvo.
- **Labrar y sembrar**: con la **pala** (clic derecho) conviertes hierba/tierra en *tierra arada*; siembra semillas de **galenas** (hierba para pipa) y **cebada** con clic derecho. Crecen solas con el tiempo; coséchalas con un golpe.
  - Al romper hierba a veces caen semillas; las galenas crecen silvestres en La Comarca.
- **Athelas**: planta medicinal verde muy rara de Lothlórien. Úsala desde el inventario para **curarte al instante y limpiar el veneno**.
- **Pipa** (4 tablones): fúmala con hierba para pipa → humo relajante y **regeneración acelerada**.
- **Cerveza**: con cebada y tablones fabricas un **Barril**; colócalo y clic derecho para servir jarras. Bébelas para ganar **fuerza** (picas más rápido y corres más).
- **Mallorn dorado**: planta una nuez de mallorn y crecerá un árbol de madera blanca y **hojas de oro que iluminan la zona de noche**.
- Tu inventario (tecla **E**) tiene ahora una sección de **Objetos** (cosecha y comida) con botones para usarlos.

## ⛏️ Minerales y metalurgia

Excavando bajo tierra encuentras **vetas de mineral**: hierro (común), oro, **plata élfica** (bajo los bosques), **hierro negro** (cerca de la lava y en Mordor) y **mithril** (en lo más profundo).

- **Forja (alto horno)**: fabrica una y colócala; clic derecho para abrirla.
  - **Fundir**: mineral → lingote; 2 lingotes de hierro → **acero de Gondor**; oro → pepitas o bloque de oro.
  - **Forjar**:
    - **Herramientas** (hierro/acero/mithril): picas, cavas y talas mucho más rápido.
    - **Armaduras** (hierro/acero/hierro negro/mithril): reducen el daño que recibes. El **hierro negro** es el más recio pero pesa; el **mithril** es ligero (corres más) y **te hace inmune al fuego y la lava**.
    - **Armas** (espada de hierro, espada de Gondor, daga élfica, cimitarra negra, espada de mithril): listas para los enemigos que llegarán.
- Abajo a la izquierda se ve tu equipo actual (⚒ herramientas · 🛡 armadura · ⚔ arma).

## ⚔️ Enemigos y combate

Al **caer la noche** aparecen enemigos (de día solo en Mordor, que siempre es hostil). Atácalos con **clic izquierdo** (apuntando a ellos): tu espada hace más daño cuanto mejor sea. ¡Equípate antes de salir de noche!

- **Orcos**: salen de noche y siempre en Mordor. Sueltan **hierro negro** y a veces piel de huargo.
- **Uruk-hai**: más altos y fuertes, cerca de Isengard. Sueltan más hierro negro y a veces un estandarte de la Mano Blanca.
- **Arañas de Mirkwood**: rápidas, en los bosques de noche; su mordisco te **envenena** (cúrate con athelas). Sueltan telaraña élfica.
- **Nazgûl**: jefe muy raro de la noche profunda. Su grito te **paraliza de miedo** (la pantalla se oscurece y te frena). Derrótalo para conseguir una **Hoja de Morgul**, que puedes empuñar como el arma más letal del juego.

El **hierro negro** que sueltan los enemigos es justo lo que necesitas para forjar la armadura más recia: derrota orcos → forja equipo pesado. En multijugador los enemigos los lleva el anfitrión y os pueden atacar a los dos.

## El mapa de la Tierra Media

Pulsa **M** para ver el mapa con tu posición. Los lugares famosos están construidos en el mundo, dispuestos como en el mapa real (el este queda a +x y el sur a +z):

- **La Comarca** — el punto de aparición, con su agujero hobbit con puerta de madera (y un cofre con regalo).
- **Moria** — las Puertas de Durin con su arco de ithildin (mithril) y los dos acebos, en la cara oeste de las **Montañas Nubladas**; dentro, la sala de pilares de Khazad-dûm y una grieta de lava.
- **Lothlórien** — el Bosque Dorado, al este de Moria, como debe ser.
- **Isengard** — anillo de roca con casa-puerta de torres gemelas, portón de madera, fosas ardientes y la torre negra de **Orthanc** con sus cuatro cuernos.
- **El Abismo de Helm** — el Muro del Bajo curvado con adarve, almenas y su alcantarilla; el espolón de roca con la Cuernavilla, la torre del Gran Cuerno y la calzada que sube a su portón.
- **Minas Tirith** — la ciudad blanca de siete niveles con el espolón de proa, la Gran Puerta de madera y la Torre de Ecthelion, sobre los campos del Pelennor.
- **El río Anduin** — serpentea de norte a sur, con el puente de **Osgiliath** frente a Minas Tirith.
- **Mordor** — al sureste: roca negra, lagos de lava, niebla rojiza y **Barad-dûr** con el Ojo ardiente.
- **Puertas de madera** en todas las fortalezas: clic derecho para abrirlas y cerrarlas (los portones de varias hojas se abren enteros). Se fabrican con 4 tablones. Y sí: arden.
- Al romper un bloque, el material **cae al suelo** junto al agujero: acércate y lo recoges solo.
- Bajo tierra hay **mithril** si excavas. Ciclo completo de día y noche (5 minutos).

El mundo es procedural e "infinito": se generan chunks nuevos al explorar. Cada mundo tiene un terreno distinto, pero los monumentos están siempre en su sitio.

## Ejecutar en local

Doble clic en `index.html`, o con servidor local: `python -m http.server 8123` y abre http://localhost:8123 (requiere internet para los CDN).
