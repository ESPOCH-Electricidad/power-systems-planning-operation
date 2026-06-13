# Teoría — Planificación de expansión de generación

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

![Decisiones GEP](../assets/figuras/teoria/gep_decisiones.svg)

El GEP decide capacidad nueva para cubrir demanda futura con criterios de costo, reserva, confiabilidad, emisiones y disponibilidad.

$$
Cap_{k,y} = Cap_{k,y-1} + Build_{k,y}
$$

$$
\sum_{k\in K} Gen_{k,y,b} + \sum_{e\in E} Gen_{e,y,b} + ENS_{y,b} = D_{y,b}
$$

$$
\sum_{k\in K} FC_k Cap_{k,y} + \sum_{e\in E} FC_e Cap^0_e \geq (1+RM)D^{peak}_y
$$

Indicadores clave: capacidad nueva, capacidad acumulada, generación por tecnología, ENS, costo total, emisiones e inversión por año.

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
