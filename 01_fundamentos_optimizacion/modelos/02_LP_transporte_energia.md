> Documento elaborado a partir de modelos AMPL revisados en clase. El repositorio público documenta la formulación y los datos; los archivos `.mod` y `.run` resueltos por el docente se mantienen en material privado.

# Modelo 02 — Transporte de energía con reserva

## Propósito
Minimizar el costo de transportar energía desde centrales hacia ciudades, cumpliendo demanda y respetando capacidad disponible.

## Estructura matemática

- Conjuntos: centrales y ciudades.
- Parámetros: capacidad, demanda, costo de transporte y factor de reserva.
- Variable: energía enviada desde cada central a cada ciudad.
- Objetivo: minimizar costo total.
- Restricciones: capacidad con reserva y demanda de cada ciudad.

## Interpretación
Es un puente hacia modelos eléctricos más complejos porque introduce balance, límite de capacidad y reserva.
