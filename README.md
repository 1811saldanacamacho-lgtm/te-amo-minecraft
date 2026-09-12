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

Abajo, sobre el pasto, una pareja chiquita baila tomada de la mano, vestida de fiesta: él
de traje con camisa y corbata, ella de vestido negro. Los cuerpos se arman por partes sobre
una rejilla de 26×36: una "pose" dice dónde van codos, manos, rodillas y pies, y alternando
tres poses se ve el baile. La mano de adentro se queda quieta a la altura del hombro —es la
que va tomada— y el baile lo hacen el otro brazo y las piernas. La chica es el mismo dibujo
en espejo, encimado apenas para que las manos se junten. El canto de arriba a la izquierda
de cada figura va aclarado, del lado por donde les da la luna.

Los negros de la ropa no son negro puro: contra un cielo así de oscuro se perderían y lo
que se vería sería un hueco. Van en gris azulado, que es como se ve la ropa negra de noche.

A los lados hay **dos torres de luces de baile**. La estructura es una celosía de píxeles;
de cada cabezal salen tres haces de color —rosa, azul y violeta— que barren el cielo a
distinto ritmo, y la de la derecha barre al revés para que los haces se crucen.

**Para poner otra letra** se cambia nada más el arreglo `LETRA` al inicio del script de
`luz.html`: cada renglón es `{ t: 'TEXTO', d: segundos }`. El tamaño de la letra, el
centrado y los tiempos se acomodan solos a partir de eso. Un renglón con texto vacío sirve
de respiro entre estrofas.

## La fuente

Está dibujada a mano, píxel por píxel, y no depende de ninguna fuente instalada. Cada letra
mide 5×7; encima se reservan dos filas para los acentos y abajo una para la sombra dura del
juego, así que la caja completa es de 5×10.

Admite **acentos** (á é í ó ú, à è ì ò ù, ä ë ï ö ü, â ê î ô û), **ñ**, **¿ ¡**, los
**números 0-9**, signos (`. , : ; - _ ' " ( ) / + < > & ! ?`) y un **corazón ♥**. Se escribe
en minúsculas o mayúsculas indistintamente: la fuente pasa todo a mayúsculas. Si llega un
carácter que no conoce, le quita el acento y dibuja la letra sin él en vez de dejar un hueco.

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
