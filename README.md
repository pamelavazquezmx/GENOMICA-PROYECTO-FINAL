# GENOMICA-PROYECTO-FINAL
Proyecto final de análisis genomicos 
# 🧬 Genómica ecológica de *Prochlorococcus*
## Diversidad genómica y diferenciación ecológica de cianobacterias marinas

<p align="center">
  <img src="https://img.shields.io/badge/Área-Ecología%20marina-167D8D?style=for-the-badge" alt="Ecología marina">
  <img src="https://img.shields.io/badge/Enfoque-Genómica%20ecológica-6A5ACD?style=for-the-badge" alt="Genómica ecológica">
  <img src="https://img.shields.io/badge/Datos-Genomas%20públicos-2E8B57?style=for-the-badge" alt="Genomas públicos">
  <img src="https://img.shields.io/badge/Lenguaje-Python%20%7C%20R-3776AB?style=for-the-badge" alt="Python y R">
</p>

## 1. Descripción del proyecto

*Prochlorococcus* es un género de cianobacterias marinas fotosintéticas que constituye uno de los componentes más importantes del fitoplancton de los océanos. Su abundancia, distribución y diversidad genética lo convierten en un modelo de estudio para comprender las relaciones entre la variación genómica, la adaptación ambiental y los procesos ecológicos que ocurren en los ecosistemas marinos.

Aunque las poblaciones de *Prochlorococcus* comparten características generales, presentan diferencias genéticas y fisiológicas relacionadas con factores ambientales como la disponibilidad de luz, la temperatura y la distribución vertical en la columna de agua. Estas diferencias permiten estudiar cómo la diversidad genómica puede contribuir a la coexistencia de linajes con distintos requerimientos ecológicos.

Este proyecto propone utilizar herramientas bioinformáticas para comparar genomas públicos de *Prochlorococcus*, identificar genes compartidos y genes variables, y explorar los patrones de similitud y diferenciación genómica entre los genomas analizados.

El análisis se organiza en un flujo de trabajo reproducible que integra la recuperación de datos, la validación taxonómica, la anotación genómica, la construcción de un pangenoma y el análisis estadístico y gráfico de los resultados.

**Pregunta central:** ¿Cómo varía la composición génica entre los genomas de *Prochlorococcus* y qué patrones de diferenciación genómica pueden identificarse a partir de sus genes compartidos y variables?

> **Alcance:** la comparación de genomas permite describir patrones de diversidad y formular hipótesis ecológicas. Sin embargo, la asociación entre genes y condiciones ambientales requiere metadatos ambientales adecuados y evidencia adicional; no puede inferirse causalidad únicamente a partir de una matriz de presencia y ausencia de genes.

---

## 2. Justificación

El estudio de la diversidad genómica permite ampliar la comprensión de la diversidad biológica más allá de las diferencias observables entre organismos. En microorganismos marinos, la variación en el contenido génico puede contribuir a explicar diferencias en el uso de recursos, la tolerancia a condiciones ambientales y las estrategias de adaptación.

Desde la ecología, este enfoque resulta relevante porque conecta la información genética con procesos como la distribución de los organismos, la diferenciación de poblaciones y la respuesta potencial ante cambios ambientales.

La genómica comparativa ofrece herramientas para identificar genes conservados, genes variables y grupos de genes que podrían estar relacionados con funciones ecológicas particulares. A su vez, el uso de datos públicos permite desarrollar un análisis reproducible sin requerir necesariamente la generación de nuevas secuencias experimentales.

El proyecto integra ecología marina, evolución, genética, estadística y programación, y muestra cómo los datos genómicos pueden convertirse en información útil para formular preguntas ecológicas.

## 3. Objetivos

### Objetivo general

Analizar la diversidad y diferenciación genómica de genomas públicos de *Prochlorococcus* mediante herramientas bioinformáticas y estadísticas, con énfasis en la composición del pangenoma y los patrones de similitud entre genomas.

### Objetivos específicos

1. Recuperar genomas públicos y metadatos asociados a los aislamientos de *Prochlorococcus*.
2. Validar la identidad taxonómica, la calidad y la procedencia de los genomas seleccionados.
3. Estandarizar la anotación de los genomas para facilitar su comparación.
4. Construir una matriz de presencia y ausencia de grupos génicos para caracterizar el pangenoma.
5. Identificar genes compartidos y variables entre los genomas analizados.
6. Calcular medidas de similitud o disimilitud genómica y explorar patrones de agrupamiento.
7. Generar tablas y visualizaciones reproducibles mediante Python y R.
8. Discutir los resultados desde una perspectiva ecológica y evolutiva, considerando las limitaciones de los datos disponibles.

