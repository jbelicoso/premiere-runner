# Premiere Runner

Minijuego web para practicar el flujo básico de edición en Adobe Premiere Pro:
abrir un clip en el monitor de origen, recorrerlo con **J K L**, marcar
**entrada (I)** y **salida (O)**, y arrastrarlo a la línea de tiempo pegado al
clip anterior.

Hecho para las capacitaciones de **Adobe Cursos Quito**.

- Un solo archivo HTML, sin dependencias ni instalación.
- Cada clip tiene su propia imagen y su propio **ambiente sonoro real**, que suena
  al reproducirlo en el monitor y al pasar el cabezal por encima en la línea de tiempo.
- Diez niveles, incluido uno de **reordenar la secuencia** arrastrando los clips, otro de **marcar el ritmo con la tecla M** otro de **cortar sobre esos marcadores** y un último de **ordenar los cortes según un guion** (edición con ritmo). En todos se practica el transporte con **J K L**.
- **Modo práctica** sin reloj ni vidas, pensado para quien recién empieza.
- **Modo reto** con tiempo, vidas y puntaje.
- Funciona en cualquier navegador de escritorio.

Jugar: https://jbelicoso.github.io/premiere-runner/

Créditos de los sonidos en [CREDITOS.md](CREDITOS.md) (todos CC0).

## Nota técnica sobre el audio

Cada `assets/audio/<nombre>.mp3` tiene un gemelo `assets/audio/<nombre>.js` con el mismo audio en base64.
Sirve para que el juego suene también al abrir `index.html` con doble clic (file://), donde el navegador
no deja leer los mp3 directamente. Si cambias un mp3, hay que regenerar su `.js`.
