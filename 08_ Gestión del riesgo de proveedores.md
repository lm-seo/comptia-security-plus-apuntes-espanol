
# 08 · Third-Party Vendor Risk

## 1. Concepto general

El **riesgo de terceros** aparece cuando una organización depende de proveedores externos, contratistas o socios para manejar datos, infraestructura o servicios críticos.
Si un proveedor sufre una brecha, **tu organización también queda expuesta**.

### Ejemplos comunes

* Servicios en la nube: AWS, Azure, Google Cloud
* Proveedores de software o mantenimiento
* Socios con acceso remoto o a datos de clientes
* Subcontratas de soporte, atención al cliente o marketing

---

## 2. Riesgos principales

| Tipo de Riesgo                          | Descripción                                                     | Ejemplo                          |
| --------------------------------------- | --------------------------------------------------------------- | -------------------------------- |
| **Seguridad de datos**                  | Exposición de datos sensibles por malas prácticas del proveedor | MSP filtra credenciales          |
| **Cumplimiento normativo**              | Incumplimiento de GDPR, HIPAA, PCI-DSS, etc.                    | Multas por uso indebido de datos |
| **Dependencia / Continuidad**           | Caída del proveedor afecta tu operación                         | Fallo del servicio de correo     |
| **Cadena de suministro (Supply Chain)** | Compromiso de un proveedor afecta tu producto                   | Caso SolarWinds                  |
| **Acceso remoto no controlado**         | Proveedores acceden sin seguridad adecuada                      | Cuentas compartidas, sin MFA     |

---

## 3. Proceso de gestión del riesgo de terceros

| Fase                                  | Actividades                                                                                            | Objetivo                             |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------ |
| **Evaluación (Assessment)**           | Identificar proveedores críticos, revisar políticas, certificaciones (ISO 27001, SOC 2), cuestionarios | Determinar riesgo antes de contratar |
| **Mitigación (Mitigation)**           | Controles contractuales, limitar acceso, exigir MFA, segmentación, revisar DR/BCP                      | Reducir probabilidad de incidentes   |
| **Supervisión continua (Monitoring)** | Auditorías, informes de cumplimiento, revisiones de seguridad                                          | Mantener control y visibilidad       |
| **Terminación (Offboarding)**         | Revocar accesos, eliminar datos, solicitar certificado de destrucción                                  | Cierre sin exposición residual       |

---

## 4. Contratos y acuerdos importantes

| Documento                             | Propósito                                        | Contenido clave                                      |
| ------------------------------------- | ------------------------------------------------ | ---------------------------------------------------- |
| **SLA (Service Level Agreement)**     | Define niveles de servicio                       | Disponibilidad, tiempos de respuesta, penalizaciones |
| **MOU / MOA**                         | Acuerdos de entendimiento sin fuerza legal total | Responsabilidades mutuas                             |
| **MSA (Master Service Agreement)**    | Contrato marco                                   | Condiciones generales y legales                      |
| **SOW (Statement of Work)**           | Define tareas y entregables                      | Objetivos y plazos                                   |
| **NDA (Non-Disclosure Agreement)**    | Garantiza confidencialidad                       | Protección de información                            |
| **BPA (Business Partners Agreement)** | Regula relaciones comerciales a largo plazo      | Roles, acceso, responsabilidades                     |

---

## 5. Técnicas de evaluación

* **Vendor Security Questionnaires**
* **Pentesting / Auditorías independientes**
* **Right-to-Audit Clause** → cláusula que permite revisar prácticas del proveedor
* **Certificaciones externas** → ISO 27001, SOC 2 Type II, FedRAMP, CSA STAR
* **Risk Scoring Tools** → BitSight, SecurityScorecard, UpGuard

---

## 6. Mitigación y supervisión continua

* Aplicar **principio de mínimo privilegio** para proveedores
* Requerir **VPN + MFA** para accesos externos
* Revisar logs de acceso remoto regularmente
* Solicitar reportes de cumplimiento (mensuales o trimestrales)
* Evaluar a los subcontratistas del proveedor (**fourth-party risk**)
* Establecer planes de contingencia ante interrupciones o compromisos
