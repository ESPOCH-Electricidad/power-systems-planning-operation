# 03 — Flujo óptimo de potencia

> [Menú principal](../README.md) · [Índice del sitio](../docs/index.md) · [Ruta de aprendizaje](../docs/learning_path.md) · [Modelos](../docs/modelos.md) · [Casos](../docs/casos_de_estudio.md) · [Evaluación](../docs/evaluacion.md)

![Mapa visual del bloque](../docs/assets/img/bloques/03_opf.svg)

## 1. Contexto y propósito

El OPF extiende el despacho económico incorporando la red eléctrica. Aquí la ubicación de la generación y la demanda importa: una unidad barata puede no abastecer una carga si las líneas se congestionan o si las tensiones violan límites.

La pregunta central es: **¿cuál es el despacho óptimo cuando la red impone restricciones físicas?**

![Figura conceptual](assets/figuras/conceptos/opf_de_ed_a_red.svg)

## 2. Conceptos que se desarrollan

| Concepto | Uso didáctico |
|---|---|
| OPF-DC | Modelo lineal de potencia activa, ángulos y congestión. |
| OPF-AC | Modelo no lineal con tensiones, reactivos y pérdidas. |
| Congestión | Límites de líneas que cambian el despacho. |
| Interpretación nodal | Balance por barra y efecto de ubicación. |

## 3. Ecuación base del bloque

La estructura común de los modelos puede leerse como una optimización de costo o inversión sujeta a balance, límites y reglas operativas:

$$
\min \; C^{op} + C^{inv} + C^{ENS}
$$

sujeto a restricciones de balance, capacidad, disponibilidad, reserva y factibilidad técnica. Cada modelo del bloque especializa esta estructura general.

## 4. Modelos del bloque

| Modelo | Acceso |
|---|---|
| Flujo óptimo de potencia DC | [Abrir](modelos/01_flujo_optimo_potencia_dc.md) |
| Flujo óptimo de potencia AC | [Abrir](modelos/02_flujo_optimo_potencia_ac.md) |

## 5. Actividad principal

- [Abrir actividad del bloque](actividades/actividad_03_opf_dc_ac.md)

## 6. Preguntas de control

1. ¿Cuál es la decisión principal del modelo?
2. ¿Qué parámetros condicionan más la solución?
3. ¿Qué restricciones podrían volverse activas?
4. ¿Qué resultado debe graficarse para interpretar la solución?
5. ¿Qué limitaciones tiene la formulación?

---

> [Menú principal](../README.md) · [Índice del sitio](../docs/index.md) · [Ruta de aprendizaje](../docs/learning_path.md) · [Modelos](../docs/modelos.md) · [Casos](../docs/casos_de_estudio.md) · [Evaluación](../docs/evaluacion.md)
