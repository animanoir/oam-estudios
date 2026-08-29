Tiene interacción con las otras 6 mecánicas:

- [[Mecánica, Habilidad]]
- [[Mecánica, Espacio]]
- [[Mecánica, Tiempo]]
- [[Mecánica, Objetos]]
- [[Mecánica, Acciones]]
- [[Mecánica, Reglas]]
- [[Aleatoriedad]].

Esta mecánica es esencial ya que el chance quiere decir incertidumbre y la incertidumbre quiere decir [[Lente 4, La Sorpresa|sorpresa]], que a su vez puede querer decir *placer* y un ingrediente secreto de **diversión**.
# La invención de la Probabilidad

Según los inventores de la ciencia de la probabilidad fueron Blaise Pascal y Pierre de Fermat, esto porque Antoine Gombaud había calculado una manera de ganar más *frecuentemente* los dados, pero al inventar un nuevo juego, donde al tirar un par de dados, él ganaba si sale al menos un 12. Pero el pendejo erró en sus cálculos y pensó que ambos juegos tenían la misma oportunidad, lo cual no era cierto.
## 10 reglas de probabilidad que todo diseñador de juegos debería saber

### 1. Las Fracciones son Decimales son Porcentajes

$$
\frac{1}{2} = 0.5 = 50\%
$$

**Las fracciones, los decimales y los porcentajes son diferentes maneras de describir los mismos números.**

Por ejemplo, para convertir $\frac{33}{50}$ a decimal basta con ${33}\div{50} = 0.66$. 
### 2. De Cero a Uno—¡y eso es todo!

**Las probabilidades sólo pueden rondar entre $0\%$ y $100\%$**, ni más ni menos. Si en mis cálculos me aparece algo mayor a $100\%$ es que está mal hecho.
### 3. "Lo buscado" dividido entre "Resultados Posibles" es igual a Probabilidad

