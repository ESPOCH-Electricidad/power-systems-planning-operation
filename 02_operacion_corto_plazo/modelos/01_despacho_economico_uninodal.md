# Despacho económico uninodal

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)



![Esquema del modelo](../assets/figuras/modelos/despacho_economico.svg)

## 1. Contexto del problema

El operador del sistema debe cubrir la demanda horaria usando generadores con costos y límites. La red se ignora, por lo que el sistema se trata como un solo nodo.

## 2. Enunciado guía

Determine la generación óptima de cada unidad para minimizar el costo operativo.

## 3. Datos que debe reconocer el estudiante

- demanda por hora;\n- costos variables;\n- límites de generación;\n- penalización por energía no servida.

## 4. Intuición del modelo

El despacho económico asigna generación para cubrir demanda al menor costo sin representar la red. Es el modelo operativo más básico.

## 5. Elementos de la formulación

| Elemento | Descripción |
|---|---|
| Conjuntos | $G$: generadores; $T$: periodos. |
| Parámetros | $c_g$, $\underline{P}_g$, $\overline{P}_g$, $D_t$, $VOLL$. |
| Variables | $P_{g,t}$, $ENS_t$. |

## 6. Formulación matemática

### Objetivo

Minimizar costo operativo y ENS.

$$
\min Z=\sum_{t\in T}\sum_{g\in G} c_g P_{g,t}+\sum_{t\in T}VOLL\,ENS_t
$$

### Balance

Generación y ENS cubren demanda.

$$
\sum_{g\in G}P_{g,t}+ENS_t=D_t \quad \forall t
$$

### Límites

Cada unidad respeta límites técnicos.

$$
\underline{P}_g \leq P_{g,t}\leq \overline{P}_g \quad \forall g,t
$$

## 7. Interpretación técnica

El resultado permite identificar la unidad marginal, el costo horario y la necesidad de ENS si no hay capacidad suficiente.

## 8. Actividad relacionada

- [Ir a la actividad](../actividades/actividad_02_operacion_corto_plazo.md)
---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
