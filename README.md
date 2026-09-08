# Te Amo Fanisita ❤️

Dos animaciones pixel-art estilo Minecraft.

En la primera, un cofre de roble flota sobre un prado lleno de flores. Al hacer click se abre
y pregunta **¿QUIERES SER MI TODO?** con botones SÍ y NO. Cada NO insiste un poco más y
encoge el botón; el SÍ desata un letrero que dice **TE AMO FANISITA**, con el jardín
floreciendo y una lluvia de corazones.

En la segunda cae la noche: unos ojos pixelados entre las luciérnagas y un letrero que dice
**ERES LA LUZ DE MI VIDA**.

## Cómo verlas

Son dos páginas:

- **El cofre** — https://1811saldanacamacho-lgtm.github.io/te-amo-minecraft/
- **La noche de luciérnagas** — https://1811saldanacamacho-lgtm.github.io/te-amo-minecraft/luz.html

La segunda se desbloquea desde la primera: aparece un botón cuando responde que sí.

También funcionan con doble click sobre cualquiera de los dos archivos. No necesitan
internet, ni instalar nada, ni conexión a un servidor.

## La canción

Debajo de los ojos corre la letra estilo karaoke: los renglones suben solos y cada uno se
va encendiendo de izquierda a derecha, como si lo fueran cantando. Arriba y abajo quedan
los renglones vecinos apagados y desenfocados, difuminándose hacia los bordes.

**Para poner otra letra** se cambia nada más el arreglo `LETRA` al inicio del script de
`luz.html`: cada renglón es `{ t: 'TEXTO', d: segundos }`. El tamaño de la letra, el
centrado y los tiempos se acomodan solos a partir de eso. Un renglón con texto vacío sirve
de respiro entre estrofas. Sólo mayúsculas y sin acentos, que es lo que dibuja la fuente.

## La noche de luciérnagas

Unos ojos pixelados flotando en la noche, dibujados por código: la almendra del ojo, el
iris, las pestañas y la ceja se generan con curvas, no con un mapa de bits. La piel
alrededor se deshace en píxeles sueltos con difuminado ordenado, así que se funden con la
oscuridad en vez de quedar recortados. Parpadean cada cierto tiempo.

El iris usa una rampa de seis tonos elegidos a mano, con fibras radiales que salen de la
pupila, anillo limbal oscuro, la sombra que proyecta el párpado sobre el globo, línea de
agua en el párpado inferior y dos brillos (el principal y el de luz rebotada).

La mirada está trabajada con la esquina de afuera levantada, delineado que engorda hacia
ese lado y termina en un rabillo, sombra rosada pegada al párpado, brillo en el lagrimal,
cejas arqueadas con el pico en el tercio exterior, y pestañas más largas y más juntas
hacia afuera, con unas cortas por debajo.

**Las luciérnagas se reflejan dentro del iris.** Las posiciones salen de las luciérnagas
de verdad: se lee dónde está cada una en la pantalla y se comprime la escena dentro del
disco del iris, invertida, como en cualquier reflejo.

Alrededor, cielo estrellado, luna cuadrada, árboles en penumbra y luciérnagas que vuelan y
titilan. Cada click suelta chispas y deja luciérnagas nuevas.

## Qué incluye el cofre

- **Bloque de pasto isométrico**, con sus tres caras proyectadas en 2:1 como en el juego.
- **12 flores de Minecraft**: amapola, diente de león, orquídea azul, allium, azulita,
  los cuatro tulipanes (rojo, naranja, blanco y rosa), margarita, aciano y lirio de los valles.
- **Tipografía pixelada 5x7** dibujada a mano, con la sombra dura de un pixel del juego.
- Prado con árboles de roble, nubes en movimiento, sol y suelo de pasto, tierra y piedra.
- Al primer click: el bloque estalla en partículas, sale el letrero, brotan flores por todo
  el prado, llueven pétalos y suben corazones por detrás del cartel.
- Después, cada click siembra más flores y lanza más corazones.
- Sonidos 8-bit generados con WebAudio, sin archivos de audio.

## Detalles técnicos

Un solo archivo HTML, sin dependencias ni librerías externas. Todo el pixel art —flores,
corazones, árboles, texturas y letras— se genera por código a partir de mapas de caracteres
que se convierten en SVG. El contorno oscuro de cada sprite se calcula solo a partir de su
silueta, y las texturas de tierra y madera usan una variación por pixel para no verse planas.

El diseño es fluido: todas las medidas del letrero van en porcentaje, así que el mensaje se
lee completo tanto en un monitor como en la pantalla de un teléfono.
