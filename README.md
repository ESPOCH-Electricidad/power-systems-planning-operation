# Planificación y Operación de Sistemas Eléctricos de Potencia

![Banner del repositorio](docs/assets/img/banner_operacion_planificacion_sep.svg)

Repositorio académico de apoyo a la asignatura **Planificación y Operación de Sistemas Eléctricos de Potencia**. Organiza formulaciones matemáticas, datos de prueba, casos de estudio, notebooks de exploración y actividades de evaluación para estudiar problemas de operación y planificación de sistemas eléctricos.

El material está estructurado para que el estudiante pueda transitar desde la formulación matemática hasta la interpretación técnica de resultados computacionales.

## Propósito

- Presentar modelos de optimización aplicados a sistemas eléctricos de potencia.
- Organizar casos de prueba reutilizables para operación, OPF, TNEP y GEP.
- Facilitar el análisis de datos mediante notebooks y archivos tabulares.
- Apoyar actividades de clase, laboratorios, evaluación formativa y discusión técnica.
- Promover una lectura crítica de las soluciones obtenidas mediante herramientas computacionales.

## Estructura temática

![Clasificación de operación y planificación](docs/assets/img/clasificacion_operacion_planificacion.svg)

| Bloque | Carpeta | Contenido principal | Finalidad didáctica |
|---|---|---|---|
| 1 | [`01_fundamentos_optimizacion`](01_fundamentos_optimizacion/) | LP, MILP, NLP básicos | Comprender la formulación matemática antes de estudiar aplicaciones eléctricas |
| 2 | [`02_operacion_corto_plazo`](02_operacion_corto_plazo/) | ED, ED con pérdidas, UC, despacho hidrotérmico | Modelar decisiones operativas de corto plazo |
| 3 | [`03_opf_flujo_optimo_potencia`](03_opf_flujo_optimo_potencia/) | OPF-DC, OPF-AC | Relacionar optimización con restricciones de red |
| 4 | [`04_tnep_expansion_transmision`](04_tnep_expansion_transmision/) | Transporte, DC, híbrido, lineal disyuntivo | Decidir expansión de red y comparar formulaciones |
| 5 | [`05_gep_expansion_generacion`](05_gep_expansion_generacion/) | Base, estático con bloques, multianual | Decidir expansión de generación por tecnología y periodo |
| 6 | [`06_casos_de_estudio`](06_casos_de_estudio/) | Garver, IEEE 14, IEEE 24 RTS, sistemas didácticos | Reutilizar datos comunes en distintos modelos |


## Horizontes temporales

![Horizontes temporales](docs/assets/img/horizontes_temporales_sep.svg)

La asignatura estudia decisiones que ocurren en distintos horizontes temporales: desde la operación de minutos u horas hasta la planificación de expansión de varios años. Esta separación ayuda a identificar qué variables son operativas, qué variables son de inversión y qué restricciones deben considerarse en cada escala.

## Flujo de trabajo sugerido

1. Revisar la formulación matemática del bloque correspondiente.
2. Identificar conjuntos, parámetros, variables, función objetivo y restricciones.
3. Explorar el caso de estudio mediante archivos de datos y notebooks.
4. Ejecutar el modelo computacional indicado por el docente.
5. Comparar resultados, validar supuestos y responder las actividades.
6. Elaborar conclusiones técnicas sobre costo, operación, factibilidad, confiabilidad y expansión.

## Sitio web del repositorio

La carpeta [`docs`](docs/) contiene una versión navegable de la guía del repositorio para publicarla mediante GitHub Pages.
