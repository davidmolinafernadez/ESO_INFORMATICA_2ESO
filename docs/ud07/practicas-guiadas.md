# Prácticas guiadas con MakeCode Arcade

**Herramienta:** MakeCode Arcade en Firefox. Los bloques pueden aparecer en español o inglés; se indican ambos nombres cuando ayuda a localizarlos. No necesitas una cuenta para descargar una copia.

## AR2-1 · El coche que se mueve

1. Abre **Firefox** y entra en [MakeCode Arcade](https://arcade.makecode.com/). Pulsa **Nuevo proyecto**, escribe `AR2_1_ApellidoNombre` y pulsa **Crear**. Elige el modo **Bloques** en la parte superior.
2. En **Sprites** arrastra al bloque **al iniciar** el bloque `establecer mySprite a sprite de tipo Player`. Pulsa el cuadrito de imagen, dibuja un coche y confirma. Mantén el nombre `mySprite`.
3. En **Controlador / Controller** encaja dentro de al iniciar `mover mySprite con botones`, con velocidad X `100` e Y `100`.
4. En **Sprites** busca `establecer mySprite permanecer en pantalla` (**stay in screen**) y actívalo. Si aparece dentro de una lista de propiedades, elige esa propiedad.
5. En **Escena / Scene** añade `establecer color de fondo` dentro de al iniciar y elige un color.
6. En **Controlador** arrastra al área un evento separado `al presionar botón A`. Dentro añade **Sprites → mySprite decir texto ¡Vamos! durante 1000 ms**.
7. Prueba el simulador de la izquierda con las cuatro flechas y con el botón A. El coche debe moverse, permanecer en pantalla y mostrar el mensaje.
8. En el campo de nombre inferior escribe `AR2_1_ApellidoNombre`. Pulsa el icono de **Guardar** junto al nombre para descargar el proyecto como imagen `.png` con el código incorporado. Guárdala en `Documentos/FERIA_DIGITAL_TUNOMBRE/UD07_VIDEOJUEGO/ACTIVIDADES`. Para comprobar la copia, vuelve a Inicio → **Importar → Importar archivo** y selecciona esa imagen.
9. Abre **Menú de aplicaciones → Captura de pantalla** y guarda una captura del simulador como `AR2_1_ApellidoNombre_prueba.png`. No sustituyas con esa captura la imagen descargada que contiene el proyecto.
10. Pulsa **Compartir → Compartir proyecto** y copia el enlace generado. Abre **Menú de aplicaciones → Oficina → LibreOffice Writer**, pégalo y guarda `AR2_1_ApellidoNombre_enlace.odt`. Abre el enlace en otra pestaña para comprobarlo.

**Entrega:** imagen de proyecto descargada, captura de prueba (dos en AR2-3) y documento con el enlace. Abre **Firefox → Aules → Informática → UD07 → práctica AR2-1 → Agregar entrega**, adjunta los archivos y pulsa **Guardar cambios** y **Enviar tarea** si aparece. Si la práctica se revisa solo en clase, muestra los archivos al profesor.

## AR2-2 · Recoger monedas

1. Abre **Firefox → MakeCode Arcade**. En la página inicial abre el proyecto AR2_1. Antes de editar, cambia el nombre del campo inferior a `AR2_2_ApellidoNombre` y guarda una copia con el botón de guardar, junto al nombre. Así mantienes la descarga anterior.
2. En **Sprites** añade a **al iniciar** `establecer mySprite2 a sprite de tipo Food`. Dibuja una moneda. Mantén `mySprite` para el coche y `mySprite2` para la moneda.
3. En **Información / Info** añade a al iniciar `establecer puntuación a 0`.
4. En **Sprites** añade `establecer posición de mySprite2 x: ... y: ...`. En cada hueco coloca **Matemáticas / Math → escoger al azar**: X entre `10` y `150`; Y entre `10` y `110`.
5. Arrastra desde **Sprites** un evento independiente `al superponerse sprite de tipo Player con otherSprite de tipo Food` (**on overlap**). Dentro encaja **Información → cambiar puntuación en 1**.
6. En el mismo evento añade `establecer posición de otherSprite` y dos números aleatorios con los mismos intervalos. Usa `otherSprite`, la moneda tocada, para no mover el coche.
7. Añade al final del evento **Bucles / Loops → pausa 200 ms** para reducir repeticiones durante el contacto. Prueba y consigue cinco puntos; comprueba que la moneda cambia de lugar.
8. En el campo de nombre inferior escribe `AR2_2_ApellidoNombre`. Pulsa el icono de **Guardar** junto al nombre para descargar el proyecto como imagen `.png` con el código incorporado. Guárdala en `Documentos/FERIA_DIGITAL_TUNOMBRE/UD07_VIDEOJUEGO/ACTIVIDADES`. Para comprobar la copia, vuelve a Inicio → **Importar → Importar archivo** y selecciona esa imagen.
9. Abre **Menú de aplicaciones → Captura de pantalla** y guarda una captura del simulador como `AR2_2_ApellidoNombre_prueba.png`. No sustituyas con esa captura la imagen descargada que contiene el proyecto.
10. Pulsa **Compartir → Compartir proyecto** y copia el enlace generado. Abre **Menú de aplicaciones → Oficina → LibreOffice Writer**, pégalo y guarda `AR2_2_ApellidoNombre_enlace.odt`. Abre el enlace en otra pestaña para comprobarlo.

**Entrega:** imagen de proyecto descargada, captura de prueba (dos en AR2-3) y documento con el enlace. Abre **Firefox → Aules → Informática → UD07 → práctica AR2-2 → Agregar entrega**, adjunta los archivos y pulsa **Guardar cambios** y **Enviar tarea** si aparece. Si la práctica se revisa solo en clase, muestra los archivos al profesor.

## AR2-3 · Enemigo y final de partida

1. Abre el proyecto AR2_2 en **Firefox → MakeCode Arcade**, cambia el nombre a `AR2_3_ApellidoNombre` y descarga una copia antes de editar.
2. En **Sprites** crea dentro de **al iniciar** otro sprite llamado `enemigo`, de tipo **Enemy**. Dibuja una figura distinta del coche y de la moneda.
3. Añade `establecer posición de enemigo x: 140 y: 100` y `establecer posición de mySprite x: 20 y: 20`, para que no comiencen tocándose.
4. En **Sprites** añade `enemigo seguir mySprite a velocidad 25` dentro de al iniciar. El objetivo del seguimiento debe ser el coche.
5. Crea un evento separado **Sprites → al superponerse Player con Enemy**. Dentro añade **Juego / Game → terminar juego con derrota** (**game over: lose**).
6. En **Información / Info** añade a al iniciar `iniciar cuenta atrás de 30 segundos`. Crea el evento independiente `al terminar cuenta atrás` y dentro añade **Juego → terminar juego con victoria**.
7. Prueba una derrota dejando que el enemigo alcance el coche. Reinicia con el botón del simulador y prueba una victoria evitando al enemigo durante 30 segundos.
8. Si siempre pierdes al comenzar, revisa las posiciones iniciales y que la velocidad del coche sea 100 y la del enemigo 25. Guarda las dos capturas de prueba.
9. En el campo de nombre inferior escribe `AR2_3_ApellidoNombre`. Pulsa el icono de **Guardar** junto al nombre para descargar el proyecto como imagen `.png` con el código incorporado. Guárdala en `Documentos/FERIA_DIGITAL_TUNOMBRE/UD07_VIDEOJUEGO/ACTIVIDADES`. Para comprobar la copia, vuelve a Inicio → **Importar → Importar archivo** y selecciona esa imagen.
10. Abre **Menú de aplicaciones → Captura de pantalla** y guarda una captura del simulador como `AR2_3_ApellidoNombre_prueba.png`. Guarda una de victoria y otra de derrota con los sufijos `_victoria` y `_derrota`.
11. Pulsa **Compartir → Compartir proyecto** y copia el enlace generado. Abre **Menú de aplicaciones → Oficina → LibreOffice Writer**, pégalo y guarda `AR2_3_ApellidoNombre_enlace.odt`. Abre el enlace en otra pestaña para comprobarlo.

**Entrega:** imagen de proyecto descargada, captura de prueba (dos en AR2-3) y documento con el enlace. Abre **Firefox → Aules → Informática → UD07 → práctica AR2-3 → Agregar entrega**, adjunta los archivos y pulsa **Guardar cambios** y **Enviar tarea** si aparece. Si la práctica se revisa solo en clase, muestra los archivos al profesor.

## Reto final sencillo

Abre una copia de AR2-3 y cambia solo tres elementos: dibujo del coche (pulsa su imagen en el bloque), color de fondo (bloque de Escena) y un sonido al recoger (bloque de Música dentro del evento Player/Food). Prueba de nuevo victoria y derrota y guarda como `AR2_RETO_ApellidoNombre`.
