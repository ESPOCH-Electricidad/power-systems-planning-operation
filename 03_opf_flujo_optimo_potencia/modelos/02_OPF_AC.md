> Documento elaborado a partir de modelos AMPL revisados en clase. El repositorio público documenta la formulación y los datos; los archivos `.mod` y `.run` resueltos por el docente se mantienen en material privado.

# Modelo 02 — OPF-AC

## Propósito
Resolver flujo óptimo con ecuaciones no lineales de potencia activa/reactiva, magnitudes de tensión y límites eléctricos.

## Elementos
- Variables: magnitud de tensión, ángulo, generación activa/reactiva y flujos por rama.
- Restricciones: balance activo/reactivo, ecuaciones AC, límites de tensión y límites de ramas.

## Interpretación
Es más completo que OPF-DC y permite estudiar tensión, reactivos y pérdidas. También es más exigente computacionalmente.
