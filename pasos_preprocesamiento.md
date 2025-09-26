# Resumen del proceso de evaluación y preprocesamiento de calidad de datos

## 1. Entendimiento de los Datos

Se inició el proceso revisando únicamente el diccionario de datos, identificando para cada columna su nombre, definición y tipo de dato esperado. Se hizo especial énfasis en identificar columnas ambiguas o con definiciones poco claras y se documentó el significado exacto de cada variable. No se revisó aún la información contenida en los datos, ajustándose a buenas prácticas metodológicas.

## 2. Completitud

Se identificaron y cuantificaron los valores nulos en cada columna del dataset. Se analizó la naturaleza de la ausencia de datos para distinguir entre nulos esperados (naturales) y aquellos que se deben a fallas de recolección o errores. Las decisiones adoptadas priorizaron la imputación o corrección antes que la eliminación de registros, siguiendo el principio de minimizar la pérdida de información relevante.

## 3. Unicidad

Se analizaron posibles registros duplicados, definiendo criterios claros para considerar un registro como duplicado total o parcial basados en variables clave. Se priorizó la eliminación únicamente de duplicados auténticos, sin riesgo de pérdida de información genuina, y se documentaron las reglas empleadas para esta definición.

## 4. Consistencia

Se estructuró la evaluación en tres dominios:

- _Consistencia geométrica:_ Se establecieron reglas físicas (ej. área convexa ≥ área) y se priorizó la recalculación o marcación como nulo, evitando la eliminación inmediata.
- _Consistencia de cálculo:_ Se validaron métricas derivadas a partir de variables base, corrigiendo valores incoherentes por recalculo.
- _Consistencia de rango lógico:_ Se verificó que los valores de proporciones y métricas geométricas respetaran los límites teóricos.
  El rastreo del número de incidencias se pospuso hasta la resolución de nulos, para evitar distorsión en los reportes.

## 5. Validez

Se verificó que cada variable respetara su tipo, formato y rango definido. Se corrigieron inconsistencias de mayúsculas/minúsculas en las variables categóricas y se marcaron como nulos los valores físicamente imposibles o fuera de rango. Se propuso que toda captura futura incluya validaciones automáticas en formularios y pipelines de procesamiento para reducir la incidencia de errores desde su origen.

---

**Conclusión:**
El proceso seguido aseguró un análisis cuidadoso, sistematizado y justificable de la calidad de datos, respetando las mejores prácticas de preprocesamiento y fundamentando cada decisión sobre el tratamiento de los registros problemáticos.
