# Actividad 01C — Localización binaria de equipos de monitoreo

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Contexto

Una empresa eléctrica debe instalar equipos de monitoreo en puntos candidatos para observar alimentadores críticos. Cada punto candidato tiene un costo de instalación y puede cubrir ciertos alimentadores. El objetivo es cubrir todos los alimentadores al menor costo.

Esta actividad introduce variables binarias y prepara al estudiante para decisiones discretas de unit commitment, TNEP y GEP.

## 2. Datos

| Sitio candidato | Costo instalación [USD] |
|---|---:|
| S1 | 850 |
| S2 | 700 |
| S3 | 920 |
| S4 | 600 |

| Alimentador | S1 | S2 | S3 | S4 |
|---|---:|---:|---:|---:|
| A1 | 1 | 1 | 0 | 0 |
| A2 | 1 | 0 | 1 | 0 |
| A3 | 0 | 1 | 1 | 1 |
| A4 | 0 | 0 | 1 | 1 |
| A5 | 1 | 0 | 0 | 1 |

## 3. Trabajo solicitado

Formule un MILP que decida qué sitios instalar para cubrir todos los alimentadores. Luego realice dos variantes:

1. exigir que A3 tenga cobertura redundante por al menos dos sitios;
2. limitar el presupuesto máximo a 1600 USD y permitir un alimentador no cubierto con penalización.

## 4. Preguntas de análisis

1. ¿Qué sitios se instalan en el caso base?
2. ¿Qué cambia al exigir redundancia?
3. ¿Qué significa introducir penalización por alimentador no cubierto?
4. ¿Por qué este modelo es MILP y no PL?


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
