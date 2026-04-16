# Snowflake — Aceleradores IA/ML por Industria

Colección de **guías detalladas** y **Cortex Code Prompts** listos para desplegar, organizados por vertical de industria. Cada caso de uso incluye datos sintéticos, modelos ML/NLP y dashboards Streamlit interactivos — todo 100% nativo en Snowflake.

🔗 **[Ver sitio web](https://dsanchezfernandez.github.io/gitpages/)**

---

## Estructura del Proyecto

```
├── index.html                  # Página principal — índice de industrias
├── seguros.html                # Página de seguros (17 casos de uso)
├── farmaceutica.html           # Página de farmacéutica (27 casos de uso)
├── banca.html                  # Página de banca (20 casos de uso)
├── energia.html                # Página de energía
├── agua.html                   # Página de gestión del agua (10 casos de uso)
├── bug-white.png               # Logo Snowflake
└── README.md
```

## Industrias

| Industria | Estado | Casos de Uso |
|---|---|---|
| **Seguros** | ✅ Disponible | 17 |
| **Farmacéutica** | ✅ Disponible | 27 |
| **Banca y Servicios Financieros** | ✅ Disponible | 20 |
| **Gestión del Agua** | ✅ Disponible | 10 |
| **Energía y Utilities** | ✅ Disponible | — |
| Salud | 🔜 Próximamente | — |
| Retail y E-Commerce | 🔜 Próximamente | — |
| Manufactura e Industria | 🔜 Próximamente | — |
| Telecomunicaciones | 🔜 Próximamente | — |
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

## Farmacéutica — Casos de Uso

### Machine Learning
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC01 | Predicción de Riesgo de Adherencia | ML.CLASSIFICATION |
| UC02 | Optimizador de Rendimiento de Campañas | Window Functions / Atribución |
| UC03 | Análisis de Sentimiento del Consumidor | CORTEX.SENTIMENT |
| UC04 | Predicción de Pérdida de Exclusividad | ML.FORECAST |
| UC05 | Optimizador de Engagement con HCPs | ML.CLASSIFICATION |
| UC06 | Chatbot de Inteligencia Comercial | Cortex Analyst |
| UC07 | Segmentación de Consumidores y LTV | SQL NTILE + ML.FORECAST |
| UC08 | Analizador de Efectividad de Contenido | CORTEX.COMPLETE |
| UC09 | Generador de Evidencia del Mundo Real | SQL Analítico |
| UC10 | Monitor de Inteligencia Competitiva | CORTEX.COMPLETE + Marketplace |
| UC11 | Mapeador de Journey Omnicanal | Cadenas de Markov |
| UC12 | Optimizador de Precios y Descuentos | GENERATOR + Elasticidad |
| UC13 | Selector de Centros para Ensayos | Geoespacial ST_DISTANCE |
| UC14 | Predicción de Demanda de Lanzamiento | ML.FORECAST |
| UC15 | Gestor de Compliance de Claims | REGEXP + FLATTEN |

### IA y Lenguaje Natural
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC16 | Detección de Crisis en Redes Sociales | CORTEX.SENTIMENT + Z-score |
| UC17 | Inteligencia de Mensajes de Competidores | Cortex Search + LLM |
| UC18 | Tracker de Sentimiento en Medios Globales | CORTEX.SENTIMENT |
| UC19 | Predictor de Recepción de Lanzamiento | ML.FORECAST + Sentiment |
| UC20 | Red de Sentimiento de KOLs e Influencers | CORTEX.SENTIMENT + Red |
| UC21 | Percepción Competitiva de Producto | CORTEX.SENTIMENT comparativo |
| UC22 | Optimizador de Comunicación Ejecutiva | CORTEX.COMPLETE |
| UC23 | Inteligencia Competitiva Automatizada | CORTEX.COMPLETE + Alertas |
| UC24 | Sentimiento Global Multi-Idioma | CORTEX.TRANSLATE + SENTIMENT |

### Journey del Paciente
| # | Caso de Uso | Tecnología |
|---|---|---|
| UC25 | Journey de Tratamiento del Paciente | CORTEX.SENTIMENT + CLASSIFY_TEXT |
| UC26 | Inteligencia de Adherencia al Tratamiento | CORTEX.COMPLETE + CLASSIFY_TEXT |
| UC27 | Insights de Engagement con HCPs | CORTEX.SENTIMENT + AI_EXTRACT |

## Cómo Usar

1. **Abrir** la web y seleccionar una industria
2. **Explorar** los casos de uso y abrir la **Guía** para entender el contexto y los datos
3. **Copiar** los **Cortex Code Prompts** y ejecutarlos secuencialmente en Cortex Code (Snowflake)
4. **Personalizar** reemplazando los datos sintéticos con tus propios datos

## Requisitos

- Cuenta de Snowflake con acceso a:
  - `SNOWFLAKE.ML.CLASSIFICATION` (Seguros: UC01-04, 06-07, 11-12; Pharma: UC01, 05)
  - `SNOWFLAKE.ML.FORECAST` (Pharma: UC04, 07, 14, 19)
  - `SNOWFLAKE.CORTEX.COMPLETE` (Seguros: UC08-10, 13-17; Pharma: UC06, 08, 10, 17, 22-23)
  - `SNOWFLAKE.CORTEX.SENTIMENT` (Seguros: UC09, 13-14, 16; Pharma: UC03, 16, 18-21, 24-27)
  - `SNOWFLAKE.CORTEX.TRANSLATE` (Pharma: UC24)
  - Cortex Search Service (Seguros: UC10; Pharma: UC17)
- Warehouse `SMALL` o superior
- Rol con permisos `CREATE DATABASE`
- Acceso a **Cortex Code** en Snowflake

## Stack Tecnológico

- **Snowflake Cortex AI** — LLM inference (mistral-large2), sentiment analysis
- **Snowflake Cortex ML** — AutoML classification
- **Snowflake Cortex Search** — RAG pipelines
- **Snowflake Cortex Code** — Prompts guiados paso a paso
- **Streamlit in Snowflake** — Dashboards interactivos
- **GitHub Pages** — Hosting estático del catálogo web

---

Desarrollado con Snowflake Cortex AI + Cortex Code + Streamlit
