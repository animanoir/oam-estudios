Es cuanto el código se organiza en base a **dominio de problemas**, no en cuanto a nombres técnicos ([[Controllers]], [[Services]], etc.). Es decir, **la arquitectura debe emerger del lenguaje del negocio, no de un framework**.

# Capas

## [[Lenguaje]] ubicuo

Como diría [[Ludwig Wittgenstein]]:

> Los límites del lenguaje del dominio son los límites del modelo.

Esto elimina fricción por mantener dos vocabularios que mantener.

## Bounded context

Por ejemplo, la palabra "miembro" significa algo diferente dependiendo del contexto. Por ejemplo en Discord: un Miembro puede tener baneos, notas, sobrenombres, etc., pero en el mismo sistema en el contexto de eventos en vivo, un Miembro tiene RSPVs, micrófonos activos, etc.

Lo que normalmente se hace es hacer que `Miembro` soporte todo, pero en contextos diferentes tendrá muchos `null`.

Lo que dice el DDD es que **cada contexto tiene su propio modelo**, con su propio `Miembro` y reglas internas. Los contextos se comunican por sus fronteras ([[APIs]] internas, eventos).

## Separación entre dominio e infraestructura


