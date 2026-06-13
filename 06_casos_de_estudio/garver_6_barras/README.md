# Caso Garver 6 barras

> [Menú principal](../../README.md) · [Índice del sitio](../../docs/index.md) · [Ruta de aprendizaje](../../docs/learning_path.md) · [Modelos](../../docs/modelos.md) · [Casos](../../docs/casos_de_estudio.md) · [Evaluación](../../docs/evaluacion.md)

## 1. Tema asociado

**Tema principal:** TNEP y GEP

## 2. Contexto del caso

El caso Garver es el caso transversal más importante del repositorio. Se usa para estudiar expansión de transmisión y expansión de generación porque permite observar cómo la ubicación de generación, demanda y corredores condiciona la decisión de inversión.

## 3. ¿Cuándo usar este caso?

| Bloque | Uso recomendado |
|---|---|
| 04 TNEP | modelos de transporte, DC, híbrido y disyuntivo |
| 05 GEP | GEP base, bloques de carga y multianual |
| 06 Integrador | comparación entre expansión de red y generación |

## 4. Datos disponibles

| Archivo | Descripción |
|---|---|
| `garver_gep_base.dat` | Datos disponibles para el caso |
| `garver_gep_multiyear.dat` | Datos disponibles para el caso |
| `garver_gep_static_blocks.dat` | Datos disponibles para el caso |
| `garver_tnep_dc.dat` | Datos disponibles para el caso |
| `garver_tnep_transporte.dat` | Datos disponibles para el caso |

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
