# Te Amo — Minecraft ❤️

Animación pixel-art estilo Minecraft: al hacer click, el bloque de pasto se rompe y aparece
un letrero de madera que dice **TE AMO**, con lluvia de corazones.

## Cómo verla

En línea: **https://1811saldanacamacho-lgtm.github.io/te-amo-minecraft/**

O abre `index.html` con doble click en cualquier navegador. No necesita internet,
ni instalar nada, ni conexión a un servidor.

## Qué incluye

- Texturas de bloque de pasto y corazones generadas por código como SVG pixelado (nada de imágenes externas).
- Cielo con nubes en movimiento, sol y suelo de bloques que se repite a cualquier ancho de pantalla.
- Al primer click: el bloque tiembla, estalla en partículas y aparece el letrero de madera.
- Después de eso, cada click lanza más corazones desde donde apuntes.
- Sonidos 8-bit generados con WebAudio, sin archivos de audio.

## Detalles técnicos

Un solo archivo HTML, sin dependencias ni librerías externas. Todo el pixel art se dibuja
a partir de mapas de bits definidos en JavaScript; el contorno oscuro y las sombras del
corazón se calculan solos a partir de la silueta.
