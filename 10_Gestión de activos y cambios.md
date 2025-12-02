# 10 · Asset and Change Management

## 1. Concepto general

### Asset Management (Gestión de activos)

Proceso de **identificar, registrar, clasificar y supervisar** todos los activos de la organización:
hardware, software, datos, personas, redes y servicios.
Permite conocer:

* Qué activos existen
* Quién los usa
* Su importancia
* Su estado de seguridad

### Change Management (Gestión de cambios)

Proceso controlado para **introducir modificaciones** en sistemas o infraestructura **sin afectar disponibilidad ni seguridad**.
Todo cambio debe ser **planificado, probado, aprobado, documentado y monitoreado**.

Ambos procesos aseguran la **estabilidad, continuidad y seguridad** del entorno TI.

---

## 2. Objetivos principales

### Gestión de activos

* Inventario actualizado de hardware, software y servicios
* Detectar dispositivos no autorizados o sin parches
* Asignar propietario, ubicación y clasificación del activo
* Facilitar gestión de riesgos y cumplimiento normativo

### Gestión de cambios

* Reducir errores y downtime
* Prevenir cambios no autorizados (**shadow IT**)
* Documentar y auditar todo cambio
* Mantener **CIA** durante actualizaciones

---

## 3. Ciclo de vida de los activos

1. **Identificación y adquisición**
   Registro inicial del activo al ingresar en la organización

   * Ejemplo: documentar serie, dueño, ubicación

2. **Clasificación**
   Determinar sensibilidad e importancia

   * Ejemplo: “Datos de clientes = confidencial”

3. **Uso y mantenimiento**
   Supervisar parches, configuración y estado operativo

4. **Desmantelamiento / Eliminación segura**
   Sanitización de datos, borrado seguro, destrucción o reciclaje

---

## 4. Tipos de activos a gestionar

* **Hardware:** servidores, portátiles, móviles, routers, firewalls
* **Software:** SO, aplicaciones, licencias, firmware
* **Datos:** bases de datos, documentos, propiedad intelectual
* **Personas:** usuarios finales, administradores, terceros
* **Infraestructura virtual y cloud:** VMs, contenedores, SaaS/PaaS/IaaS

> Ejemplo: una CMDB detecta equipos no autorizados conectándose a la red.

---

## 5. Proceso de gestión de cambios (Change Management Lifecycle)

| Etapa                              | Actividades                                              |
| ---------------------------------- | -------------------------------------------------------- |
| **RFC – Request for Change**       | Documentar motivo, impacto, recursos y plan de reversión |
| **Evaluación y aprobación**        | El CAB revisa riesgos y aprueba/rechaza                  |
| **Pruebas y validación**           | Ensayos en entorno de staging o laboratorio              |
| **Implementación**                 | Cambio aplicado en ventana de mantenimiento              |
| **Revisión post-cambio**           | Lecciones aprendidas y verificación de resultados        |
| **Actualización de documentación** | Inventarios, diagramas y CMDB actualizados               |

---

## 6. Tipos de cambios

| Tipo           | Descripción                             | Ejemplo                       |
| -------------- | --------------------------------------- | ----------------------------- |
| **Estándar**   | Rutinario, preaprobado, bajo riesgo     | Actualización antivirus       |
| **Normal**     | Requiere evaluación y aprobación formal | Actualizar DB a nueva versión |
| **Emergencia** | Respuesta inmediata por riesgo crítico  | Parche urgente ante 0-day     |

---

## 7. Documentación y herramientas clave

### CMDB (Configuration Management Database)

Base de datos que almacena activos, configuraciones y relaciones.
Ejemplo: “Servidor Web A depende del Firewall B y la App C”.

### Sistemas de ticketing

Permiten registrar solicitudes, aprobaciones y evidencias:
ServiceNow, Jira, Remedy.

### Version Control

Control de versiones para código y configuraciones:
Git, SVN.

### Plantillas de Change Request

Incluyen:

* Descripción del cambio
* Análisis de riesgos y mitigaciones
* Plan de reversión
* Fecha de implementación
* Responsable

---

## 8. Buenas prácticas

* Usar un inventario centralizado de activos
* Mantener la CMDB actualizada
* No realizar cambios sin aprobación documentada
* Fomentar coordinación DevSecOps
* Realizar revisiones post-cambio
* Aplicar cambios con mínimo impacto y ser reversibles
