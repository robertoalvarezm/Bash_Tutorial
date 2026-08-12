# 🧬 Bioinformática en la Línea de Comandos

Tutorial práctico para aprender a utilizar la línea de comandos aplicada a la bioinformática, desde la manipulación de archivos de texto hasta la construcción de flujos de trabajo reproducibles.

El objetivo no es memorizar comandos, sino **entender qué hacen, cuándo utilizarlos y cómo combinarlos para resolver problemas reales de bioinformática**.

---

## 📚 Contenido

El tutorial está organizado de manera progresiva: primero aprenderás a manipular texto, después aplicarás estas herramientas a datos biológicos y finalmente trabajarás con herramientas especializadas, bases de datos y flujos de trabajo integrados.

| Capítulo                             | Contenido principal                                              | Propósito                                                                |
| ------------------------------------ | ---------------------------------------------------------------- | ------------------------------------------------------------------------ |
| **01 · Manipulación de texto**       | `awk`, `sed`, `grep`, `cut`, `sort`, `uniq`, `wc`, `tr`, `paste` | Aprender a transformar, filtrar y resumir texto                          |
| **02 · Datos biológicos**            | FASTA, FASTQ, VCF, BAM, BLAST, paired-end                        | Aplicar las herramientas a formatos utilizados en bioinformática         |
| **03 · Automatización**              | `find`, `xargs`, loops, GNU `parallel`                           | Trabajar con múltiples archivos y muestras                               |
| **04 · `seqtk`**                     | FASTA / FASTQ                                                    | Utilizar herramientas especializadas para el procesamiento de secuencias |
| **05 · GFF3**                        | Anotaciones genómicas                                            | Explorar y analizar archivos de anotación                                |
| **06 · SRA Toolkit**                 | `prefetch`, `fasterq-dump`, `vdb-validate`                       | Obtener y validar datos públicos de secuenciación                        |
| **07 · E-utilities**                 | `einfo`, `esearch`, `efetch`, `elink`, `xtract`                  | Consultar y navegar por las bases de datos del NCBI                      |
| **08 · `gget`**                      | Python + CLI                                                     | Consultar recursos genómicos y realizar análisis programáticos           |
| **09 · NCBI Datasets**               | `datasets`, `dataformat`                                         | Descargar recursos genómicos y metadatos organizados                     |
| **10 · Resumen y recursos**          | Referencia rápida y documentación                                | Repasar conceptos y continuar aprendiendo                                |

---

## 🎯 Objetivos

Al finalizar el tutorial podrás:

* Manipular archivos de texto y datos biológicos desde Bash.
* Construir *pipelines* combinando diferentes comandos.
* Trabajar con formatos como FASTA, FASTQ, VCF, BAM y GFF3.
* Automatizar tareas sobre múltiples archivos y muestras.
* Utilizar `seqtk` para el procesamiento de secuencias.
* Obtener y validar datos públicos mediante SRA Toolkit.
* Consultar las bases de datos del NCBI mediante E-utilities.
* Utilizar `gget` desde Python y desde la línea de comandos.
* Descargar genomas, genes y metadatos mediante NCBI Datasets.
* Integrar diferentes herramientas en flujos de trabajo reproducibles.

---

## 💻 Requisitos

Para aprovechar este tutorial se recomienda contar con:

* conocimientos básicos de la línea de comandos y Bash;
* acceso a una terminal Bash;
* Linux, macOS o Ubuntu mediante WSL en Windows;
* conocimientos básicos de formatos de datos biológicos;
* Python para las secciones que utilizan `gget`.

Las herramientas adicionales se instalarán y explicarán en los capítulos correspondientes.

---

## 🧠 Una idea importante

No necesitas memorizar todos los comandos.

Lo importante es aprender a reconocer **qué problema quieres resolver**, elegir una herramienta apropiada y saber combinarla con otras.

A lo largo del tutorial se repite una misma lógica:

**entrada → transformación → filtrado → salida**

Por ejemplo:

```bash
cat archivo.tsv | grep "gene" | cut -f1 > genes.txt
```

Cada comando realiza una tarea pequeña y la salida de uno puede convertirse en la entrada del siguiente.

También encontrarás una pregunta que se repetirá a lo largo de los capítulos:

> **¿Qué entra?, ¿qué transforma?, ¿qué sale y cómo compruebo que salió bien?**

Esta forma de pensar ayuda a construir *pipelines* más claros, detectar errores y trabajar de manera más reproducible.

---

## 🗂️ Estructura del repositorio

```text
.
├── README.md
├── index.qmd
├── chapters/
│   ├── 01-manipulacion-texto.qmd
│   ├── 02-datos-biologicos.qmd
│   ├── 03-automatizacion.qmd
│   ├── 04-seqtk.qmd
│   ├── 05-gff3.qmd
│   ├── 06-sra-toolkit.qmd
│   ├── 07-eutilities.qmd
│   ├── 08-gget.qmd
│   ├── 09-ncbi-datasets.qmd
│   └── 10-integracion.qmd
├── figures/
└── ...
```

---

## 🚀 ¿Cómo utilizar el tutorial?

Los capítulos están organizados de manera progresiva, por lo que se recomienda recorrerlos en orden.

Si ya tienes experiencia con alguna de las herramientas, también puedes utilizar el índice para acceder directamente al capítulo correspondiente.

Cada capítulo combina:

* 📖 Explicación conceptual
* 💻 Ejemplos de código
* 🧬 Aplicaciones a datos biológicos
* 📝 Ejercicios (preguntas de comprensión y retos prácticos
* 🔎 Preguntas de comprensión
* 🏆 Retos prácticos

La recomendación es **intentar resolver los ejercicios antes de consultar las soluciones**.

---


## 📖 Recursos

Cada capítulo incluye documentación y recursos relacionados con las herramientas utilizadas.

Algunos recursos principales incluyen:

* [Bioinformatics one-liners — Stephen Turner](https://github.com/stephenturner/oneliners)
* [SRA Toolkit Wiki](https://github.com/ncbi/sra-tools/wiki)
* [NCBI Datasets — documentación oficial](https://www.ncbi.nlm.nih.gov/datasets/docs/v2/command-line-tools/download-and-install/)
* [NCBI Datasets — referencia de comandos](https://www.ncbi.nlm.nih.gov/datasets/docs/v2/reference-docs/command-line/datasets/)
* [NCBI E-utilities Documentation](https://www.ncbi.nlm.nih.gov/books/NBK25498/)
* [gget Documentation](https://github.com/pachterlab/gget)
* [seqtk](https://github.com/lh3/seqtk)
* [GNU parallel Tutorial](https://www.gnu.org/software/parallel/parallel_tutorial.html)

---


**🧬 De comandos individuales a workflows reproducibles.**