## 4. Hipótesis de trabajo

Los genomas de *Prochlorococcus* presentarán una combinación de genes conservados y genes variables. La proporción de genes compartidos y la composición del repertorio génico podrían diferir entre los genomas, reflejando distintos grados de similitud y diferenciación evolutiva.

Si se dispone de metadatos ambientales confiables, será posible explorar si algunos patrones de composición génica coinciden con diferencias en las condiciones ambientales de los aislamientos.

Esta hipótesis se evaluará mediante los resultados del análisis, no se asumirá como verdadera antes de obtenerlos.

---

## 5. Organismo de estudio

### *Prochlorococcus* spp.

*Prochlorococcus* es un género de cianobacterias marinas unicelulares que realiza fotosíntesis oxigénica y contribuye a la producción primaria de los océanos. Es especialmente abundante en regiones oceánicas cálidas y oligotróficas, donde la disponibilidad de nutrientes puede ser limitada.

Entre sus características relevantes se encuentran:

- Tamaño celular reducido.
- Alta abundancia en distintos ambientes oceánicos.
- Diversidad genética y fisiológica entre linajes.
- Diferencias en los requerimientos y la tolerancia a condiciones de luz.
- Adaptaciones relacionadas con la disponibilidad de nutrientes y otras variables ambientales.

Su diversidad hace posible estudiar cómo la evolución del contenido génico se relaciona con la diferenciación entre linajes y con la ocupación de distintos nichos ecológicos.

**Importante:** la ecología de cada genoma no debe asignarse únicamente a partir de su nombre o de su agrupamiento genético. Para comparar adaptaciones ambientales es necesario verificar la procedencia del aislamiento y sus metadatos.

---

## 6. Fuente de datos

El proyecto utiliza genomas y metadatos de acceso público disponibles en repositorios de secuencias biológicas.

### Fuente inicial

**NCBI BioProject: PRJNA664924**

https://www.ncbi.nlm.nih.gov/bioproject/PRJNA664924

Este proyecto constituye un punto de partida para localizar genomas asociados con aislamientos de *Prochlorococcus*. La descripción del conjunto incluye genomas de aislamientos objetivo y bacterias heterótrofas asociadas a cultivos. Por ello, no deben descargarse ni analizarse todos los registros como si pertenecieran al mismo género.

### Fuentes complementarias

- **NCBI Assembly:** registros de ensamblajes genómicos y metadatos.
  https://www.ncbi.nlm.nih.gov/datasets/
- **NCBI BioProject:** información sobre proyectos de secuenciación.
  https://www.ncbi.nlm.nih.gov/bioproject/
- **NCBI Taxonomy:** consulta y validación de nombres taxonómicos.
  https://www.ncbi.nlm.nih.gov/taxonomy

### Criterios de selección

Antes de realizar el análisis, cada genoma deberá evaluarse considerando:

1. Identidad taxonómica compatible con el objetivo del proyecto.
2. Accesión de ensamblaje y versión verificables.
3. Disponibilidad de los archivos genómicos requeridos.
4. Calidad y nivel de ensamblaje documentados.
5. Ausencia de contaminación evidente o de secuencias pertenecientes a otros organismos.
6. Disponibilidad de metadatos útiles para la interpretación.

Los registros que correspondan a bacterias heterótrofas asociadas a los cultivos deberán excluirse del análisis principal del pangenoma de *Prochlorococcus*, salvo que se diseñe explícitamente una comparación distinta.

El número final de genomas se determinará después de verificar los registros y aplicar los criterios de inclusión. No se considera confirmado hasta completar esta etapa.

---

## 7. Metodología general

El flujo de trabajo se divide en seis etapas.

### Etapa 1. Recuperación y organización de datos

Se identifican las accesiones de los ensamblajes, se recuperan los archivos genómicos y se registran los metadatos disponibles.

Cada registro deberá conservar, como mínimo, el identificador del ensamblaje, el nombre taxonómico, el origen del dato y la decisión de inclusión o exclusión.

**Producto:** una tabla de metadatos y un conjunto de genomas seleccionados.

### Etapa 2. Control de calidad y validación taxonómica

Se revisa la identidad de los organismos, la integridad de los archivos y la información disponible sobre la calidad de los ensamblajes.

Esta etapa es fundamental para evitar que la contaminación, los registros duplicados o la inclusión de especies no objetivo distorsionen la comparación.

**Producto:** un conjunto de genomas documentado y apto para continuar con el análisis.

### Etapa 3. Anotación genómica