>[!tip] La probabilidad es **tomar el número de veces que tu resultado "buscado" puede aparecer y lo divides entre el número de resultados posibles (asumiendo que tus resultados son igualmente probables, y lo tienes**.

Ejemplos:

¿Cuál es la probabilidad de que el 6 caiga al tirar un dado?

$1 \div 6 = \frac{1}{6} = 17\% = 0.1667$

¿Cuál es la probabilidad de que salga un número par cuando lanzas un dado? Hay 3 números pares en el dado (2, 4, 6)

$3\div6 = \frac{3}{6} = 50\% = 0.5$

¿Cuál es la probabilidad de sacar una carta de figura de un deck de cartas? Hay 12 cartas de figura en una baraja de 52 cartas en total.

$12\div52 = \frac{12}{52} = 23\% = 0.2308$
### 4. Enumera!

A veces los 2 números que necesitamos para obtener la probabilidad (*lo buscado* y *resultados posibles*) no siempre son tan obvios. Por ejemplo, si me pregunto cuáles son las probabilidades de lanzar una moneda tres veces y obtener "cara" al menos 2 veces, ¿cuál es el número de resultados "buscados"? Es fácil encontrar la respuesta al enumerar todos los resultados posibles:

- CCC
- CCX
- CXC
- CXX
- XCC
- XCX
- XXC
- XXX

Hay exactamente 8 resultados posibles, y cae al menos 2 veces cara en 4. Eso es 4 resultados de 8 posibilidades, así que la respuesta es $\frac{4}{8} = 50\%$. 

Enumerar es útil, pero sólo cuando los números no son astronómicos.
### 5. En ciertas casos, OR (o) quiere decir Add (sumar)

#importante A menudo queremos determinar las posibilidades de que suceda "eso O aquello", como ¿cuáles son las posibilidades de sacar una carta de figura O un as de una baraja de cartas? **Cuando las dos cosas de las que estamos hablando son *mutuamente excluyentes*, es decir, cuando es imposible que ambas sucedan simultáneamente, puedes *sumar sus probabilidades individuales para obtener una probabilidad general***.

Por ejemplo, las posibilidades de sacar una carta de figura son $\frac{12}{52}$, y las posibilidades de sacar un as son $\frac{4}{52}$. Como estos son eventos mutuamente excluyentes (es imposible que ambos sucedan a la vez), podemos sumarlos:

$\frac{12}{52} + \frac{4}{52} = \frac{16}{52} = 31\%$.

Otro ejemplo más sencillo de entender es con pizzas:

¿Cuál es la probabilidad de que alguien pida una pizza de pepperoni O pizza de jamón? No puedo pedir ambas al mismo tiempo (sólo puedo elegir una). **Si pepperoni tiene 30% y jamón tiene 25%, entonces $30\% + 25\% = 55\%$**. Otro ejemplo es la probabilidad de que llueva O haga sol.

Ahora, cuando **no deberíamos sumar** es **cuando los eventos que SÍ pueden ocurrir juntos**, como por ejemplo:

¿Cuál es la probabilidad de que Juan sea alto O que use lentes?. Juan PUEDE ser alto Y usar lentes al mismo tiempo. Si sumo las probabilidades estaría contando a "Juan alto con lentes" dos veces.

**El ejemplo de las cartas:**

- As de diamantes cuenta como "as" Y como "diamante"
- Si sumas 4/52 + 13/52 = 17/52, estás contando el as de diamantes dos veces
- La respuesta correcta es 16/52 (porque 4 ases + 12 diamantes restantes = 16)

>[!important] Sólo suma probabilidades cuando los eventos NO puedan ocurrir al mismo tiempo.
### 6. En ciertos casos, AND (Y) significa Multiplicar

Esta regla es casi la opuesta a la [[Mecánica, Chance#5. En ciertas casos, OR (o) quiere decir Add (sumar)|anterior]].**Si queremos encontrar la probabilidad de que dos cosas sucedan simultáneamente, podemos multiplicar sus probabilidades para obtener la respuesta, *pero SÓLO si los dos eventos NO son mutuamente excluyentes!***

---

Traducción completa de la regla 6:

**Regla #6: En Ciertos Casos, Y Significa Multiplicar**

¡Esta regla es casi lo opuesto de la anterior! Si queremos encontrar la probabilidad de que dos cosas sucedan simultáneamente, podemos multiplicar sus probabilidades para obtener la respuesta—¡pero SOLO si los dos eventos NO son mutuamente excluyentes! Considera dos lanzamientos de dados. Si queremos encontrar la probabilidad de sacar un seis en ambos lanzamientos, podemos multiplicar las probabilidades de los dos eventos: La posibilidad de obtener un seis en un lanzamiento de dado es 1/6, y también 1/6 para un segundo lanzamiento. Así que la posibilidad de obtener dos seis es 1/6 × 1/6 = 1/36. También podrías haber determinado eso por enumeración, por supuesto, pero esta es una forma mucho más rápida de hacerlo.

En la Regla #5, preguntamos por la probabilidad de sacar un as O un diamante de una baraja de cartas—la regla falló, porque los dos eventos no eran mutuamente excluyentes. Entonces, ¿qué pasa si preguntamos sobre la probabilidad de sacar un as Y un diamante? En otras palabras, ¿cuál es la probabilidad de sacar el as de diamantes? Debería ser bastante intuitivo que la respuesta es 1/52, pero podemos verificar eso con la Regla #6, ya que sabemos que los dos eventos no son mutuamente excluyentes. La posibilidad de obtener un as es 4/52, y la posibilidad de un diamante es 13/52. Multiplicándolas, 4/52 × 13/52 = 52/2704 = 1/52. Así que la regla funciona y coincide con nuestra intuición.

¿Tenemos suficientes reglas para resolver los problemas del Chevalier? Consideremos su primer juego:

**Primer Juego:** En cuatro lanzamientos de un solo dado, el Chevalier gana si sale al menos un seis.

Ya hemos establecido que podríamos enumerar esto y obtener la respuesta 671/1296, pero eso tomaría una hora. ¿Hay una forma más rápida, usando las reglas que tenemos?

(Te advierto ahora—esto se pone un poco complicado. Si realmente no te importa tanto, ahórrate el dolor de cabeza y simplemente salta a la Regla #7. Si sí te importa, entonces continúa—encontrarás que vale la pena el esfuerzo.)

Si la pregunta fuera sobre las posibilidades de lanzar un dado cuatro veces y obtener cuatro seis, esa sería una pregunta de Y para cuatro eventos que no son mutuamente excluyentes, y simplemente podríamos usar la Regla #6: 1/6 × 1/6 × 1/6 × 1/6 = 1/1296. Pero eso no es lo que se pregunta. Esta es una pregunta de O para cuatro eventos que no son mutuamente excluyentes (es posible que el Chevalier obtenga múltiples seis en los cuatro lanzamientos). Entonces, ¿qué podemos hacer? Bueno, una forma es desglosarlo en eventos que son mutuamente excluyentes y luego sumarlos. Otra forma de expresar este juego es:

¿Cuáles son las posibilidades de lanzar cuatro dados y obtener ya sea a. Cuatro seis, O b. Tres seis y un no-seis, O c. Dos seis y dos no-seis, O d. Un seis y tres no-seis

Eso puede sonar un poco complicado, pero son cuatro eventos mutuamente excluyentes diferentes, y si podemos calcular la probabilidad de cada uno, simplemente podemos sumarlos y obtener nuestra respuesta. Ya hemos calculado la probabilidad de (a), usando la Regla #6: 1/1296. Entonces, ¿qué hay de (b)? Realmente, (b) son cuatro posibilidades mutuamente excluyentes diferentes:

1. 6, 6, 6, no-seis
2. 6, 6, no-seis, 6
3. 6, no-seis, 6, 6
4. No-seis, 6, 6, 6

La probabilidad de sacar un seis es 1/6, la probabilidad de sacar un no-seis es 5/6. Así que la probabilidad de cada una de esas es 1/6 × 1/6 × 1/6 × 5/6 = 5/1296. Ahora, si sumamos las cuatro, eso da 20/1296. Así que la probabilidad de (b) es 20/1296.

¿Qué hay de (c)? Esta es igual que la anterior, pero hay más combinaciones. Es complicado calcular cuántas formas hay para que salgan exactamente dos seis y dos no-seis, pero hay seis formas:

1. 6, 6, no-seis, no-seis
2. 6, no-seis, 6, no-seis
3. 6, no-seis, no-seis, 6
4. no-seis, 6, 6, no-seis
5. no-seis, 6, no-seis, 6
6. no-seis, no-seis, 6, 6

Y la probabilidad de cada una de estas es 1/6 × 1/6 × 5/6 × 5/6 = 25/1296. Sumar las seis da 150/1296.

Esto deja solo (d), que es el inverso de (b):

a. No-seis, no-seis, no-seis, 6 b. No-seis, no-seis, 6, no-seis c. No-seis, 6, no-seis, no-seis d. 6, no-seis, no-seis, no-seis

La probabilidad de cada una es 5/6 × 5/6 × 5/6 × 1/6 = 125/1296. Sumar las cuatro da 500/1296.

Así que ahora hemos calculado la probabilidad de los cuatro eventos mutuamente excluyentes:

a. Cuatro seis—(1/1296) b. Tres seis y un no-seis—(20/1296) c. Dos seis y dos no-seis—(150/1296) d. Un seis y tres no-seis—(500/1296)

Sumar esas cuatro probabilidades (como permite la Regla #5) nos da un total de 671/1296, o aproximadamente 51.77%. Así que podemos ver que este era un buen juego para el Chevalier—al ganar más del 50% de las veces, eventualmente era probable que obtuviera una ganancia, pero el juego estaba lo suficientemente cerca del equilibrio como para que sus amigos creyeran que tenían una oportunidad—al menos por un tiempo. ¡Ciertamente es un resultado muy diferente del 66% de posibilidades de ganar que el Chevalier creía que tenía!

Esta es la misma respuesta que podríamos haber obtenido de la enumeración, pero mucho más rápido. Realmente, sin embargo, hicimos una especie de enumeración—es solo que las reglas de suma y multiplicación nos permiten contar todo mucho más rápido. ¿Podríamos hacer lo mismo para obtener la respuesta al segundo juego del Chevalier? Podríamos, ¡pero con 24 lanzamientos de dos dados, probablemente tomaría una hora o más! Esto es más rápido que la enumeración, pero podemos hacerlo aún mejor siendo astutos—ahí es donde entra la Regla #7.

---

Ejemplo de IA:

## **Analogía del Restaurante para la Regla #6**

Imagina que vas a un restaurante que tiene un menú especial:

### **CUÁNDO MULTIPLICAS (Eventos Independientes):**

**Situación:** Quieres ir al restaurante dos días seguidos y pedir tu plato favorito cada día.

- **Día 1:** Probabilidad de que tengan tu plato favorito = 80%
- **Día 2:** Probabilidad de que tengan tu plato favorito = 80%
- **Probabilidad de que lo tengan AMBOS días:** 80% × 80% = 64%

Es como el ejemplo de los dados: cada día es independiente del otro.

### **LA COMPLICACIÓN DEL CHEVALIER:**

El Chevalier quería calcular: _"¿Cuál es la probabilidad de que salga al menos un 6 en 4 lanzamientos?"_

**Esto es como preguntar:** _"¿Cuál es la probabilidad de que el restaurante tenga mi plato favorito al menos uno de los próximos 4 días?"_

### **EL MÉTODO LARGO (pero correcto):**

**Desglosamos todas las formas de "al menos una vez":**

1. **Lo tienen exactamente 4 días** (como sacar 4 seises)
2. **Lo tienen exactamente 3 días** (como sacar 3 seises)
3. **Lo tienen exactamente 2 días** (como sacar 2 seises)
4. **Lo tienen exactamente 1 día** (como sacar 1 seis)

**Para cada caso:**

- Calculamos la probabilidad (usando multiplicación)
- Contamos todas las combinaciones posibles
- Sumamos todo al final

### **POR QUÉ ES COMPLICADO:**

**Caso "exactamente 3 días":** Hay 4 formas diferentes:

- Día 1: ✓, Día 2: ✓, Día 3: ✓, Día 4: ✗
- Día 1: ✓, Día 2: ✓, Día 3: ✗, Día 4: ✓
- Día 1: ✓, Día 2: ✗, Día 3: ✓, Día 4: ✓
- Día 1: ✗, Día 2: ✓, Día 3: ✓, Día 4: ✓

Cada una tiene la misma probabilidad, pero hay que sumarlas todas.

### **EL RESULTADO:**

Al final obtienes 51.77% (no el 66% que pensaba el Chevalier), igual que en el restaurante sería menos probable de lo que pensarías inicialmente.

>[!important] Cuando quieres "al menos una vez", no puedes simplemente sumar. Tienes que ser muy cuidadoso y contar cada posibilidad por separado.
## **¿Por qué 80% × 80% = 64% (y no 160%)?**

### **Analogía Visual:**

Imagina que tienes **100 personas**.

**Día 1:** 80 de ellas van al restaurante (80%) **Día 2:** De esas 80 personas que fueron el día 1, solo el 80% va también el día 2

**¿Cuántas van ambos días?**

- 80 personas × 80% = 80 × 0.8 = **64 personas**
- Eso es 64% del total

### **Otra forma de pensarlo:**

**Con fracciones es más claro:**

- 80% = 8/10
- 8/10 × 8/10 = 64/100 = 64%

### **Analogía de la Caja:**

**Día 1:** Tienes una caja con 100 canicas, tomas 80 (el 80%) **Día 2:** De esas 80 canicas que tienes, solo conservas el 80%

**Resultado:** 80 × 0.8 = 64 canicas (64% del total original)

### **¿Por qué es menor?**

Porque cuando **multiplicas probabilidades**, estás calculando la probabilidad de que **ambos eventos ocurran juntos**, lo cual es **más difícil** que solo uno de ellos.

**Piénsalo así:**

- Es fácil que el restaurante tenga tu plato **un día** (80%)
- Es **más difícil** que lo tenga **dos días seguidos** (64%)

### **La regla general:**

Cuando multiplicas cualquier número menor que 1 (como 0.8), el resultado siempre será **menor** que el número original.

- 0.8 × 0.8 = 0.64
- 0.5 × 0.5 = 0.25
- 0.9 × 0.9 = 0.81

---
## 7. Uno Menos "Sí Ocurre" = "No Ocurre"

Si el chance de que algo ocurra es del 10%, el chance de que *no ocurra* es de 90%. ¿Por qué es útil esta observación? Porque a veces **es más fácil entender el chance de que algo no ocurra**.
### **La Idea Básica (Super Simple):**

Si hay 30% de probabilidad de que llueva, entonces hay 70% de que **NO** llueva. **Fórmula:** 100% - 30% = 70%

### **¿Por Qué Es Útil Este Truco?**

**Problema Difícil:** "¿Cuál es la probabilidad de que gane la lotería al menos una vez si compro 50 boletos diferentes?" _→ Esto es súper complicado de calcular_

**Pregunta Más Fácil:** "¿Cuál es la probabilidad de que pierda en los 50 boletos?" _→ Esto es mucho más fácil_

### **Ejemplo del Chevalier (Versión Simple):**

**Lo que quería saber (difícil):** _"¿Probabilidad de sacar doble 6 al menos una vez en 24 lanzamientos?"_

**Lo que es más fácil calcular:** _"¿Probabilidad de NO sacar doble 6 en ninguno de los 24 lanzamientos?"_

### **Los Pasos:**

1. **Probabilidad de doble 6 en un lanzamiento:** 1/36
2. **Probabilidad de NO sacar doble 6:** 35/36
3. **Probabilidad de NO sacarlo 24 veces seguidas:** (35/36)²⁴ = 50.86%
4. **Probabilidad de sacarlo al menos una vez:** 100% - 50.86% = **49.14%**

### **Analogía del Videojuego:**

**Imagina un jefe final que tiene 3% de probabilidad de soltar un objeto raro.**

**Pregunta difícil:** "¿Cuál es la probabilidad de conseguir el objeto en 100 peleas?"

**Pregunta fácil:** "¿Cuál es la probabilidad de NO conseguirlo en 100 peleas?"

- Probabilidad de no conseguirlo en una pelea: 97%
- Probabilidad de no conseguirlo en 100 peleas: (97%)¹⁰⁰ = 4.7%
- **Probabilidad de conseguirlo al menos una vez:** 100% - 4.7% = **95.3%**

### **¿Por Qué Perdía el Chevalier?**

Sus probabilidades eran **49.14%** (menos del 50%), así que a largo plazo, inevitablemente perdería dinero.

### **La Lección para Diseñadores de Juegos:**

Cuando quieras calcular "al menos una vez", piensa "al revés": calcula "nunca" y réstalo de 100%.
## 8. La suma de múltiples selecciones aleatorias NO es una selección aleatoria lineal!

## Selección aleatoria lineal

Un evento aleatorio donde todos los resultados tienen **el mismo chance de suceder**. Un ejemplo es el dado. En cambio, si tiras múltiples dados los resultados NO tendrán el mismo chance de pasar.

Por ejemplo, al tirar 2 dados, ¿cuál es el chance de tener 7 y 12? De 7 es probable, de 12 no tanto:

![[Pasted image 20250916115151.png]]
![[Pasted image 20250916115229.png]]

A esta gráfica se le llama **curva de distribución de probabilidad** #matemáticas

>[!tip] Los diseñadores de juego deben saber qué tipo de distribución de probabilidad queremos y cómo tenerla. Por ejemplo, cuando sumo dados, creo una "campana de probabilidad": Los valores medios son comunes, los valores extremos raros. Esto hace el juego más **predecible y balanceado**.
## 9. Tira el dado

Toda la probabilidad que hemos hablado se conoce como **probabilidad teórica** #matemáticas. En contraparte está la 
### **probabilidad práctica**

La medida de lo que *ha pasado*.

Esto quiere decir que, al tirar un dado, *matemáticamente* es probable que saldrá un 6 en un 16.67%. En cambio, si *prácticamente* tiro el dado, digamos 100 veces, y casualmente sale 20 veces el 6, la *probabilidad práctica* fue de 20%. Claro, entre más tiradas haga, más me acercaré a la probabilidad teórica. Esto se conoce como el [[Método Monte Carlo]], por el famoso casino.
## 10. A los Geeks les encanta farolear (Ley de Gombaud)

Es válido e incluso esperado preguntarle a personas que saben más sobre probabilidad que yo para solucionar mis problemas.
# Valor esperado #importante

Una de las formas más útiles de usar la probabilidad es calcular el **valor esperado**. Muchas veces, cuando se realiza una **acción** en un juego, *la acción tendrá un valor* ya sea positivo o negativo. Esto puede dar puntos, fichas o dinero ganado o perdido. **El valor esperado de una transacción en un juego es el *promedio de todos los valores posibles que podrían resultar***.

![[Pasted image 20250916135309.png]]
# Considera los valores cuidadosamente

Es importante saber el valor esperado para que las acciones se usen debidamente sin penalización.
### **La Analogía de la Máquina Expendedora Rota**

Imagina tres máquinas expendedoras de refrescos, todas cuestan $1:

**Máquina A (Viento):** Siempre funciona, siempre da 1 refresco **Máquina B (Bola de Fuego):** 80% funciona (1 refresco), 20% se traga tu dinero **Máquina C (Rayo):** 20% funciona (¡pero da 2 refrescos!), 80% se traga tu dinero

### **Calculando el "Valor Esperado":**

- **Máquina A:** 1 refresco garantizado = **1 refresco promedio**
- **Máquina B:** (0.8 × 1) + (0.2 × 0) = **0.8 refrescos promedio**
- **Máquina C:** (0.2 × 2) + (0.8 × 0) = **0.4 refrescos promedio**

### **¿Por Qué No Siempre Usas la "Mejor"?**

**Situación 1: Tienes sed todo el día**

- La Máquina A es la mejor (más confiable a largo plazo)

**Situación 2: Solo tienes $1 y NECESITAS un refresco ahora**

- La Máquina A sigue siendo mejor (garantizada)
- La Máquina C es terrible (80% de probabilidad de quedarte sin nada)

### **El Ejemplo del Videojuego Explicado Simple:**

![[Pasted image 20250916141054.png]]

**Contra un Jefe con 500 HP:**

- **Rayo:** Hace 8 de daño promedio → Necesitas ~63 turnos
- **Viento:** Hace 4 de daño promedio → Necesitas 125 turnos
- **¡El Rayo es mejor!**

**Contra un Enemigo con 15 HP:**

- **Rayo:** 20% probabilidad de matarlo en 1 turno, 80% de fallar completamente
- **Viento:** Lo mata en 4 turnos, 100% garantizado
- **¡El Viento es mejor!**

### **La Lección para Diseñadores:**

**El valor esperado cambia según el contexto:**

1. **Contra enemigos fuertes:** Los ataques de alto riesgo/alta recompensa son mejores
2. **Contra enemigos débiles:** Los ataques consistentes son mejores
3. **Cuando tienes prisa:** La confiabilidad vale más que el daño promedio

### **Aplicación Práctica:**

Cuando diseñes armas/habilidades, pregúntate:

- ¿En qué situaciones es útil cada una?
- ¿Los jugadores tendrán opciones interesantes?
- ¿O siempre elegirán la misma porque es "objetivamente mejor"?

>[!important] **La clave:** El valor esperado no es solo un número. Depende de la situación del jugador.
# El Elemento Humano

Uno esperaría que el humano siempre escogerá la opción con el valor esperado más alto, pero no siempre es el caso. A veces es por ignorancia—los estimados que hacen los jugadores sobre cuán probables son los eventos suelen estar equivocados. 

>[!important] Esto se conoce como la **probabilidad percibida** y determinará cómo los jugadores jugarán el juego.

Han habido experimentos de probabilidad donde, si uno hiciera el cálculo, aquello que parece de menor valor en realidad es de mayor valor, pero cuando una probabilidad resulta superficialmente "más conveniente" la gente tenderá a escoger esta opción. Esto se debe a que **las personas quieren evitar *el remordimiento* a toda costa.**

![[Pasted image 20250916164516.png]]
Las personas suelen inflar ciertas probabilidades dependiendo de su percepción personal.

>[!important] La distorsión de la realidad de las personas está reflejada por sus *miedos*. Por eso, un diseñador de juegos deberá no sólo entender las probabilidades actuales/matemáticas, sino también las *percibidas* por la [[Audiencia Objetivo]], que pueden variar por múltiples factores.
# [[Lente 35, El Lente del Valor Esperado]]
# La [[Mecánica, Habilidad|habilidad]] y el chance se enrollan

Aquí hay una lista de las 5 interacciones entre la habilidad y la suerte para considerar:

1. **Estimar el chance es una habilidad**
	1.  **Lo que separa a un jugador de un buen jugador es cuando éste es capaz de predecir qué sucederá después a través de calcular las probabilidades.**
	2. La **probabilidad percibida** variará entre jugadores capaces de estimar probabilidades y aquellos que no.
2. **La habilidad tiene una probabilidad de éxito**
	1. Cada acción tiene un nivel de riesgo, y los jugadores están constantemente haciendo decisiones basadas en el valor esperado, decidiendo cuándo jugar con mayores riesgos.
	2. Cuando diseñe mi juego **debo asegurarme que las habilidades estén balanceadas tanto como si balanceara "pura suerte" ya que la probabilidad percibida siempre será distinta para cada jugador**.
3. **Estimar la habilidad de un jugador es una habilidad**
	1. Es muy útil engañar al jugador sobre tu habilidad, haciéndolo subestimar o infraestimar tu verdadera habilidad.
4. **Predecir pura suerte es una habilidad imaginada**
	1. El ser [[Humano]] busca patrones, [[Consciencia|consciente]] e [[Subconsciencia|inconscientemente]], para *predecir* que pasará después.
		1. A veces nuestra mania nos lleva a ver patrones donde, tal vez, no existan.
			1. Como cuando crees que tienes una "racha ganadora" o "racha perdedora", esta última donde *esperas* ganar porque "se te debe".
	2. Como diseñador es importante entender esta cuestión para aprovecharla en mi diseño.
5. **Controlar pura suerte es una habilidad imaginada**
	1. Nuestra mente también suele buscar relaciones *causas-y-efectos*. 
	2. Con la suerte pura no tenemos ningún control, pero *nos gusta* creer que sí, con amuletos, tirar el dado de cierta manera, etc.
		1. Esto es lo que hace que apostar sea estimulante.
	3. **Nuestra tendencia natural a querer controlar nuestro destino vuelve a los juegos divertidos**.

>[!important] La suerte interrelaciona matemáticas, [[Psicología]] humana y todas las [[Mecánicas de juego]] básicas, y por ello los juegos tienen esa riqueza, complejidad y profundidad que nos gusta.
# [[Lente 36, El lente de la Suerte, Probabilidad]]





















