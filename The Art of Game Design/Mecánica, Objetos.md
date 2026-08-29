Un espacio sin objetos es un espacio vacío, que pueden ser:

- **[[Personajes]]**.
- [[Objetos interactivos]]
- Tokens
- Tablas de puntuación

O lo que sea que pueda ser manipulado en mi juego.

>[!tip] Los objetos son los *sustantivos* de las [[Mecánicas de juego]].

A veces el espacio mismo puede ser un objeto.

Los objetos generalmente tienen uno o más **atributos**, entre los cuales está su posición en el [[Espacio de juego]].

>[!info] Los **atributos** son **categorías de información para un objeto**.

Otros atributos podrían ser, por ejemplo, la velocidad máximo y la velocidad actual de un automóvil. **Cada atributo tiene un *estado***, por ejemplo 150km/h y 75km/h respectivamente.

>[!info] Si los objetos son los sustantivos, **los atributos son los *adjetivos***.

Los atributos pueden ser:

- **Estáticos**
	- Atributos que nunca cambian
		- Color, tamaño, etc.
- **Dinámicos**
	- Atributos que cambian
		- Movimiento, estado, etc.

>[important] Es importante comunicar los cambios de estado esenciales al [[Jugador]].

>[!tip] Si two objetos se comportan igual, deberían verse igual. SI se comportan diferente, deberían verse diferente.

---

Muchas veces algunos objetos, especialmente personajes que simulan inteligencia, tienen tantos atributos como estados que pueden llegar a ser confusos. Por eso es útil construir un **Diagrama de estados para cada atributo para estar seguro y entender qué estados están conectados con qué y qué desencadena cambios de estado**. 

En [[Programación]] se le conoce como [[State Machine]].

![[Pasted image 20250910123509.png]]

El doble círculo (que rodea "In cage") suele usarse para decir que allí inicia el estado. Cada flecha representa **una posible transición de estado, con un evento que desencadena esa transición**.

Este tipo de diagramas son útiles para que, al momento de programar, evitemos bugs.

---
# [[Lente 28, EL Lente del State Machine]]

# Secretos

>[!important] Una decisión muy importante sobre los atributos de juego y sus estados es **quién está consciente de ellos**.

En los juegos de mesa toda la información es pública. En algunos juegos de carta, hay información tanto pública como privada (como en el Poker).

**El juego se vuelve diferente dramáticamente cuando cambiamos hacemos la información pública o privada**. Algunos juegos como Stratego o Battleship se basa en adivinar los estados de los atributos de tu oponente.

Pero en los videojuegos un nuevo tipo de estado existe: **un estado que sólo el juego en sí sabe**. Esto plantea la pregunta, #filosofía, si los oponentes virtuales, desde el punto de vista de las [[Mecánicas de juego]], deberían ser considerados como jugadores o simplemente parte del juego. 

>[!info] Cuando jugamos algunos juegos, por ejemplo Blackjack, no sólo sólo los jugadores son "entidades", sino también el *oponente virtual* y el *algoritmo* del sistema, en total 3.
> Es decir, el *jugador* tiene conciencia de su mano, el *oponente virtual* que tiene "conciencia" de su propia mano, y el *algoritmo* que sabe el estado de todos los atributos del juego.

Por ello, *desde la perspectiva del juego*, el *oponente virtual* sí podría considerarse otro jugador. **El juego en sí es otra entidad per se, cuyo estatus es especial dado que no está "jugando" el juego, pero sí permite su ejecución**.

[[Celia Pearce]] dice que hay otro tipo de información, privada de todas las entidades discutidas anteriormente: información [[Aleatoriedad|aleatoriamente]] generada.

![[Pasted image 20250910182927.png]]
*Jerarquía de sabedores.*

Cada círculo representa un "sabedor". Los sabedores son dios, el juego, los jugadores 1, 2 y 3. Cada punto representa información del juego—el estado de un atributo.

- **A**
	- Información completamente pública.
		- Posición de una pieza en el tablero, o una carta boca-arriba.
		- **Todos los jugadores saben esta información**.
- **B**
	- Es el estado que se comparte entre el jugador 2 y 3, pero se mantiene secreta del jugador 1.
		- Puede ser que J2 y J3 sean oponentes virtuales que comparten información entre ellos contra el J1 humano.
- **C**
	- Información privada tan sólo para el J2.
		- Cartas echadas, etc.
- **D**
	- La información que el [[Juego]] o [[Sistema de juego]] sabe, pero no los jugadores. **Existe información del juego que permanece oculta a los jugadores, pero que afecta las [[Mecánicas de juego]]**.
		- El Dungeon Master conoce información privada del estado del juego
- **E**
	- Información generada aleatoriamente, sabido tan sólo por el destino, dioses, etc. 
# [[Lente 29, El Lente de los Secretos]]