Los genomas seleccionados se anotan con una herramienta uniforme, como **Prokka**, para identificar y describir características génicas a partir de las secuencias.

Utilizar el mismo procedimiento de anotación ayuda a reducir las diferencias que podrían surgir por el uso de métodos distintos entre los genomas.

**Producto:** archivos de anotación y secuencias de proteínas predichas, según los formatos generados por la herramienta.

### Etapa 4. Construcción del pangenoma

Se utiliza **Panaroo** para agrupar genes homólogos entre los genomas y construir una matriz que represente la presencia o ausencia de cada grupo génico.

El pangenoma permite distinguir, de forma operativa, entre:

- **Núcleo genómico:** genes presentes en todos los genomas analizados.
- **Genes accesorios:** genes presentes en una parte de los genomas.
- **Genes específicos del conjunto de datos:** genes detectados en uno o pocos genomas, según el criterio utilizado.

La clasificación exacta dependerá de los parámetros del análisis, del número de genomas y de la calidad de las anotaciones.

**Producto:** matriz de presencia y ausencia de genes y archivos de resultados del pangenoma.

### Etapa 5. Análisis estadístico y comparativo

La matriz de presencia y ausencia se utiliza para calcular medidas de similitud o disimilitud entre genomas. Una alternativa es la distancia de Jaccard, que compara la proporción de elementos compartidos respecto del total de elementos presentes en al menos uno de los dos conjuntos.

También pueden explorarse:

- Frecuencia de los grupos génicos.
- Distribución de genes compartidos y variables.
- Matrices de distancia.
- Agrupamientos y dendrogramas exploratorios.
- Patrones de similitud en la composición génica.

Estos análisis describen la similitud del contenido génico; no equivalen por sí mismos a una reconstrucción filogenética.

### Etapa 6. Visualización e interpretación ecológica

Los resultados se organizan en tablas, figuras y descripciones que permitan interpretar los patrones observados.

La discusión considerará la ecología de *Prochlorococcus*, la diferenciación genómica y las limitaciones de los metadatos disponibles. Las interpretaciones sobre adaptación ambiental se plantearán como hipótesis cuando no exista evidencia suficiente para establecer relaciones directas.

---

## 8. Herramientas bioinformáticas

| Herramienta | Función en el proyecto |
|---|---|
| NCBI Datasets / NCBI Assembly | Recuperación de genomas y metadatos |
| Python | Automatización, validación y análisis de archivos |
| Prokka | Anotación genómica uniforme |
| Panaroo | Construcción y análisis del pangenoma |
| R | Análisis estadístico y visualización |
| Git y GitHub | Control de versiones y documentación reproducible |

La disponibilidad y compatibilidad de cada herramienta deberá verificarse en el entorno de ejecución. Los comandos y versiones utilizados se documentarán para facilitar la reproducibilidad.

---

## 9. Estructura del repositorio

La organización propuesta para el proyecto es la siguiente:

```text
Prochlorococcus_Genomica_Ecologica/
│
├── README.md
├── LICENSE.txt
├── .gitignore
│
├── data/
│   ├── metadata/
│   │   ├── assemblies_seed.csv
│   │   └── NCBI_fuente_y_decisiones.csv
│   └── genomes/
│
├── environment/
│   └── environment.yml
│
├── workflow/
│   └── Prochlorococcus_Colab.ipynb
│
├── scripts/
│   ├── analizar_pangenoma.py
│   └── analizar_resultados.R
│
├── docs/
│   └── PROCEDIMIENTO_DETALLADO.md
│
└── results/
    ├── tables/
    └── figures/
```

**Descripción de los directorios:**

- `data/metadata/`: inventario de genomas, accesiones, fuentes y decisiones de selección.
- `data/genomes/`: genomas descargados para el análisis; pueden mantenerse fuera de Git si ocupan demasiado espacio.
- `environment/`: definición del entorno y las dependencias.
- `workflow/`: cuaderno con el flujo de trabajo documentado.
- `scripts/`: código para procesar y analizar los resultados.
- `docs/`: metodología detallada, decisiones y procedimientos.
- `results/tables/`: tablas generadas por el análisis.
- `results/figures/`: visualizaciones y figuras finales.

Los nombres representan la estructura prevista del repositorio. Los archivos deberán incorporarse conforme se desarrollen y validen; su presencia en este esquema no significa que todos los análisis ya se hayan ejecutado.

---

## 10. Resultados que se busca obtener

El proyecto busca generar los siguientes productos:

