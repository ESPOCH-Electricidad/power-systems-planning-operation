# Actividad 01B — Transporte de energía entre fuentes y cargas

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto

Un sistema simplificado tiene tres fuentes de energía y tres centros de carga. Se desea asignar el suministro desde cada fuente hacia cada carga minimizando el costo de transporte. Este ejercicio permite comprender oferta, demanda, flujos y costos antes de estudiar OPF o TNEP.

## 2. Datos

| Fuente | Capacidad disponible [MW] |
|---|---:|
| F1 | 100 |
| F2 | 80 |
| F3 | 120 |

| Carga | Demanda [MW] |
|---|---:|
| C1 | 70 |
| C2 | 110 |
| C3 | 90 |

| Costo [USD/MWh] | C1 | C2 | C3 |
|---|---:|---:|---:|
| F1 | 5 | 7 | 9 |
| F2 | 6 | 4 | 8 |
| F3 | 9 | 6 | 3 |

## 3. Trabajo solicitado

Formule un modelo de transporte que minimice el costo total. Luego resuelva tres variantes:

1. aumentar demanda de C2 en 20 MW;
2. reducir capacidad de F3 a 90 MW;
3. prohibir el envío F1 → C3.

## 4. Preguntas de análisis

1. ¿Qué rutas de transporte se usan en el caso base?
2. ¿Qué fuente queda más comprometida?
3. ¿Qué ocurre cuando se prohíbe una ruta?
4. ¿Qué diferencia conceptual existe entre este modelo y un OPF?


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
