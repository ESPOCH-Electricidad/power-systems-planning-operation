> Documento elaborado a partir de modelos AMPL revisados en clase. El repositorio público documenta la formulación y los datos; los archivos `.mod` y `.run` resueltos por el docente se mantienen en material privado.

# Modelo 03 — Localización de antenas y cobertura

## Propósito
Minimizar el costo de instalación de antenas garantizando cobertura mínima de todos los medidores.

## Estructura matemática

- Conjuntos: medidores y antenas candidatas.
- Parámetros: distancia, distancia máxima y costo de instalación.
- Variables binarias: instalación de antena y cobertura medidor-antena.
- Objetivo: minimizar costo de instalación.
- Restricciones: cobertura válida por distancia, cobertura solo si antena instalada y cobertura mínima.

## Interpretación
Es un MILP de cobertura. Su lógica se parece a problemas de inversión binaria en expansión de red y generación.
