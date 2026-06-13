# Forma matricial de un programa lineal

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)



![Esquema del modelo](../assets/figuras/modelos/modelo_forma_matricial.svg)

## 1. Contexto del problema

Todo programa lineal puede representarse mediante matrices y vectores. Esta lectura permite comprender cómo un solver organiza un modelo y por qué es necesario mantener consistencia entre dimensiones, índices y unidades.

## 2. Intuición del modelo

La forma matricial resume un problema lineal usando vectores y matrices. Es útil para entender cómo los solvers organizan la información y por qué es importante mantener consistencia dimensional.

## 3. Elementos de la formulación

| Elemento | Descripción |
|---|---|
| Conjuntos | $I$: restricciones; $J$: variables. |
| Índices | $i \in I$, $j \in J$. |
| Parámetros | $c_j$: costo; $A_{i,j}$: coeficiente; $b_i$: lado derecho. |
| Variable | $x_j$: decisión. |

## 4. Formulación matemática

### Objetivo

Minimizar costo lineal.

$$
\min Z = \sum_{j \in J} c_j x_j
$$

### Restricciones

Cada fila de la matriz representa una restricción.

$$
\sum_{j \in J} A_{i,j}x_j \geq b_i \quad \forall i \in I
$$

### Dominio

Variables continuas no negativas.

$$
x_j \geq 0 \quad \forall j \in J
$$

## 5. Interpretación técnica

Esta formulación permite reconocer que modelos eléctricos grandes son extensiones estructuradas de matrices de balance, límites y costos.

## 6. Actividad relacionada

- [Ir a la actividad](../actividades/README.md)
---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
