# Programación lineal entera mixta (MILP)

## Idea del modelo

Un problema MILP combina variables continuas con variables enteras o binarias. En sistemas eléctricos permite representar encendido/apagado de unidades, construcción de líneas, selección de tecnologías y decisiones discretas de inversión.

## Conjuntos e índices

- $i \in \mathcal{I}$: actividades continuas.
- $j \in \mathcal{J}$: decisiones discretas o candidatas.
- $r \in \mathcal{R}$: restricciones del problema.

## Parámetros

- $c_i$: costo de una variable continua.
- $f_j$: costo fijo asociado a activar la decisión $j$.
- $a_{r,i}$, $b_{r,j}$: coeficientes técnicos de las restricciones.
- $M_j$: constante suficientemente grande para vincular decisiones continuas y binarias.

## Variables de decisión

- $x_i \geq 0$: variable continua.
- $y_j \in \{0,1\}$: variable binaria de activación.

## Función objetivo

$$
\min \sum_{i\in\mathcal{I}} c_i x_i + \sum_{j\in\mathcal{J}} f_j y_j
$$

## Restricciones principales

$$
\sum_{i\in\mathcal{I}} a_{r,i}x_i + \sum_{j\in\mathcal{J}} b_{r,j}y_j \leq d_r
\qquad \forall r\in\mathcal{R}
$$

Vinculación entre variable continua y decisión binaria:

$$
0 \leq x_j \leq M_j y_j \qquad \forall j\in\mathcal{J}
$$

## Interpretación

La solución indica tanto cantidades continuas como decisiones discretas. Es común en UC, TNEP y GEP cuando la inversión o el estado operativo no puede fraccionarse libremente.

## Errores frecuentes

- Seleccionar valores de $M$ demasiado grandes.
- Relajar variables binarias sin justificarlo.
- No distinguir entre costo fijo y costo variable.
