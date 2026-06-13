# Actividad 01B — Modelo de transporte de energía

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto del problema

Tres centrales deben abastecer cuatro zonas de demanda. El objetivo es minimizar el costo de transporte de energía entre centrales y zonas. Este modelo no representa todavía las leyes físicas de una red eléctrica; es un modelo de asignación oferta-demanda.

Esta actividad replica y extiende el [modelo de transporte de energía](../modelos/03_modelo_transporte_energia.md).

## 2. Datos

| Central | Oferta máxima [MWh] |
|---|---:|
| C1 | 120 |
| C2 | 100 |
| C3 | 90 |

| Zona | Demanda [MWh] |
|---|---:|
| Z1 | 70 |
| Z2 | 80 |
| Z3 | 60 |
| Z4 | 75 |

| Central/Zona | Z1 | Z2 | Z3 | Z4 |
|---|---:|---:|---:|---:|
| C1 | 4 | 6 | 9 | 7 |
| C2 | 5 | 4 | 7 | 6 |
| C3 | 8 | 5 | 4 | 3 |

## 3. Formulación esperada

$$
\min Z = \sum_{i\in I}\sum_{j\in J} c_{i,j} f_{i,j}
$$

$$
\sum_{j\in J} f_{i,j} \leq S_i \quad \forall i\in I
$$

$$
\sum_{i\in I} f_{i,j} \geq D_j \quad \forall j\in J
$$

## 4. Extensiones

Agregar penalización por demanda no servida, aumentar Z4 en 25 %, reducir oferta C2 en 30 % y prohibir el envío C1-Z3.

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
