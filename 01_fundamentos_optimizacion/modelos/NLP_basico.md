# Programación no lineal (NLP)

## Idea del modelo

Un problema NLP incluye función objetivo o restricciones no lineales. En sistemas eléctricos aparece en OPF-AC, funciones de pérdidas, costos cuadráticos, ecuaciones de flujo de potencia y restricciones de tensión.

## Conjuntos e índices

- $n \in \mathcal{N}$: barras del sistema.
- $g \in \mathcal{G}$: generadores.
- $(i,j) \in \mathcal{L}$: líneas o ramas.

## Parámetros

- $D_n$: demanda en la barra $n$.
- $G_{ij}, B_{ij}$: conductancia y susceptancia de la red.
- $P_g^{\min}, P_g^{\max}$: límites de generación.
- $V_n^{\min}, V_n^{\max}$: límites de tensión.

## Variables de decisión

- $P_g, Q_g$: potencia activa y reactiva del generador $g$.
- $V_n$: magnitud de tensión en la barra $n$.
- $\theta_n$: ángulo de tensión en la barra $n$.

## Función objetivo

Un caso típico minimiza costos de generación:

$$
\min \sum_{g\in\mathcal{G}} \left(a_gP_g^2+b_gP_g+c_g\right)
$$

## Restricciones principales

Balance de potencia activa:

$$
P_n^G - D_n^P = V_n\sum_{m\in\mathcal{N}} V_m\left(G_{nm}\cos\theta_{nm}+B_{nm}\sin\theta_{nm}\right)
$$

Balance de potencia reactiva:

$$
Q_n^G - D_n^Q = V_n\sum_{m\in\mathcal{N}} V_m\left(G_{nm}\sin\theta_{nm}-B_{nm}\cos\theta_{nm}\right)
$$

Límites técnicos:

$$
P_g^{\min}\leq P_g\leq P_g^{\max}, \qquad
V_n^{\min}\leq V_n\leq V_n^{\max}
$$

## Interpretación

La solución depende de la no linealidad y puede ser sensible al punto inicial, a los límites y al solver utilizado. Es más representativa físicamente que una aproximación lineal, pero también más exigente computacionalmente.

## Errores frecuentes

- Comparar directamente resultados AC y DC sin considerar supuestos.
- Ignorar límites de tensión o potencia reactiva.
- Asumir que toda solución local es globalmente óptima.
