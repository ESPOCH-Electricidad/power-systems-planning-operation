# Actividad 01A — Producción lineal de componentes eléctricos

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto

Una empresa fabrica tres tipos de componentes eléctricos para redes de distribución: aisladores, conectores y soportes metálicos. Cada componente consume horas de máquina y material. El objetivo es decidir cuántas unidades producir para maximizar el margen total sin exceder los recursos disponibles.

Esta actividad extiende el modelo de producción con recursos limitados, pero incorpora dos recursos y una demanda mínima para un componente prioritario.

## 2. Datos

| Producto | Margen [USD/u] | Horas máquina [h/u] | Material [kg/u] | Producción máxima [u] |
|---|---:|---:|---:|---:|
| Aislador | 12 | 0.40 | 1.2 | 180 |
| Conector | 9 | 0.25 | 0.8 | 220 |
| Soporte | 15 | 0.55 | 1.5 | 140 |

| Recurso | Disponibilidad |
|---|---:|
| Horas máquina | 120 h |
| Material | 280 kg |

Además, por requerimiento de contrato, deben producirse al menos **60 aisladores**.

## 3. Trabajo solicitado

Formule un modelo PL que maximice el margen total. Luego realice tres extensiones:

1. aumentar 15 % la disponibilidad de horas máquina;
2. reducir 20 % la disponibilidad de material;
3. imponer producción mínima de 80 conectores.

## 4. Preguntas de análisis

1. ¿Qué recurso limita la producción?
2. ¿Qué producto domina la solución?
3. ¿Cómo cambia el resultado cuando aumenta la disponibilidad de máquina?
4. ¿La demanda mínima modifica la solución óptima?


## Entregables

- `.dat`: datos construidos desde las tablas.
- `.mod`: formulación desarrollada por el estudiante.
- `.run`: archivo de ejecución.
- `.out`: salida del solver.
- `.xlsx`: resultados y gráficos.
- `.pdf`: informe técnico breve.

## Criterios de evaluación

| Criterio | Peso |
|---|---:|
| Interpretación del enunciado y datos | 20 % |
| Formulación matemática | 30 % |
| Implementación computacional | 20 % |
| Resultados y gráficos | 15 % |
| Análisis de sensibilidad | 15 % |


---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
