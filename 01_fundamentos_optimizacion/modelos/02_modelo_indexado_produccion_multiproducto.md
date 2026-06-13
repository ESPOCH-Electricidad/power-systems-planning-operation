# Modelo indexado de producción multiproducto

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)



![Esquema del modelo](../assets/figuras/modelos/modelo_produccion_lineal.svg)

## 1. Contexto del problema

El problema anterior puede crecer rápidamente. En lugar de escribir una ecuación por cada producto, se usa notación indexada. Esta es la forma natural de construir modelos de sistemas eléctricos con decenas de generadores, barras o líneas.

## 2. Enunciado guía

Reformule el problema usando conjuntos e índices para que el número de productos pueda cambiar sin modificar la estructura matemática.

## 3. Datos que debe reconocer el estudiante

- conjunto de alternativas;\n- matriz de consumo por recurso;\n- disponibilidad de cada recurso;\n- requerimiento o demanda mínima.

## 4. Intuición del modelo

La formulación indexada permite pasar de un ejemplo pequeño a un modelo escalable. En sistemas eléctricos, esta idea se usa para agregar generadores, líneas, tecnologías, periodos o escenarios sin reescribir todas las ecuaciones.

## 5. Elementos de la formulación

| Elemento | Descripción |
|---|---|
| Conjuntos | $P$: productos; $R$: recursos. |
| Índices | $p \in P$, $r \in R$. |
| Parámetros | $c_p$, $a_{r,p}$, $B_r$, $D$, $\overline{x}_p$. |
| Variable | $x_p$: producción del producto $p$. |

## 6. Formulación matemática

### Objetivo

Minimizar costo total de producción.

$$
\min Z = \sum_{p \in P} c_p x_p
$$

### Demanda mínima

La producción agregada cubre un requerimiento.

$$
\sum_{p \in P} x_p \geq D
$$

### Recursos múltiples

Cada recurso limita la producción total.

$$
\sum_{p \in P} a_{r,p}x_p \leq B_r \quad \forall r \in R
$$

### Dominio

Producción no negativa y acotada.

$$
0 \leq x_p \leq \overline{x}_p \quad \forall p \in P
$$

## 7. Interpretación técnica

La ventaja principal es la escalabilidad. El estudiante debe reconocer que el mismo modelo funciona con dos productos o con cientos de alternativas.

## 8. Actividad relacionada

- [Ir a la actividad](../actividades/actividad_01_fundamentos_optimizacion.md)
---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
