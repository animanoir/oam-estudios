Haskell es un lenguaje de [[programación funcional]] de [[funciones puras]]. Es decir, declaras lo que *algo es*, en lugar de escribirle a la computadora una secuencia de instrucciones, como sucede en la [[programación imperativa]].

> En Haskell, el espacio aplica funciones, es decir, no es necesario escribir una función con paréntesis.
# Características

- [[Lazy]]: Sólo ejecuta funciones cuando se le pide un resultado.
- [[Tipado estático]]: Cuando le especificas el [[Tipo de dato]] que es una variable. Los compiladores de Haskell son buenos infiriendo.

Al momento de emplear operaciones aritméticas (+, -, etc.) éstas son ya funciones de tipo **infix**.

A diferencia de los lenguajes de programación [[Paradigma imperativo de programación|imperativos]], donde la función se escribe con los parámetros a modular dentro de paréntesis, en Haskell se escribe el nombre de la función y después el parámetro con un espacio:

```haskell
succ 8
9
```

Podemos convertir una función en tipo infix usando backticks, para evitar confusiones dado que en Haskell una función se suele escribir como:

`div 92 9` 

Con backticks:

92 `div` 9: 10
# Funciones

- `succ`: regresa el sucesor de un número.