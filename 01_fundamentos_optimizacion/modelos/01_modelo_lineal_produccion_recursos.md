# Modelo lineal de producción con recursos limitados

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)



![Esquema del modelo](../assets/figuras/modelos/modelo_produccion_lineal.svg)

## 1. Contexto del problema

Una organización debe asignar recursos limitados entre varias alternativas productivas. Aunque el ejemplo no representa una red eléctrica completa, reproduce la lógica básica de muchos problemas eléctricos: decidir cuánto producir, cuánto generar o cuánto invertir bajo limitaciones técnicas.

## 2. Enunciado guía

Determine la cantidad óptima de cada alternativa para maximizar beneficio o minimizar costo, respetando disponibilidad de recursos y límites de producción.

## 3. Datos que debe reconocer el estudiante

- alternativas o productos;\n- beneficio o costo unitario;\n- consumo de recursos;\n- disponibilidad total;\n- límites mínimos o máximos.

## 4. Intuición del modelo

Este modelo permite introducir la programación lineal mediante una decisión de asignación de recursos. Cada alternativa consume capacidad y aporta beneficio o costo. El objetivo es encontrar la combinación factible que optimiza el criterio económico.

## 5. Elementos de la formulación

| Elemento | Descripción |
|---|---|
| Conjunto | $P$: productos o alternativas. |
| Índice | $p \in P$. |
| Parámetros | $c_p$: beneficio; $a_p$: consumo de recurso; $R$: recurso disponible; $\overline{x}_p$: producción máxima. |
| Variable | $x_p$: cantidad producida del producto $p$. |

## 6. Formulación matemática

### Función objetivo

Maximizar beneficio total.

$$
\max Z = \sum_{p \in P} c_p x_p
$$

### Recurso disponible

El consumo total no puede superar el recurso disponible.

$$
\sum_{p \in P} a_p x_p \leq R
$$

### Límite de producción

Cada alternativa respeta su capacidad máxima.

$$
0 \leq x_p \leq \overline{x}_p \quad \forall p \in P
$$

## 7. Interpretación técnica

La solución muestra qué alternativas son económicamente atractivas y qué restricción limita el sistema. Si la restricción de recurso está activa, aumentar $R$ podría mejorar el objetivo.

## 8. Actividad relacionada

- [Ir a la actividad](../actividades/actividad_01_fundamentos_optimizacion.md)
---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
