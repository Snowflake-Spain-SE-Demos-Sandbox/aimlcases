# Snowflake — Aceleradores IA/ML por Industria

Colección de **guías detalladas** y **Cortex Code Prompts** listos para desplegar, organizados por vertical de industria. Cada caso de uso incluye datos sintéticos, modelos ML/NLP y dashboards Streamlit interactivos — todo 100% nativo en Snowflake.

> **15 industrias · 299 casos de uso · 100% Snowflake nativo**

---

## Ficheros Principales

| Fichero | Descripción |
|---|---|
| `index.html` | Página principal — catálogo de industrias con buscador global |
| `manual.html` | Guía paso a paso para usar Cortex Code en Snowsight |
| `hackathon.html` | Página del hackathon Snowflake |
| `README.md` | Este fichero |
| `SUMMARY_CHANGES.md` | Reglas de optimización de prompts aplicadas (R01–R11) |

---

## Industrias Disponibles — 15 verticales

| # | Industria | Fichero | UCs | Categorías |
|---|---|---|---|---|
| 1 | **Farmacéutica** | `farmaceutica.html` | 27 | Machine Learning · IA y Lenguaje Natural · Journey del Paciente |
| 2 | **Seguros** | `seguros.html` | 36 | Detección de Fraude · Riesgo y Suscripción · IA y Lenguaje Natural · Siniestros · Call Center IA · Asistentes IA · Comercial · Operaciones · Pricing |
| 3 | **Banca** | `banca.html` | 20 | Riesgo y Compliance · Cliente y Negocio · Operaciones y Mercados · Inteligencia Avanzada |
| 4 | **Banca de Inversión y Custodia** | `banca_inversion.html` | 20 | Activos y Custodia · Distribución de Fondos · Trading y Mercados · Cumplimiento y Riesgo · Operaciones |
| 5 | **Retail y E-Commerce** | `retail.html` | 20 | Personalización y CX · Pricing & Revenue · Supply Chain · Marketing & Loyalty · Fraude y Seguridad |
| 6 | **Manufactura** | `manufactura.html` | 15 | Calidad y Producción · Mantenimiento Predictivo · Cadena de Suministro · Operaciones IA |
| 7 | **Hospitality y Turismo** | `hospitality.html` | 20 | Revenue & Pricing · Experiencia del Huésped · Operaciones · Distribución B2B · Fraude y Seguridad |
| 8 | **Logística y Transporte** | `logistica.html` | 20 | Rutas y Última Milla · Almacén y Fulfillment · Flota y Mantenimiento · Demanda y Planificación · Seguridad |
| 9 | **Medios Audiovisuales** | `medios.html` | 20 | Contenido y Producción · Audiencia y Engagement · Publicidad y Monetización · Distribución · Seguridad |
| 10 | **Telecomunicaciones** | `telecom.html` | 20 | Red y Conectividad · Experiencia de Cliente · Operaciones y Eficiencia · Monetización · Seguridad |
| 11 | **Energía y Utilities** | `energia.html` | 20 | Generación Renovable · Red y Smart Grid · Experiencia de Cliente · Operaciones · Seguridad |
| 12 | **Sector Público** | `sector_publico.html` | 20 | Experiencia Ciudadana · Políticas Públicas · Fraude y Control · Eficiencia Administrativa · Smart Cities |
| 13 | **Salud y Hospitales** | `salud.html` | 20 | Atención al Paciente · Datos Clínicos · Operaciones · Crónicos · Seguridad |
| 14 | **Educación** | `educacion.html` | 20 | Experiencia Estudiante · Gestión Académica · Admisiones · Investigación · Operaciones |
| 15 | **Managed Services** | `managed_services.html` | 20 | Fuerza Laboral · Seguridad y Vigilancia · Seguridad Bancaria CIT · Limpieza y Auxiliares · Clientes y SLA · ESG |

> **Total: 299 casos de uso** distribuidos en 15 industrias

---

## Casos de Uso con Feature Store y Model Registry

