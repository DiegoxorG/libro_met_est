# Análisis de la severidad motora en la enfermedad de Parkinson mediante características acústicas de telemonitoreo

**Autores:** Diego Payares & Salma Romero
**Curso:** Métodos Estadísticos — Universidad del Norte

Libro escrito con [bookdown](https://bookdown.org/) que documenta el análisis
exploratorio (EDA) e inferencial del conjunto de datos
[Parkinsons Telemonitoring](https://archive.ics.uci.edu/dataset/189/parkinsons+telemonitoring)
(Tsanas et al., 2010): 5.875 grabaciones de voz de 42 pacientes con Parkinson
en etapa temprana, con 16 medidas acústicas, variables demográficas/temporales
y las puntuaciones clínicas `motor_UPDRS` (variable respuesta) y `total_UPDRS`.

## Estructura

| Archivo | Contenido |
|---|---|
| `index.Rmd` | Contexto del problema, objetivo general y objetivos específicos |
| `01-intro.Rmd` | Análisis exploratorio de datos (EDA) e ingeniería de características |
| `02-inferencial.Rmd` | Estadística inferencial: supuestos, pruebas de hipótesis y tamaños del efecto (a nivel de paciente) |
| `06-references.Rmd` | Referencias |
| `data/parkinsons_updrs.data` | Datos (CSV) |
| `data/parkinsons_updrs.names` | Diccionario de variables |
| `docs/` | Libro renderizado (GitHub Pages) |

## Cómo compilar

Desde RStudio: abrir `metest.Rproj` y usar **Build > Build Book**, o desde R:

```r
bookdown::render_book("index.Rmd", "bookdown::gitbook")
```

El resultado se escribe en `docs/`.

## Paquetes necesarios

`bookdown`, `tidyverse`, `moments`, `scales`, `patchwork`, `GGally`, `Amelia`,
`effsize`, `nortest`, `car`, `rstatix`, `coin`, `dunn.test`.