1. **Inventario de genomas:** lista de accesiones y metadatos de los registros incluidos.
2. **Registro de control de calidad:** documentación de las decisiones de inclusión y exclusión.
3. **Anotaciones genómicas:** archivos producidos por el proceso de anotación.
4. **Matriz del pangenoma:** tabla de presencia y ausencia de grupos génicos.
5. **Resumen del contenido génico:** estadísticas sobre genes compartidos y variables.
6. **Matriz de distancias:** comparación de la composición génica entre genomas.
7. **Visualizaciones:** gráficos y agrupamientos exploratorios.
8. **Informe interpretativo:** discusión de los patrones encontrados, las limitaciones y las posibles preguntas futuras.

Los valores numéricos, las cantidades de genes y los patrones de agrupamiento se reportarán únicamente después de ejecutar el flujo de trabajo y comprobar sus archivos de salida.

---

## 11. Reproducibilidad

Para que los resultados puedan verificarse, se propone registrar:

- Accesiones y versiones de los ensamblajes utilizados.
- Fecha de consulta y descarga.
- Criterios de inclusión y exclusión.
- Versiones de Python, R y las herramientas bioinformáticas.
- Parámetros utilizados durante la anotación y la construcción del pangenoma.
- Archivos de entrada y salida de cada etapa.
- Código de análisis y generación de figuras.

Git permite conservar el historial de modificaciones del código y la documentación. GitHub facilita compartir el repositorio, consultar los cambios y reproducir el procedimiento.

Los archivos de gran tamaño, como los genomas completos y los resultados intermedios, deberán gestionarse de manera adecuada para evitar un repositorio innecesariamente pesado.

---

## 12. Limitaciones del estudio

La interpretación de los resultados dependerá de la calidad y representatividad de los genomas disponibles.

Entre las principales limitaciones se consideran:

- Diferencias en la calidad y completitud de los ensamblajes.
- Posibles errores o diferencias en la anotación de genes.
- Representación desigual de los linajes.
- Disponibilidad limitada de metadatos ambientales.
- Dificultad para atribuir una función ecológica específica a un gen únicamente por su presencia.
- Diferencias entre la similitud del contenido génico y la historia evolutiva de los organismos.
- Posibles sesgos derivados de los criterios de selección y los parámetros de análisis.

Por estas razones, los resultados deberán interpretarse dentro del alcance del conjunto de datos utilizado y no como una descripción definitiva de toda la diversidad de *Prochlorococcus* en los océanos.

---

## 13. Conclusión esperada

Este proyecto propone integrar genómica comparativa y análisis ecológico para estudiar la diversidad del contenido génico en *Prochlorococcus*. Mediante el uso de genomas públicos, anotación estandarizada, construcción del pangenoma y análisis estadístico, se busca identificar patrones de conservación y variación genética entre los genomas seleccionados.

La principal contribución será establecer un flujo de trabajo documentado y reproducible que permita transformar datos genómicos públicos en resultados comparables y generar nuevas preguntas sobre la diversidad y diferenciación ecológica de estas cianobacterias marinas.

La conclusión definitiva se redactará después de analizar los resultados obtenidos, evitando atribuir patrones o mecanismos que no estén respaldados por la evidencia.

---

## 14. Referencias y recursos

- **NCBI BioProject.** Proyecto de referencia para localizar los registros genómicos. https://www.ncbi.nlm.nih.gov/bioproject/PRJNA664924
- **NCBI Datasets.** Documentación para descargar genomas. https://www.ncbi.nlm.nih.gov/datasets/docs/v2/how-tos/genomes/download-genome/
- **Prokka.** Herramienta de anotación de genomas procariotas. https://github.com/tseemann/prokka
- **Panaroo.** Herramienta para construir y analizar pangenomas bacterianos. https://github.com/gtonkinhill/panaroo
- **R Project.** Entorno para análisis estadístico y gráficos. https://www.r-project.org/
- **Git.** Sistema de control de versiones. https://git-scm.com/
- **GitHub Docs.** Documentación para administrar repositorios. https://docs.github.com/

---

## 15. Estado del proyecto

El proyecto se encuentra en desarrollo. La metodología y la estructura de análisis definen el procedimiento que se seguirá; la finalización de cada etapa dependerá de la validación de los datos, la ejecución de los programas y la revisión de sus resultados.

**Próximo paso:** verificar y descargar el conjunto definitivo de genomas de *Prochlorococcus*, ejecutar la anotación y construir el pangenoma para generar las tablas y figuras que sustentan las conclusiones.

<p align="center">
  <i>Ecología + genómica + bioinformática: de los datos moleculares a las preguntas ecológicas.</i>
</p>
