# Actividad 01C — Localización binaria de equipos de monitoreo

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto del problema

Una empresa distribuidora desea instalar equipos de monitoreo en puntos candidatos para cubrir alimentadores críticos. Cada equipo tiene un costo de instalación y puede cubrir ciertos alimentadores según distancia o alcance de comunicación.

Esta actividad replica y extiende el [modelo binario de localización y cobertura](../modelos/04_modelo_binario_localizacion_cobertura.md).

## 2. Datos

| Sitio | Costo de instalación [USD] |
|---|---:|
| S1 | 4200 |
| S2 | 3800 |
| S3 | 4500 |
| S4 | 3600 |

| Sitio/Alimentador | F1 | F2 | F3 | F4 | F5 |
|---|---:|---:|---:|---:|---:|
| S1 | 1 | 1 | 0 | 0 | 0 |
| S2 | 0 | 1 | 1 | 1 | 0 |
| S3 | 0 | 0 | 1 | 1 | 1 |
| S4 | 1 | 0 | 0 | 1 | 1 |

## 3. Formulación esperada

$$
\min Z = \sum_{s\in S} C_s y_s
$$

$$
\sum_{s\in S} z_{s,f} \geq 1 \quad \forall f\in F
$$

$$
z_{s,f} \leq y_s \quad \forall s\in S, f\in F
$$

$$
z_{s,f} \leq q_{s,f} \quad \forall s\in S, f\in F
$$

$$
y_s,z_{s,f}\in\{0,1\}
$$

## 4. Extensiones

Exigir doble cobertura en F4, limitar presupuesto a 8000 USD, aumentar costo S4 en 30 % y agregar un sitio S5 propuesto por el estudiante.

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
