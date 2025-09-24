# Laboratorio 2 - Tarea de agrupación

[Objetivos](#objetivos)

[Herramientas](#herramientas)

[Enunciado](#enunciado)

[Entregables](#entregables)

[Rúbrica de clasificación](#rubrica)

[Sugerencias y aclaraciones](#sugerencias)

## <a name="objetivos"></a> Objetivos

- Aplicar el proceso de aprendizaje para resolver una tarea de agrupación, desde la preparación de los datos hasta la interpretación de los resultados. 
- Aplicar tres algoritmos de clústering (k-means y dos de libre elección) para resolver el objetivo de la organización. 
- Determinar los hiperparámetros para la construcción de los modelos dependiendo de los algoritmos utilizados.
- Construir una tabla comparativa que muestre el rendimiento de los tres modelos de agrupación. 
- Derivar conclusiones a partir de los mejores grupos identificados, que sean útiles para la organización.
- Comunicar los hallazgos encontrados a la organización, explicando por qué tienen valor para el negocio.


## <a name="herramientas"></a> Herramientas

Durante este laboratorio trabajaremos con las siguientes herramientas:

 - Python
	 - Distribución sugerida: [Anaconda](https://www.continuum.io/downloads) 
		 - La versión de Anaconda es 4.4
		 - La versión usada es la de python 2.7, usar python 3 no debería requerir muchos cambios.
	 - Ambiente de desarrollo
	   	 - JupyterLab
	   	 - Google Colab
	 - Librerías
	 	 - Pandas
		 - Scikit-learn
		 - Matplot
		 - Seaborn 

## <a name="enunciado"></a> Enunciado

### Descripción del problema

SenecaféAlpes es una compañía dedicada a la producción, procesamiento y comercialización de café de alta calidad. Uno de sus principales retos consiste en garantizar la uniformidad y trazabilidad de sus granos, ya que la heterogeneidad en tamaño, forma y estructura puede afectar tanto los procesos de tostión como la percepción de calidad del consumidor final. Para enfrentar este desafío, la empresa implementó un sistema de visión por computadora que capturó imágenes de granos correspondientes a siete variedades registradas de café. Tras un proceso de segmentación y extracción de características, se construyó un conjunto de datos con 16 atributos para cada grano. 

A partir de este insumo, SenecaféAlpes ha decidido emprender un proyecto de analítica de datos cuyo objetivo es la aplicación de técnicas de agrupación para identificar patrones morfológicos que permitan caracterizar las distintas variedades de café. La expectativa de la empresa es que los resultados de este estudio generen beneficios en tres dimensiones principales: (i) control de calidad, mediante la caracterización morfológica de los granos para estandarizar procesos de selección y clasificación; (ii) optimización del mercado, a partir de la comprensión de las agrupaciones naturales de las variedades y su aprovechamiento en el diseño de nuevas mezclas con valor agregado; (iii) innovación en trazabilidad, estableciendo las bases para sistemas automáticos de identificación que reduzcan la dependencia de evaluaciones manuales.
Para llevar a cabo este proyecto, la empresa nos ha contratado como científicos de datos, proporcionándonos no solo el conjunto de datos generado, sino también la documentación correspondiente a la descripción detallada de cada atributo (diccionario).

* [Datos de entrenamiento](Datos_SenecaféAlpes.csv)
* [Diccionario de datos](Diccionario_SenecaféAlpes.xlsx)


### Instrucciones 

SenecaféAlpes desea que usted los apoye en la construcción del modelo de agrupación previamente descrito con base en las etapas de la metodología "CRISP-ML":

1. **Preparación de datos:** Realizar la preparación de los datos teniendo en cnuenta las características de los algoritmos de agrupación a emplear. 

3. **Modelamiento:** Aplicar el algoritmo K-Means y otros dos algorimos para construir tres modelos de agrupación. Tengan en cuenta que, en ambientes profesionales, la elección y justificación del algoritmo y sus hiperparámetros hace parte de su tarea de consultoría.

4. **Validación cuantitativa:** La calidad desde el punto de vista cuantitativo puede validarse utilizando diferentes métricas intrínsecas, como el coeficiente de silueta.
    
5. **Validación cualitativa:** Una vez realizada la validación cuantitativa, se debe hacer una descripción de los grupos obtenidos y relacionarlo con el objetivo que tiene la organización para determinar si es posible utilizar el resultado obtenido, o hay que seguir trabajando en alguna dirección específica para la comprensión por parte de la organización.

## <a name="entregables"></a> Entregables
- Informe, que puede ser el mismo cuaderno, el cual debe incluir:
    - Descripción detallada de cada etapa según las instrucciones dadas previamente
    - Indicar el nombre del estudiante que desarrolló cada algoritmo y el uso que le dieron a la IA generativa en el desarrollo del laboratorio.
- Presentación con los resultados.
- Cuaderno ejecutado.

    
Algunas preguntas que pueden guiar su desarrollo son: 

1. ¿Qué criterios son importantes para la selección del modelo? 

2. ¿Cómo medir la calidad del modelo construido? ¿Cómo saber que el modelo construido tiene una buena calidad?  

3. ¿Qué retos tienen estos modelos no supervisados, si se quisieran aplicar a nivel profesional?

4. ¿Cómo varía la calidad de la solución obtenida si se aplican diferentes algoritmos?


**Nota:** 
Recuerde que la presentación debe estar orientada a la organización, por lo que se recomienda evitar el uso de términos muy técnicos y utilizar un lenguaje que sea familiar en el contexto de aplicación. Se les sugiere centrarse en la interpretación de los resultados.


## Instrucciones de Entrega
- El laboratorio se entrega en grupos de mínimo 2 y máximo 3 estudiantes. Estos estudiantes pueden ser de diferentes secciones.
- Recuerde hacer la entrega por la sección unificada en Bloque Neón, antes del sábado 27 de septiembre a las 20:00.   
  Ese será el único medio por el cual se reciben entregas.

## <a name="rubrica"></a> Rúbrica de Calificación

A continuación se encuentra la rúbrica de calificación.

**Nota:** Los siguientes porcentajes hacen referencia a la nota grupal, que corresponde a un 80% de la nota inidiviudal.  
El 20% restante se calcula según el puntaje obtenido en la implementación del algoritmo del cual el estudiante estuvo a cargo dentro del grupo.

| Concepto | Porcentaje |
|:---:|:---:|
| **Estudiante 1 (la parte genérica y la preparación de cada algoritmo se asocia al estudiante que lo implementa):** Descripción del proceso de preparación de datos realizado, el genérico y el relacionado con el algoritmo utilizado. Justitificar utilizando el entendimiento de los datos | 15% |
| **Estudiante 1:** Implementación de K-means, descripción de las decisiones más importantes asociadas a la implementación del algoritmo y los hiperparámetros configurados | 15% |
| **Estudiante 2:** Implementación de un segundo algoritmo de libre elección, descripción corta del algoritmo y de las decisiones más importantes asociadas a la implementación y los hiperparámetros configurados | 15% |
| **Estudiante 3:** Implementación de un tercer algoritmo de libre elección, descripción corta del algoritmo y de las decisiones más importantes asociadas a la implementación y los hiperparametros configurados | 15% |
| Análisis de los resultados obtenidos y justificación del modelo recomendado para el caso propuesto | 25% |
| Presentación para la organización con resultados, con las recomendaciones y donde se incluye el uso que hiciero de IA generativa| 10% |
| Cuaderno asociado, ejecutado | 5% |

## <a name="sugerencias"></a> Sugerencias y aclaraciones

 - Nota 1: la interpretación de los grupos se debe hacer en términos de las variables que consideren importantes (incluya las usadas para la construcción de los clusters
 pero también otras variables, que no hayan incluido)
 - Nota 2: Analizar si los valores de cada columna corresponden a valores adecuados para el negocio, en caso de que no lo sean, deben tratar dichos valores y justificar sus decisiones.

Los siguientes enlaces pueden serle de utilidad para la implementación en Python. 

* [Ejemplo de K-Means usando Sklearn](https://jakevdp.github.io/PythonDataScienceHandbook/05.11-k-means.html)

* [Artículo de Towards Data Science: Mastering K-Means Clustering](https://towardsdatascience.com/mastering-k-means-clustering-065bc42637e4/)

* [Artículo de Towards Data Science: Best Practices for Visualizing Your Cluster Results](https://towardsdatascience.com/best-practices-for-visualizing-your-cluster-results-20a3baac7426) 

 - Cada integrante del grupo debe estar encargado de la implementación de un algoritmo distinto. Sin embargo, todos los integrantes del grupo
deben tener la capacidad de explicar lo realizado por los demás compañeros
 - El análisis de resultados y su justificación debe ser realizado en grupo.

