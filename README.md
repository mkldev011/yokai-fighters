# Yo-Kai Watch: Survivors ·

Bullet-heaven con Yo-kais al estilo de Survivor.io, con sprites de los juegos de la saga, capa roguelike, **más de 100 Yo-kai de todas las tribus** (Valiente, Misterioso, Robusto, Guapo, Amable, Escurridizo, Siniestro y Legendarios), medallas y la clásica **Expendekai (gacha) por tribu**. Música y efectos adaptados para el juego.

HTML + CSS + JavaScript vanilla sobre Canvas 2D. Sin build, sin dependencias y **todo local**: no necesita internet para jugar.

> **Aviso sobre criptomonedas / Crypto disclaimer**
> Yo-Kai Watch: Survivors **no tiene ninguna criptomoneda, token ni NFT oficial**, y nadie del equipo ha creado ninguno. Cualquier token que use el nombre del juego lo han creado terceros ajenos al proyecto. **No nos hacemos cargo de ninguna compra, venta o inversión** que hagas con ellos y nada de lo que hay aquí es una recomendación de inversión. El juego es gratis y lo seguirá siendo.
> This fan game has **no official cryptocurrency, token or NFT**. Any token using the game's name was created by third parties. **We take no responsibility for any purchase, sale or investment** you make with them. The game is free and will stay free.

## Jugar

Doble clic en `index.html`. Crea una cuenta o entra como invitado, haz el test de personalidad con el Yo-kai Watch y directo a la mazmorra.

| Tecla | Acción |
| --- | --- |
| `W` `A` `S` `D` / flechas | Moverse |
| `1` `2` `3` `4` | Elegir el movimiento activo |
| `Q` / `E` | Ciclar movimientos |
| `Esc` / `P` | Pausa |

**En móvil o tablet** (en horizontal): pon el dedo en cualquier sitio y arrastra para moverte (el joystick aparece donde tocas), toca un ataque de abajo para cambiarlo y el botón de arriba a la derecha para pausar. Se puede instalar como app ("Añadir a pantalla de inicio"). En **Ajustes** hay sonido, calidad gráfica (con modo automático), números de daño, menos sacudidas, FPS y la gestión de la cuenta.

El Yo-kai ataca solo con el movimiento activo (o con todos los de un **vínculo / Animáximum**: cada jefe o Yo-kai legendario vencido deja fusionar técnicas para lanzarlas a la vez desde un solo hueco, hasta 4). Las rocas, cofres y los arbustos se rompen; las paredes y los árboles bloquean los disparos enemigos; el agua frena y el fuego o la lava queman (afectando también a los enemigos).

En el mapa hay **altares de poder**, **manantiales sagrados** que curan, **cofres con candado** (quédate a su lado unos segundos para abrirlos) y **trampas** que también dañan a los enemigos. A veces se abre una **grieta dimensional**: entra y te enfrentarás a un **jefe legendario u Oni** (como Gargaros u Ogralus) en una arena aparte.

Hay **tabla de elementos y tribus** (por ejemplo, los ataques de fuego hacen más daño a los Yo-kai débiles a ese elemento) y, de vez en cuando, **climas** (soleado, lluvia, tormenta de arena, ventisca) que potencian unos atributos y debilitan otros.

Cada día hay **misiones** (y semanales) que otorgan puntos y monedas; los **logros** desbloquean medallas y títulos, y tu **perfil** muestra tus 3 Yo-kai favoritos, tus récords y tus medallas conseguidas. En las partidas encuentras **objetos de equipamiento y comida** (Chocobarritas, Hamburguesas, Estampitas...) y tus técnicas **evolucionan** al alcanzar el nivel máximo. Los enemigos tienen comportamientos variados: curan, ponen escudos, llaman a su manada o avisan de su ataque en el suelo antes de golpear.

Las **mejoras** se aplican a cada Yo-kai individualmente. El **gacha (Expendekai)** funciona con **monedas** que se consiguen jugando (monedas rojas, naranjas, amarillas, moradas o especiales de jefes y legendarios), y se tira en una máquina tragaperras de estilo retro.

Cada enemigo tiene una probabilidad de 1/4096 de salir en **versión especial / variocolor (Shiny)**: brilla, una flecha en el borde de la pantalla te indica su posición, y si lo derrotas te lo quedas para siempre. En la Expendekai sale en versión especial 1 de cada 100 tiradas. En la colección puedes elegir si quieres llevar a tu compañero en su aspecto normal o especial.

La música suena tras el primer clic (los navegadores bloquean el sonido automático inicial). Para ajustar el volumen o silenciar, usa el botón del altavoz arriba a la derecha o hazlo desde el menú de pausa.

El guardado se almacena en el `localStorage` del navegador: si borras los datos del sitio web, se perderá el progreso local.

En la carpeta `videos/` hay grabaciones del juego (con su música original): un combate contra un jefe de la parca, la captura de un Yo-kai especial salvaje y una tirada afortunada en la Expendekai.

## Guardado en la nube y publicación

