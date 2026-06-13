> Documento elaborado a partir de modelos AMPL revisados en clase. El repositorio público documenta la formulación y los datos; los archivos `.mod` y `.run` resueltos por el docente se mantienen en material privado.

# Modelo 01 — OPF-DC

## Propósito
Minimizar el costo de generación considerando balance nodal activo, flujo por líneas, ángulo de referencia y límites de transmisión.

## Elementos
- Conjuntos: barras, líneas y generadores.
- Parámetros: demanda, costos, límites de generación, reactancia y límites térmicos.
- Variables: generación activa, ángulos y flujos.
- Restricciones: balance nodal, flujo DC, límites de línea y límites de generación.

## Interpretación
Permite identificar congestión y redespacho. No representa pérdidas, tensión ni potencia reactiva.
