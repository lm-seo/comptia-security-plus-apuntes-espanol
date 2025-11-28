# 01 · Fundamentals of Security

## 1. Conceptos básicos

### Information Security

Protección de datos frente a:

* Acceso no autorizado
* Modificación
* Destrucción

### Information Systems Security

Protección de los sistemas que procesan la información:

* Hardware
* Software
* Redes

---

## 2. CIA Triad

* **Confidentiality**
  Solo acceso autorizado.
  Ejemplos: cifrado, control de accesos.

* **Integrity**
  Datos exactos y sin alteraciones.
  Ejemplos: hashing, checksums.

* **Availability**
  Acceso cuando se necesita.
  Ejemplos: redundancia, backups.

### CIANA Pentagon

Extiende la CIA añadiendo:

* **Non-repudiation**: evita la negación de acciones (firmas digitales).
* **Authentication**: verificación de identidad.

### AAA Framework

* **Authentication**
* **Authorization**
* **Accounting**

---

## 3. Tipos de Controles de Seguridad

### Por categoría

* **Técnicos**
  Hardware y software (firewalls, cifrado).

* **Administrativos**
  Políticas, gobernanza, gestión.

* **Operacionales**
  Procedimientos y formación.

* **Físicos**
  Medidas tangibles (cerraduras, cámaras).

### Por función

* **Preventive**: previene incidentes.
* **Deterrent**: disuade ataques.
* **Detective**: detecta eventos.
* **Corrective**: restaura sistemas.
* **Compensating**: reemplazo temporal.
* **Directive**: establece normas y políticas.

---

## 4. Modelos y Procesos Clave

### Zero Trust Model

Nadie es fiable por defecto. Todo acceso debe ser verificado.

### Planes de control

* **Control Plane**
  Gestiona identidades, políticas y zonas seguras.

* **Data Plane**
  Aplica las políticas mediante puntos de control (PEP).

---

## 5. Gap Analysis

Evaluación de brechas entre:

* Estado actual
* Estado deseado

Tipos:

* Técnico
* De negocio

Resultado:

* **POA&M (Plan of Action and Milestones)**

---

## 6. Principios Fundamentales

### Confidentiality

Protección contra accesos no autorizados.
Ejemplos:

* Cifrado
* Control de accesos
* Data masking

### Integrity

Garantiza precisión y consistencia.
Ejemplos:

* Hashing
* Firmas digitales
* Auditorías

### Availability

Garantiza acceso continuo.
Ejemplos:

* Redundancia de servidores
* Energía de respaldo
* Alta disponibilidad

---

## 7. Factores de Autenticación

* Algo que sabes → contraseña
* Algo que tienes → token, tarjeta
* Algo que eres → biometría
* Algo que haces → patrón o gesto
* Donde estás → ubicación

### MFA (Multi-Factor Authentication)

Uso de dos o más factores combinados.

### Authorization

Definición de permisos tras la autenticación.

### Accounting

Registro y auditoría de actividades.
Herramientas:

* Syslog
* SIEM