* **Base de datos (Firebase):** cuentas con usuario + contraseña o Google, para continuar la partida en cualquier ordenador. Pasos detallados en [docs/FIREBASE.md](https://www.google.com/search?q=docs/FIREBASE.md). Sin configurar, el juego guarda únicamente en el navegador de forma local.
* **Jugar con amigos (hasta 4) y ranking:** con cuenta en la nube, usa el menú **Amigos** (añadir por apodo, invitar a salas privadas) y el **Ranking** (tiempo aguantado: en solitario o en grupo, diario o histórico, filtrado por amigos o por Yo-kai).
* **Publicar gratis en GitHub Pages:** [docs/PUBLICAR.md](https://www.google.com/search?q=docs/PUBLICAR.md).
* Si se juega en dos dispositivos a la vez o sin conexión, las partidas se **fusionan**: las colecciones se combinan (nunca se pierde un Yo-kai ni una variante especial), las mejoras y estadísticas se actualizan con el valor máximo, y las monedas o el compañero activo se quedan con la versión más reciente. Los cambios de otro equipo se sincronizan en directo.

## Licencia

Código bajo [PolyForm Noncommercial 1.0.0](https://www.google.com/search?q=LICENSE-NONCOMMERCIAL.md): se puede usar, estudiar y modificar, pero **no con fines comerciales** (ni vender el juego ni cobrar nada dentro de él). Los sprites, la fuente tipográfica y los elementos de Yo-kai Watch tienen sus propias condiciones de uso por parte de los creadores originales (Level-5). Proyecto de fan sin ánimo de lucro.

**La única web oficial es la del proyecto.** El juego es y será totalmente gratuito: si alguien te pide dinero, no somos nosotros.

## Estructura

```
index.html              pantallas + orden de carga
css/style.css           interfaz inspirada en los menús de Yo-kai Watch
assets/yokai/{id}/      hojas de sprites (Idle, Walk, Attack, Shoot, Charge, Hurt, Faint)
assets/yokai/{id}/s/    las mismas en versión especial / variocolor
assets/fonts/           Fuentes retro y de estilo píxel optimizadas
js/
  net/                  social (apodo, amigos, salas), red (WebRTC + relé),
                        coop (partida en grupo), ranking
  core/                 util, db (guardado), audio (sintetizador + efectos), input,
                        sprites (animador), camera
  data/                 yokai-dex*, sprites-meta*, moves, starters (+ test), enemies,
                        upgrades, music (partituras)
  world/                tiles (pixel art en código), terreno, objetos, colisiones
  entities/             player, enemy, projectile, pickup, fx
  systems/              combat, spawner, levelup, gacha
  ui/                   icons (pixel art), ui, hud, login, test, menu, gacha-ui, run-ui,
                        social-ui, ranking-ui
  game.js               flujo y bucle principal
tools/                  scripts que regeneran los ficheros marcados con *

```

`*` = generado. Para regenerarlos (requiere Python 3 + Pillow e internet, solo la primera vez):

```
python tools/fetch_sprites.py     # sprites normales y especiales + js/data/sprites-meta.js
python tools/fetch_pokedex.py     # js/data/yokai-dex.js
python tools/fetch_credits.py     # CREDITS.md

```

## Notas de implementación

* **Sprites y Animaciones.** Columnas = fotogramas, filas = direcciones de movimiento. Cada animación maneja su propio tamaño de fotograma, alineándose mediante el ancla al suelo para evitar saltos visuales al atacar.
* **Coordenadas.** Las coordenadas `(x, y)` de cada entidad representan sus **pies**. Las colisiones ocurren en el plano del suelo; los proyectiles viajan por ese plano y se dibujan con una sombra inferior para dar sensación de profundidad.
* **Mundo.** Chunks de 16×16 tiles: los datos de terreno y objetos son ligeros y se generan constantemente; la imagen visual se procesa a resolución de arte escribiendo en un `ImageData` (de forma muy eficiente en Chrome) únicamente para las zonas visibles.
* **Rendimiento.** Emplea una rejilla espacial de enemigos que se reconstruye en cada fotograma. Con cientos de enemigos simultáneos, la simulación y el renderizado completo se mantienen en valores mínimos por frame en navegadores modernos.
* **Metadatos en `.js` en lugar de `.json**`, para evitar restricciones al abrir el juego localmente (`file://`).
* **Variantes Especiales (Shiny).** Las versiones especiales utilizan paletas de colores alternativas guardadas de forma optimizada para mantener un peso mínimo en memoria y disco.
* **Audio.** Sintetizador basado en Web Audio API con planificación anticipada de notas y efectos de sonido optimizados para evitar saturaciones cuando se golpea a una gran cantidad de enemigos a la vez.
* **Iconos.** Elementos gráficos convertidos dinámicamente a canvas y data URLs para garantizar que los píxeles se mantengan nítidos a cualquier escala.

## Créditos y licencia

Sprites y recursos gráficos obtenidos de repositorios de la comunidad bajo términos de uso **no comercial** y con atribución a sus respectivos autores. Yo-kai Watch y todos sus personajes son propiedad intelectual de **LEVEL-5**. Proyecto de fan sin ánimo de lucro creado puramente por pasión.
