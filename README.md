# GENOMICA-PROYECTO-FINAL
Proyecto final de análisis genomicos 
# 🧬 Genómica ecológica de *Prochlorococcus*
## Diversidad genómica y diferenciación ecológica de cianobacterias marinas

# 🧬 Genómica ecológica de *Prochlorococcus*
### Diversidad genómica y diferenciación ecológica de cianobacterias marinas

![Ecología marina](https://img.shields.io/badge/Área-Ecología%20marina-167D8D?style=for-the-badge)
![Bioinformática](https://img.shields.io/badge/Enfoque-Bioinformática-6A5ACD?style=for-the-badge)
![Python y R](https://img.shields.io/badge/Lenguajes-Python%20%7C%20R-3776AB?style=for-the-badge)

## 🌊 ¿De qué trata?

*Prochlorococcus* es una cianobacteria fotosintética fundamental para la producción primaria de los océanos. Sus distintos linajes presentan variaciones genéticas que podrían relacionarse con diferencias en sus adaptaciones y requerimientos ambientales.

Este proyecto utiliza genomas públicos y herramientas bioinformáticas para comparar su contenido génico, identificar genes compartidos y variables, y explorar patrones de diferenciación genómica.

## 🎯 Objetivo

Analizar la diversidad genómica de *Prochlorococcus* mediante la construcción de un pangenoma y la comparación estadística de sus genes, para explorar patrones de similitud y formular hipótesis sobre su diferenciación ecológica.

## ❓ Pregunta de investigación

¿Qué patrones de similitud y diferenciación genómica existen entre los genomas de *Prochlorococcus*, y cómo podrían contribuir a comprender su diversidad ecológica?

## 🧪 Metodología

1. **Obtención de datos:** recuperar genomas y metadatos públicos de NCBI.
2. **Validación:** comprobar la identidad taxonómica y calidad de los ensamblajes.
3. **Anotación:** identificar genes mediante Prokka.
4. **Pangenoma:** agrupar genes homólogos y construir una matriz de presencia y ausencia con Panaroo.
5. **Análisis estadístico:** comparar los genomas mediante Python y R.
6. **Interpretación:** visualizar los patrones encontrados y discutir sus posibles implicaciones ecológicas.

## 💻 Herramientas utilizadas

| Herramienta | Aplicación |
|---|---|
| NCBI | Obtención de genomas públicos |
| Prokka | Anotación genómica |
| Panaroo | Construcción del pangenoma |
| Python | Procesamiento y organización de datos |
| R | Estadística, distancias y visualización |
| GitHub | Documentación y reproducibilidad |

### 📊 ¿Qué se analizará en R?

- Frecuencia de genes compartidos y variables.
- Proporción de genes del núcleo y accesorios.
- Distancias de Jaccard entre genomas.
- Agrupamientos exploratorios mediante dendrogramas.
- Gráficos comparativos y visualizaciones de la diversidad genómica.

## 🔬 Posibles resultados

Los resultados dependerán de los genomas seleccionados y del análisis realizado. Se esperan evaluar los siguientes patrones:

- **Núcleo genómico:** genes presentes en todos los genomas analizados, potencialmente asociados con funciones conservadas.
- **Genes accesorios:** genes presentes solo en una parte de los genomas, que podrían reflejar diferencias funcionales.
- **Diferenciación genómica:** grupos de genomas con mayor similitud en su contenido génico.
- **Variación entre linajes:** diferencias en la composición génica que podrían orientar futuras investigaciones sobre adaptación ambiental.

Estos son resultados esperados, no hallazgos confirmados. Para relacionar los patrones genómicos con condiciones ambientales será necesario contar con metadatos confiables y evidencia adicional.

## 🌱 Importancia ecológica

La comparación genómica permite estudiar la diversidad microbiana desde una perspectiva evolutiva y ecológica. Comprender cómo varía el contenido génico de *Prochlorococcus* puede ayudar a formular hipótesis sobre sus estrategias de adaptación y su papel en los ecosistemas oceánicos.

## 📚 Fuentes

- NCBI BioProject: https://www.ncbi.nlm.nih.gov/bioproject/PRJNA664924
- NCBI Datasets: https://www.ncbi.nlm.nih.gov/datasets/
- Prokka: https://github.com/tseemann/prokka
- Panaroo: https://github.com/gtonkinhill/panaroo
- R Project: https://www.r-project.org/

---

**Estado del proyecto:** en desarrollo. Los resultados definitivos se incorporarán después de validar los genomas y ejecutar el flujo de análisis.

*Ecología + genómica + bioinformática: de los genes a las preguntas ecológicas.*
