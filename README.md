  <p style="text-align: right;margin: 0;">Universidad Complutense de Madrid</p>
  <p style="text-align: right;margin: 0;">Master Data Science, Big Data & Business Analytics</p>
  <p style="text-align: right;margin: 0;">José Javier Galán</p>
  <p style="text-align: right;margin: 0;">María Carolina González Bernal</p>
  <p style="text-align: right;margin: 0;">Python básico I</p>
  <p style="text-align: right;font-size: 14px; margin: 0;">20 de noviembre de 2025</p>

<div style="display: flex; justify-content: center; align-items: center; margin-top: 20px;">
<img src="https://www.svgrepo.com/show/37183/slut-machine-with-handle.svg", width="60" height="65", style="margin-left: 10px;">
 <p style="color: #000000; font-size: 28px; font-weight: bold; margin: 0; text-aling: center">
    Adivina    el número
  </p>
</div>

Mediante el desarrollo del siguiente **juego de adivinanza en Python** deberá utilizarse todo lo aprendido sobre lo básico de python, valorando la correcta decisión en el uso de los algoritmos.   

La estructura del juego será la siguente:

### Menú principal

Al comenzar el juego y durante el desarrollo del mismo, las opciones que se muestran hasta elegir la opción salir son:

1. **Partida modo solitario**
   *(Modo solitario supone que el número a adivinar es generado aleatoriamente por el ordenador).*
2. **Partida 2 Jugadores**
   *(Primero se escribe un número a adivinar y luego un segundo jugador intenta adivinarlo).*
3. **Estadística**
   *(Mostrará los datos almacenados en el fichero Excel, donde se podrá observar el historial de partidas jugadas).*
4. **Salir**

#### Submenú de dificultad

Tanto la opción 1 como la opción 2 tendrán un submenú para elegir la dificultad.     
En ambos menús debe chequearse que la opción elegida es válida y avisar en caso contrario.    

1. **Fácil** (20 intentos)
2. **Medio** (12 intentos)
3. **Difícil** (5 intentos)

### Reglas del juego
* El número a adivinar debe ser entre **1 y 1000**.
* Si se adivina el número, se gana la partida y se vuelve al menú principal.
* Si no se adivina, el programa debe indicar si el número buscado es **mayor o menor**.
* Si se supera el número de intentos, se pierde y se vuelve al menú principal.

### Registro de resultados

* Al finalizar cada partida (ya sea ganada o perdida), se pide el **nombre del jugador**.
* Se guarda esta información junto con el resultado de la partida en un **fichero Excel**.