Los siguientes casos de uso demuestran capacidades avanzadas de MLOps en Snowflake:

### Feature Store (`SNOWFLAKE.ML.FEATURE_STORE`)
| Industria | UC | Entity | FeatureViews |
|---|---|---|---|
| Seguros | UC21 – Optimización Comercial de Oficinas | `OFICINA` | 6 FeatureViews de rendimiento, zona y cartera |
| Seguros | UC30 – Sofisticación Pricing Hogar | `RIESGO_HOGAR` | 5 FeatureViews: catastral, siniestralidad, clima, sociodemográfico, IoT |
| Banca de Inversión | UC01 – Reconciliación de Posiciones | `CUENTA_CUSTODIA` | 6 FeatureViews: posiciones, confirmaciones, SWIFT, riesgo, histórico, mercado |
| Banca de Inversión | UC20 – Fallos de Liquidación | `OPERACION_LIQUIDACION` | 8 FeatureViews de contraparte, instrucción, valores, posición, mercado, broker |
| Managed Services | UC01 – Predicción de Absentismo | `EMPLEADO_360` | 6 FeatureViews: ausencias, turno, contrato, rendimiento, contexto, zona |

### Model Registry (`SNOWFLAKE.ML.MODEL_REGISTRY`)
| Industria | UC | Modelo | Versiones |
|---|---|---|---|
| Seguros | UC28 – Smart Triage | `smart_triage_model` | v1 / v2 con métricas |
| Seguros | UC33 – Score Pricing Low Cost | `low_cost_pricing_model` | v1 conservador / v2 agresivo + A/B testing |
| Banca de Inversión | UC08 – Flujos de Fondos | `flujos_fondos_model` | v1 / v2 |
| Banca de Inversión | UC20 – Fallos de Liquidación | `settlement_failure_model` | v1 / v2 |
| Retail | UC01 – Dynamic Pricing | `pricing_model` | v1 / v2 |
| Managed Services | UC05 – Riesgo de Instalación | `incident_risk_model` | v1 / v2 |
| Managed Services | UC14 – Gestión de Consumibles | `consumibles_model` | v1 / v2 |
| Managed Services | UC17 – Churn de Contratos | `contract_churn_model` | v1 / v2 + A/B testing |

---

## Estructura de Cada Caso de Uso

Cada uno de los 299 casos de uso incluye tres capas de contenido:

```
UC_XX — Nombre del Caso de Uso
├── Card              → Badge ID + categoría + tiempo estimado
│                       Problema (pain point) + descripción + features clave
│                       Botones: [Ver Guía] [Cortex Code Prompts]
│
├── Guía              → Contexto de negocio · Foco · Reto
│                       Objetivos de aprendizaje · Funcionalidades
│                       Datos generados · Estratificación · Cómo usar
│
└── Cortex Code       → 9–12 prompts secuenciales ejecutables en Snowsight
    Prompts             Paso 1: Configurar entorno (DB + warehouse)
                        Paso 2–N: Datos sintéticos → Feature engineering
                                  → Entrenar modelo → Evaluar → Dashboard
                        Último: Limpieza opcional
```

---

## Buenas Prácticas Aplicadas (SUMMARY_CHANGES.md)

Todos los prompts han sido optimizados siguiendo las reglas documentadas en `SUMMARY_CHANGES.md`:

| Regla | Severidad | Descripción |
|---|---|---|
| R01 | CRITICAL | Columna target ML debe ser `VARCHAR`/`BOOLEAN`, no `FLOAT` |
| R02 | RECOMMENDED | `evaluate => TRUE` explícito en todos los entrenamientos ML |
| R04 | CRITICAL | `OBJECT_CONSTRUCT(* EXCLUDE (target_col))` en `!PREDICT` |
| R06 | RECOMMENDED | `GENERATOR(ROWCOUNT => N)` con `UNIFORM()` para datos sintéticos |
| R11 | RECOMMENDED | `snowflake.connector.connect()` para dashboards Streamlit locales |

