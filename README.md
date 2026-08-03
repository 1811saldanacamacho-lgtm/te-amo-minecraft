# Te Amo Fanisita ❤️

Animación pixel-art estilo Minecraft: un bloque de pasto flota sobre un prado lleno de flores.
Al hacer click el bloque se rompe y aparece un letrero de roble que dice **TE AMO FANISITA**,
mientras el jardín florece y llueven corazones.

## Cómo verla

En línea: **https://1811saldanacamacho-lgtm.github.io/te-amo-minecraft/**

O abre `index.html` con doble click en cualquier navegador. No necesita internet,
ni instalar nada, ni conexión a un servidor.

## Qué incluye

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
