# Actividad 01A — Producción lineal con recursos limitados

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto del problema

Una empresa local fabrica tres tipos de aisladores eléctricos de baja tensión. Cada tipo consume tiempo de máquina, material cerámico y horas de inspección. La empresa desea planificar la producción diaria para maximizar la utilidad, respetando recursos disponibles y demanda máxima.

Esta actividad replica y extiende el [modelo lineal de producción con recursos limitados](../modelos/01_modelo_lineal_produccion_recursos.md).

## 2. Datos

| Producto | Utilidad [USD/unid] | Tiempo [h/unid] | Material [kg/unid] | Inspección [h/unid] | Demanda máxima |
|---|---:|---:|---:|---:|---:|
| Aislador_A | 9 | 0.40 | 1.20 | 0.10 | 80 |
| Aislador_B | 13 | 0.65 | 1.80 | 0.12 | 60 |
| Aislador_C | 16 | 0.90 | 2.40 | 0.18 | 45 |

| Recurso | Disponibilidad diaria |
|---|---:|
| Tiempo máquina | 70 h |
| Material cerámico | 180 kg |
| Inspección | 16 h |

## 3. Formulación esperada

$$
\max Z = \sum_{p\in P} u_p x_p
$$

$$
\sum_{p\in P} a_{r,p}x_p \leq B_r \quad \forall r\in R
$$

$$
0 \leq x_p \leq \overline{D}_p \quad \forall p\in P
$$

## 4. Sensibilidad obligatoria

Caso base, reducción del 20 % en material, incremento del 15 % en utilidad del producto B y eliminación de demanda máxima del producto C.

## 5. Preguntas

¿Qué recurso limita la producción? ¿Qué producto domina la solución? ¿Qué significa una restricción activa?

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
