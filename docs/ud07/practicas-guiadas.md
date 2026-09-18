# Prácticas guiadas con MakeCode Arcade

Abre [MakeCode Arcade](https://arcade.makecode.com/) y trabaja con bloques. Guarda una copia al terminar cada sesión. Si un bloque no aparece, pregunta antes de cambiar otros bloques.

## AR2-1 · El coche que se mueve

!!! example "Ejemplo de resultado"
    El coche se desplaza con las cuatro flechas, permanece dentro de la pantalla y dice `¡Vamos!` al pulsar A.

1. Crea un proyecto llamado `AR2_1_ApellidoNombre`.
2. Crea un sprite de tipo **Player** y dibuja un coche sencillo.
3. Añade el bloque para moverlo con los botones.
4. Activa la opción para que no salga de la pantalla.
5. Cambia el color del fondo.
6. Pulsa **A** y haz que el coche diga `¡Vamos!` durante un segundo.
7. Prueba las cuatro direcciones y el botón A.

**Entrega:** enlace compartido del proyecto y una captura funcionando.

## AR2-2 · Recoger monedas

!!! example "Ejemplo de resultado"
    Al tocar la moneda, el marcador cambia de 0 a 1 y la moneda aparece en otro lugar.

1. Abre una copia de AR2-1.
2. Crea otro sprite de tipo **Food** con forma de moneda.
3. Colócalo en una posición aleatoria.
4. Añade el evento `Player overlaps Food`.
5. Dentro del evento, suma un punto.
6. Mueve la moneda a otra posición aleatoria.
7. Consigue cinco puntos para comprobarlo.

**Entrega:** `AR2_2_ApellidoNombre` compartido y captura con 5 puntos.

## AR2-3 · Enemigo y final de partida

!!! example "Ejemplo de resultado"
    Si el enemigo toca al coche aparece la pantalla de derrota; si termina el tiempo sin choque aparece victoria.

1. Abre una copia de AR2-2.
2. Crea un sprite **Enemy** sencillo.
3. Haz que siga al jugador a velocidad baja.
4. Añade el evento de choque entre Player y Enemy.
5. Dentro, termina la partida con derrota.
6. Añade una cuenta atrás de 30 segundos.
7. Prueba una victoria y una derrota.

**Entrega:** enlace del juego y dos capturas: victoria y derrota.

## Reto final sencillo

Cambia únicamente tres elementos: personaje, fondo y sonido. No añadas nuevas mecánicas hasta que el juego básico funcione.
