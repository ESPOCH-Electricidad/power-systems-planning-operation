# Programación lineal (LP)

## Idea del modelo

Un problema de programación lineal minimiza o maximiza una función objetivo lineal sujeta a restricciones lineales. En sistemas eléctricos se usa en modelos simplificados de despacho, flujo DC, balance de energía y planificación con aproximaciones lineales.

## Conjuntos e índices

- $i \in \mathcal{I}$: actividades, generadores, recursos o alternativas.
- $r \in \mathcal{R}$: restricciones o recursos disponibles.

## Parámetros

- $c_i$: costo o beneficio unitario de la actividad $i$.
- $a_{r,i}$: consumo o aporte de la actividad $i$ en la restricción $r$.
- $b_r$: disponibilidad, límite o requerimiento asociado a $r$.
- $\ell_i, u_i$: límites inferior y superior de la variable $i$.

## Variables de decisión

- $x_i \geq 0$: nivel de actividad, producción, flujo o capacidad asignada.

## Función objetivo

$$
\min \sum_{i\in\mathcal{I}} c_i x_i
$$

## Restricciones principales

$$
\sum_{i\in\mathcal{I}} a_{r,i}x_i \leq b_r \qquad \forall r\in\mathcal{R}
$$

$$
\ell_i \leq x_i \leq u_i \qquad \forall i\in\mathcal{I}
$$

## Interpretación

La solución entrega valores continuos de las variables. Es adecuada cuando las decisiones pueden representarse como cantidades divisibles, como potencia, energía o flujo agregado.

## Errores frecuentes

- Usar variables continuas para decisiones que en realidad son discretas.
- Ignorar unidades de parámetros y variables.
- Interpretar una aproximación lineal como representación completa del sistema físico.