---

## Estructura de Ficheros

```
├── index.html                    # Catálogo principal — 15 industrias, 299 UCs
├── manual.html                   # Guía de uso de Cortex Code (12 secciones)
├── hackathon.html                # Página del hackathon Snowflake
│
├── farmaceutica.html             # Farmacéutica (27 UCs)
├── seguros.html                  # Seguros (36 UCs)
├── banca.html                    # Banca (20 UCs)
├── banca_inversion.html          # Banca de Inversión y Custodia (20 UCs)
├── retail.html                   # Retail y E-Commerce (20 UCs)
├── manufactura.html              # Manufactura (15 UCs)
├── hospitality.html              # Hospitality y Turismo (20 UCs)
├── logistica.html                # Logística y Transporte (20 UCs)
├── medios.html                   # Medios Audiovisuales (20 UCs)
├── telecom.html                  # Telecomunicaciones (20 UCs)
├── energia.html                  # Energía y Utilities (20 UCs)
├── sector_publico.html           # Sector Público (20 UCs)
├── salud.html                    # Salud y Hospitales (20 UCs)
├── educacion.html                # Educación (20 UCs)
├── managed_services.html         # Managed Services (20 UCs)
│
├── SUMMARY_CHANGES.md            # Reglas de optimización de prompts
└── README.md                     # Este fichero
```

---

## Cómo Usar

1. **Abrir** `index.html` y seleccionar una industria
2. **Explorar** los casos de uso — leer el `Problema` y la descripción de cada card
3. **Abrir la Guía** para entender el contexto de negocio y los datos generados
4. **Copiar los Cortex Code Prompts** y ejecutarlos secuencialmente en Cortex Code (Snowsight)
5. **Personalizar** reemplazando los datos sintéticos con los datos reales de tu cliente

---

## Requisitos Técnicos

- Cuenta de Snowflake con acceso a **Cortex AI/ML**:
  - `SNOWFLAKE.ML.CLASSIFICATION` — modelos de clasificación binaria y multiclase
  - `SNOWFLAKE.ML.FORECAST` — forecasting de series temporales
  - `SNOWFLAKE.ML.ANOMALY_DETECTION` — detección de anomalías no supervisada
  - `SNOWFLAKE.ML.FEATURE_STORE` — Feature Store para MLOps
  - `SNOWFLAKE.ML.MODEL_REGISTRY` — registro y versionado de modelos
  - `SNOWFLAKE.CORTEX.COMPLETE` — LLM inference (snowflake-arctic, mistral, llama)
  - `SNOWFLAKE.CORTEX.SENTIMENT` — análisis de sentimiento
  - `SNOWFLAKE.CORTEX.EMBED_TEXT` — embeddings para búsqueda semántica
  - `VECTOR_COSINE_SIMILARITY` — similitud vectorial para clustering
  - `CORTEX SEARCH SERVICE` — RAG pipelines y búsqueda semántica
- Warehouse `SMALL` o superior (auto-suspend 60s recomendado)
- Rol con permisos `CREATE DATABASE`
- Acceso a **Cortex Code** en Snowsight

---

## Stack Tecnológico

| Componente | Uso |
|---|---|
| **Snowflake Cortex AI** | LLM inference, sentiment, embeddings, translate, summarize |
| **Snowflake Cortex ML** | AutoML: classification, forecasting, anomaly detection |
| **Snowflake Feature Store** | Centralización de features para MLOps |
| **Snowflake Model Registry** | Versionado, A/B testing y gobierno de modelos |
| **Snowflake Cortex Search** | RAG pipelines y búsqueda semántica sobre documentos |
| **Snowflake Cortex Code** | Prompts guiados paso a paso con skills de best-practices |
| **Streamlit in Snowflake** | Dashboards interactivos integrados con los modelos |
| **GitHub Pages** | Hosting estático del catálogo web |

---

Desarrollado con Snowflake Cortex AI + Feature Store + Model Registry + Cortex Code
