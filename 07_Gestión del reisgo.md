# 07 · Risk Management

## 1. Concepto general

La **gestión de riesgos** es el proceso de **identificar, analizar, tratar y monitorear** los riesgos que pueden afectar activos, operaciones o reputación de una organización.
El objetivo es **reducir probabilidad e impacto** hasta un nivel aceptable según la tolerancia al riesgo.

---

## 2. Ciclo de vida de la gestión de riesgos

### 2.1 Identificación del riesgo

* Detectar eventos que amenazan los objetivos de la empresa
* Fuentes: financieras, operativas, tecnológicas, regulatorias, humanas
* Herramientas: brainstorming, análisis de escenarios, entrevistas, checklists

### 2.2 Análisis del riesgo

Evaluación basada en:

* **Probabilidad (Likelihood)**
* **Impacto (Impact)**

Métodos:

* **Cualitativo** → clasificación subjetiva (alto/medio/bajo)
* **Cuantitativo** → valores numéricos y métricas financieras

### 2.3 Tratamiento del riesgo (Risk Treatment)

| Estrategia                | Acción                                     |
| ------------------------- | ------------------------------------------ |
| **Avoid (Evitar)**        | Eliminar la causa del riesgo               |
| **Mitigate (Reducir)**    | Aplicar controles técnicos/administrativos |
| **Transfer (Transferir)** | Seguros, outsourcing, proveedores          |
| **Accept (Aceptar)**      | Asumir el riesgo residual                  |

### 2.4 Monitoreo y revisión

* Supervisión continua de riesgos y controles
* Actualizar el **Risk Register** regularmente

---

## 3. Herramientas clave

| Herramienta                   | Función                                                                |
| ----------------------------- | ---------------------------------------------------------------------- |
| **Risk Register**             | Documento con riesgos, impacto, probabilidad, responsable y mitigación |
| **KRI (Key Risk Indicators)** | Métricas de alerta temprana                                            |
| **Risk Owner**                | Persona responsable de gestionar un riesgo específico                  |

---

## 4. Tipos de evaluación de riesgos

| Tipo           | Descripción                              | Ejemplo                      |
| -------------- | ---------------------------------------- | ---------------------------- |
| **Ad-Hoc**     | Evaluación puntual ante un evento        | Brecha de seguridad          |
| **Recurrente** | Evaluación periódica (anual, trimestral) | Auditoría TI anual           |
| **One-Time**   | Evaluación ligada a un proyecto puntual  | Lanzamiento de app           |
| **Continua**   | Monitoreo constante                      | SIEM, detección de anomalías |

---

## 5. Métodos de análisis

### Análisis cualitativo

* Enfoque subjetivo basado en experiencia
* Usa escalas → bajo / medio / alto
* **Ventaja:** rápido y simple
* **Desventaja:** menos preciso

### Análisis cuantitativo

Convierte riesgos en valores financieros:

| Métrica                                 | Definición              | Fórmula                  |
| --------------------------------------- | ----------------------- | ------------------------ |
| **EF (Exposure Factor)**                | % de pérdida del activo | —                        |
| **SLE (Single Loss Expectancy)**        | Pérdida por incidente   | `SLE = Asset Value × EF` |
| **ARO (Annualized Rate of Occurrence)** | Frecuencia anual        | —                        |
| **ALE (Annualized Loss Expectancy)**    | Pérdida anual           | `ALE = SLE × ARO`        |

---

## 6. Tolerancia y apetito de riesgo

### Risk Appetite

Nivel de riesgo que la organización está dispuesta a aceptar.

Tipos:

* **Expansionary** → acepta riesgos altos
* **Conservative** → minimiza riesgos
* **Neutral** → equilibrio

### Risk Tolerance

Límite máximo permitido antes de tomar medidas.

---

## 7. Estrategias de gestión

* **Transferir** → seguros, proveedores
* **Mitigar** → firewalls, cifrado, capacitación
* **Evitar** → eliminar procesos riesgosos
* **Aceptar** → documentar y monitorear riesgo residual

---

## 8. Business Impact Analysis (BIA)

Evalúa el impacto de interrupciones sobre funciones críticas del negocio.

### Métricas BIA

| Métrica                               | Definición                               | Ejemplo                  |
| ------------------------------------- | ---------------------------------------- | ------------------------ |
| **RTO (Recovery Time Objective)**     | Tiempo máximo para restaurar un servicio | “Correo en menos de 4 h” |
| **RPO (Recovery Point Objective)**    | Máxima pérdida aceptable de datos        | “Hasta 30 min”           |
| **MTTR (Mean Time To Repair)**        | Tiempo medio de reparación               | 2 horas                  |
| **MTBF (Mean Time Between Failures)** | Tiempo entre fallos                      | 6 meses                  |

---
