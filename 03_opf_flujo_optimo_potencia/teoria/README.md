# Teoría — Flujo óptimo de potencia

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

![Del despacho económico al OPF](../assets/figuras/teoria/opf_de_ed_a_red.svg)

El OPF combina optimización económica con restricciones físicas de red. En su forma completa es no lineal y no convexa.

## 1. Modelo DC

$$
F_\ell = \frac{\theta_i-\theta_j}{x_\ell}
$$

## 2. Modelo AC

$$
P_i = V_i\sum_{j\in N} V_j(G_{ij}\cos\theta_{ij}+B_{ij}\sin\theta_{ij})
$$

$$
Q_i = V_i\sum_{j\in N} V_j(G_{ij}\sin\theta_{ij}-B_{ij}\cos\theta_{ij})
$$

## 3. Diferencia pedagógica

| Aspecto | OPF-DC | OPF-AC |
|---|---|---|
| Variables | $P$, $\theta$ | $P$, $Q$, $V$, $\theta$ |
| Pérdidas | no | sí |
| Reactivos | no | sí |
| Complejidad | lineal | no lineal |

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
