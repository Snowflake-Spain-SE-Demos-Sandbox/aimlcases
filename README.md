# Snowflake — Aceleradores IA/ML por Industria

Colección de **notebooks Snowflake** y **prompts de Cortex Code** listos para desplegar, organizados por vertical de industria. Cada caso de uso incluye datos sintéticos, modelos ML/NLP y dashboards Streamlit interactivos — todo 100% nativo en Snowflake.

🔗 **[Ver sitio web](https://dsanchezfernandez.github.io/gitpages/)**

---

## Estructura del Proyecto

```
├── index.html                  # Página principal — índice de industrias
├── seguros.html                # Página de seguros (17 casos de uso)
├── seguros/                    # Notebooks de seguros
│   ├── notebook_uc01_fraude.ipynb
│   ├── notebook_uc02_accidentes_simulados.ipynb
│   ├── ...
│   └── notebook_uc17_compliance.ipynb
├── bug-white.png               # Logo Snowflake
└── README.md
```

## Industrias

| Industria | Estado | Casos de Uso |
|---|---|---|
| **Seguros** | ✅ Disponible | 17 |
| Salud | 🔜 Próximamente | — |
| Farmacéutica | 🔜 Próximamente | — |
| Banca y Servicios Financieros | 🔜 Próximamente | — |
| Retail y E-Commerce | 🔜 Próximamente | — |
| Manufactura e Industria | 🔜 Próximamente | — |
| Telecomunicaciones | 🔜 Próximamente | — |
| Energía y Utilities | 🔜 Próximamente | — |
| Logística y Transporte | 🔜 Próximamente | — |
| Educación | 🔜 Próximamente | — |
| Sector Público | 🔜 Próximamente | — |

## Seguros — Casos de Uso

### Detección de Fraude
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC01 | Puntuación de Fraude en Siniestros | ML.CLASSIFICATION |
| UC02 | Detección de Accidentes Simulados | ML.CLASSIFICATION |
| UC03 | Fraude en Solicitudes de Identidad Sintética | ML.CLASSIFICATION |

### Riesgo y Suscripción
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC04 | Puntuación Dinámica de Riesgo Auto | ML.CLASSIFICATION |
| UC05 | Analítica de Exposición a Catástrofes | SQL Analítico |
| UC06 | Predicción de Fuga en Renovación | ML.CLASSIFICATION |
| UC07 | Segmentación de Riesgo Telemático | ML.CLASSIFICATION |

### IA y Lenguaje Natural
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC08 | Extracción Documental con IA | CORTEX.COMPLETE |
| UC09 | Inteligencia de Quejas de Clientes | CORTEX.SENTIMENT + COMPLETE |
| UC10 | Asistente de Consultas de Póliza | Cortex Search + RAG |

### Gestión de Siniestros
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC11 | Predicción de Severidad en Siniestros | ML.CLASSIFICATION |
| UC12 | Identificación de Oportunidades de Subrogación | ML.CLASSIFICATION |

### Call Center IA
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC13 | Clasificación Automática de Llamadas | CORTEX.COMPLETE + SENTIMENT |
| UC14 | Evaluación Automática de Agentes (QA) | CORTEX.COMPLETE + SENTIMENT |
| UC15 | Generación Automática de Resúmenes | CORTEX.COMPLETE |
| UC16 | Mejora de CX en Tiempo Real | CORTEX.SENTIMENT + Alertas |
| UC17 | Cumplimiento Normativo (Compliance) | CORTEX.COMPLETE |

## Cómo Usar

1. **Descargar** un notebook desde la web o clonar este repositorio
2. **Importar** el `.ipynb` en Snowsight (Notebooks)
3. **Ejecutar** las celdas secuencialmente — cada notebook crea su propia base de datos con datos sintéticos
4. **Personalizar** reemplazando los datos sintéticos con tus propios datos

## Requisitos

- Cuenta de Snowflake con acceso a:
  - `SNOWFLAKE.ML.CLASSIFICATION` (UC01-04, 06-07, 11-12)
  - `SNOWFLAKE.CORTEX.COMPLETE` (UC08-10, 13-17)
  - `SNOWFLAKE.CORTEX.SENTIMENT` (UC09, 13-14, 16)
  - Cortex Search Service (UC10)
- Warehouse `SMALL` o superior
- Rol con permisos `CREATE DATABASE`

## Stack Tecnológico

- **Snowflake Cortex AI** — LLM inference (mistral-large2), sentiment analysis
- **Snowflake Cortex ML** — AutoML classification
- **Snowflake Cortex Search** — RAG pipelines
- **Streamlit in Snowflake** — Dashboards interactivos embebidos en notebooks
- **GitHub Pages** — Hosting estático del catálogo web

---

Desarrollado con Snowflake Cortex AI + Streamlit
