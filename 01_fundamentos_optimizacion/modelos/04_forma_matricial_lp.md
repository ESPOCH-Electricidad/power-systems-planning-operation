> Documento elaborado a partir de modelos AMPL revisados en clase. El repositorio público documenta la formulación y los datos; los archivos `.mod` y `.run` resueltos por el docente se mantienen en material privado.

# Modelo 04 — Forma matricial LP

## Propósito
Representar problemas lineales mediante matriz de restricciones, vector de costos y lado derecho.

## Estructura matemática

- Conjunto de variables `J`.
- Conjunto de restricciones `I`.
- Parámetros: matriz `A`, vector `B`, costos `C`.
- Variables no negativas `X[j]`.
- Objetivo: minimizar la suma de costos.
- Restricciones: sistema lineal parametrizado.

## Interpretación
Permite entender la estructura algebraica general que luego se repite en modelos ED, OPF, TNEP y GEP.
