Boca Contra el Reloj

TP 2: Boca Contra el Reloj

Descripción del juego
Boca Contra el Reloj es un juego de preguntas y respuestas sobre fútbol. El jugador debe elegir la respuesta correcta entre cuatro opciones que aparecen en pantalla. Por cada respuesta correcta obtiene 10 puntos, mientras que por cada respuesta incorrecta pierde una vida. El objetivo es conseguir la mayor cantidad de puntos posibles respondiendo todas las preguntas antes de que termine el tiempo. El jugador tiene 3 vidas y 60 segundos para jugar. La partida termina si se queda sin vidas, se acaba el tiempo o responde todas las preguntas. Al finalizar, se muestra el puntaje obtenido y aparece la opción de volver a jugar.

Árbol de decisión
```
INICIO (botón JUGAR)
        |
        v
Comienza el juego
60 segundos - 3 vidas - 0 puntos
        |
        v
  ¿Se acabó el tiempo?
      /         \
    SÍ           NO
    |             |
    v             v
 FIN: TIEMPO   Aparece una pregunta
 AGOTADO            |
    |               v
    |       ¿Respondió correctamente?
    |            /       \
    |          SÍ         NO
    |          |           |
    |          v           v
    |      +10 puntos   -1 vida
    |          |           |
    |          |           v
    |          |     ¿Quedan vidas?
    |          |       /       \
    |          |     SÍ         NO
    |          |      |          |
    |          |      |          v
    |          |      |      FIN: GAME OVER
    |          |      |          |
    |          |      |          v
    |          |      |     Mostrar puntaje
    |          |      |
    |          v      v
    |      ¿Quedan preguntas?
    |          /       \
    |        SÍ         NO
    |        |           |
    |        v           v
    |  Siguiente      FIN: TRIVIA
    |   pregunta      COMPLETADA
    |        |           |
    |        └───┐       v
    |            |  Mostrar puntaje
    |            |
    |            └── Volver a comprobar
    |                el tiempo
    |
    v
Mostrar puntaje final
        |
        v
BOTÓN VOLVER A JUGAR
```

IA usada: ChatGPT, modelo GPT-6.

Brief: Crear un juego de trivia futbolera en un único archivo index.html, con un botón de inicio, un cronómetro de 60 segundos, tres vidas, un puntaje visible, preguntas de opción múltiple y una pantalla final. El diseño debe adaptarse a celulares y computadoras.

Qué corregimos: Nada del código, solamente el README para que contenga todas las actividades.
