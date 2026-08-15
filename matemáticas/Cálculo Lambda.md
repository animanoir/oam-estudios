El cálculo Lambda **λ** es, entre otras cosas:
- Una noción de [[computación]] mínima.
- Computación basada estrictamente en [[funciones puras]].
- No tiene estado interno
- El "lenguaje de [[programación]] más pequeño del mundo".

El cálculo Lambda puede representar cualquier [[Máquina de Turing]].

Se compone de 3 elementos:
1. Variable
	1. x (una variable llamada "x")
2. Función
	1. λx.x (una función con el parámetro "x" y el cuerpo "x")
3. Aplicación
	1.  (λx.x)a (llamar una función λx.x con el argumento "a")

La función más básica es la función identidad: λx.x que es equivalente a f(x) = x. La primera "x" es el argumento de la función, y el segundo es el cuerpo de la función.

# Free vs. Bound Variables (libre / ligada)

- En la función λx.x, "x" se llama **variable ligada** porque está dentro del cuerpo como el parámetro de la función.
- En λx.y, "y" se llama **variable libre** porque nunca es declarada antes.
# Evaluación

La evaluación es hecha via la **β-reduction** (beta reducción) que es esencialmente **sustitución con alcance léxico**

**β-reduction** es "meter el argumento donde va la variable", y *alcance léxico* es la regla que garantiza que al meterlo nadie cambie de identidad en el camino.

> **Alcance léxico**: Un nombre significa lo que significaba *en el lugar donde se escribió, no en el lugar a donde llegó*.
> Por ejemplo: En la oficina trabajas con Ana. Escribes una nota: "Que Ana revise el contrato.". Mandas esa nota a otra sucursal. Ahí también hay una Ana, pero *es otra persona*.
> **Con alcance léxico**: la nota sigue refiriéndose a *tu Ana*, la de la oficina donde escribiste. El significado viaja con el texto.
> **Sin alcance léxico**: la nota se refiere a la Ana de donde se lea. El significado cambia según a dónde llegue, y el contrato lo revisa la persona equivocada.
> El cálculo Lambda usa lo primero. Y por eso, cuando al sustituir hay riesgo de confusión, se le cambia el nombre a una de las dos: la Ana local pasa a llamarse "Ana B." antes de meter la nota. Eso es **α-conversión**, y es lo que hace que la sustitución sea ***capture-avoiding***, que evita la captura.

![[Pasted image 20260729130148.png]]