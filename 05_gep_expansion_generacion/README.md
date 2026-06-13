# 05 — Expansión de generación

> [Menú principal](../README.md) · [Índice del sitio](../docs/index.md) · [Ruta de aprendizaje](../docs/learning_path.md) · [Modelos](../docs/modelos.md) · [Casos](../docs/casos_de_estudio.md) · [Evaluación](../docs/evaluacion.md)

![Mapa visual del bloque](../docs/assets/img/bloques/05_gep.svg)

## 1. Contexto y propósito

La expansión de generación decide qué tecnologías instalar, en qué cantidad y en qué periodo. El bloque integra crecimiento de demanda, costos de inversión, costos operativos, reserva, energía no servida y escenarios.

La pregunta central es: **qué capacidad debe instalarse para abastecer demanda futura con costo y riesgo aceptables?**

![Figura conceptual](assets/figuras/conceptos/gep_decisiones.svg)

## 2. Conceptos que se desarrollan

| Concepto | Uso didáctico |
|---|---|
| GEP estático | Decisión de capacidad en un periodo representativo. |
| Bloques de carga | Vincular inversión con operación anual aproximada. |
| Multianual | Acumular capacidad y decisiones en varios años. |
| Escenarios | Analizar demanda, costos, hidrología y emisiones. |

## 3. Ecuación base del bloque

La estructura común de los modelos puede leerse como una optimización de costo o inversión sujeta a balance, límites y reglas operativas:

$$
\min \; C^{op} + C^{inv} + C^{ENS}
$$

sujeto a restricciones de balance, capacidad, disponibilidad, reserva y factibilidad técnica. Cada modelo del bloque especializa esta estructura general.

## 4. Modelos del bloque

| Modelo | Acceso |
|---|---|
| GEP estático de capacidad | [Abrir](modelos/01_modelo_gep_estatico_capacidad.md) |
| GEP con bloques de carga | [Abrir](modelos/02_modelo_gep_bloques_carga.md) |
| GEP multianual | [Abrir](modelos/03_modelo_gep_multianual.md) |

## 5. Actividad principal

- [Abrir actividad del bloque](actividades/actividad_05_gep_multianual.md)

## 6. Preguntas de control

1. ¿Cuál es la decisión principal del modelo?
2. ¿Qué parámetros condicionan más la solución?
3. ¿Qué restricciones podrían volverse activas?
4. ¿Qué resultado debe graficarse para interpretar la solución?
5. ¿Qué limitaciones tiene la formulación?

---

> [Menú principal](../README.md) · [Índice del sitio](../docs/index.md) · [Ruta de aprendizaje](../docs/learning_path.md) · [Modelos](../docs/modelos.md) · [Casos](../docs/casos_de_estudio.md) · [Evaluación](../docs/evaluacion.md)
