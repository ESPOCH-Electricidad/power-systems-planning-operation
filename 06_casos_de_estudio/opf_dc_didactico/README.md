# Caso OPF-DC didáctico

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Tema asociado

**Tema principal:** OPF-DC

## 2. Contexto del caso

Caso pequeño diseñado para que el estudiante entienda incidencia, ángulos, flujos y límites de transmisión sin perderse en una red grande.

## 3. ¿Cuándo usar este caso?

| Bloque | Uso recomendado |
|---|---|
| 03 OPF | primer modelo OPF-DC |
| 01 Fundamentos | relación con balances lineales |

## 4. Datos disponibles

| Archivo | Descripción |
|---|---|
| `opf_dc_base.dat` | Datos disponibles para el caso |

## 5. Flujo de trabajo sugerido

1. Revisar qué modelo se desea aplicar.
2. Identificar datos disponibles y unidades.
3. Adaptar los datos al `.dat` del modelo correspondiente.
4. Ejecutar el modelo y verificar factibilidad.
5. Graficar resultados: generación, flujos, inversión, ENS o tensiones según corresponda.
6. Comparar el caso base con al menos un escenario de sensibilidad.

## 6. Resultados que debe producir el estudiante

| Tipo de análisis | Resultado mínimo |
|---|---|
| Operación | generación, costo, ENS, unidad marginal |
| OPF | flujos, límites activos, tensiones o ángulos |
| TNEP | corredores construidos, costo de inversión, ENS |
| GEP | capacidad nueva, capacidad acumulada, generación por bloque |

---

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)
