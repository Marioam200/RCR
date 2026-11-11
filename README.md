# RCR — Representación del Conocimiento y Razonamiento

Material de la asignatura **Representación del Conocimiento y Razonamiento (RCR)** del Grado en Ciencia de Datos: apuntes de teoría, boletines de ejercicios con soluciones y prácticas en Jupyter Notebook (Python).

## Estructura

```
RCR/
├── Presentaci_n_RCR.pdf          # Presentación de la asignatura
├── Teor_a/                       # Teoría
│   ├── Tema_1/                   # Introducción
│   ├── Tema_2/                   # Representación del conocimiento basada en la lógica
│   ├── Tema_3-1/                 # Representación y razonamiento con ontologías
│   ├── Tema_3/                   # Tema 4: razonamiento basado en reglas
│   └── Preparaci_n_parcial/      # Ejercicios y soluciones para el parcial
└── Pr_cticas/                    # Boletines de prácticas (notebooks)
```

## Teoría

| Tema | Contenido | Material |
|------|-----------|----------|
| 1 | Introducción | [RCR_Tema_1.pdf](Teor_a/Tema_1/RCR_Tema_1.pdf) |
| 2 | Representación del conocimiento basada en la lógica (LPO, Datalog) | [Apuntes](Teor_a/Tema_2/RCR_Tema_2.pdf), [seminario](Teor_a/Tema_2/Seminario_tema2.pdf), [intro a pyDatalog](Teor_a/Tema_2/intro_pydatalog.pdf), [ejercicios pyDatalog](Teor_a/Tema_2/ejercicios_pydatalog.ipynb) |
| 3 | Representación y razonamiento con ontologías (lógicas descriptivas, OWL, SWRL) | [Apuntes](Teor_a/Tema_3-1/RCR_Tema_3.pdf), boletines de DL/SWRL con soluciones, ontología `GameOntology` (`.owl`) y tutoriales de Owlready2 (básico, razonamiento y SWRL) |
| 4 | Razonamiento basado en reglas | [Apuntes](Teor_a/Tema_3/RCR_Tema_4.pdf), [ejercicios](Teor_a/Tema_3/RCR_Tema_4_ejercicios.pdf) |

### Preparación del parcial

En [`Teor_a/Preparaci_n_parcial`](Teor_a/Preparaci_n_parcial) hay ejercicios de **lógica de primer orden** y de **ontologías**, cada uno con su solución.

## Prácticas

| Notebook | Contenido |
|----------|-----------|
| [Boletín 1](Pr_cticas/RCR_Pra_ct_Boleti_n_1.ipynb) | Carga de datos de OCity (Valencia) con Pandas y visualización en mapas interactivos |
| [Boletín 2](Pr_cticas/RCR_Pra_ct_Boleti_n_2.ipynb) | Uso de ontologías OWL con Owlready2 |
| [Boletín 3](Pr_cticas/RCR_Pra_ct_Boleti_n_3.ipynb) | CLIPSPY (I): COOL, a partir de la ontología del boletín anterior |
| [RCR_Bib_Mapas](Pr_cticas/RCR_Bib_Mapas.ipynb) | Funciones de utilidad para mapas (se incluye con `%run RCR_Bib_Mapas.ipynb`) |
| [Notas sobre COOL y CLIPSPY](Pr_cticas/Notas_sobre_COOL_y_CLIPSPY.ipynb) | Apuntes de COOL (CLIPS Object Oriented Language) con CLIPSPY |

Los datos de las prácticas están en [`2022_05_24_Valencia.json`](Pr_cticas/2022_05_24_Valencia.json).

## Entorno

Los notebooks se han validado con un entorno de **Anaconda** con Python 3.12/3.13. Librerías utilizadas:

- `pandas`
- `folium`, `geopy`, `openrouteservice` — mapas y rutas
- `owlready2` — ontologías OWL, razonamiento y SWRL
- `clipspy` — sistemas basados en reglas (CLIPS / COOL)
- `pyDatalog` — programación lógica

```bash
pip install pandas folium geopy openrouteservice owlready2 clipspy pyDatalog
```

> `openrouteservice` necesita una API key gratuita de [openrouteservice.org](https://openrouteservice.org/) para calcular rutas.
