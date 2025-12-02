# 04 · Social Engineering

## 1. Concepto general

La Ingeniería Social es la manipulación psicológica utilizada para obtener información confidencial o forzar acciones que comprometan la seguridad.
Es una amenaza **no técnica**, extremadamente efectiva, que se apoya en emociones como **confianza, miedo, curiosidad o autoridad**.

---

## 2. Principales tipos de ataques de ingeniería social

| Tipo                          | Descripción                                            | Medio común          |
| ----------------------------- | ------------------------------------------------------ | -------------------- |
| **Phishing**                  | Correos falsos que imitan entidades legítimas          | Email                |
| **Spear Phishing**            | Ataques dirigidos a un individuo o grupo específico    | Email, LinkedIn      |
| **Whaling**                   | Phishing dirigido a altos ejecutivos                   | Email personalizado  |
| **Vishing**                   | Engaño mediante llamadas telefónicas                   | Voz                  |
| **Smishing**                  | Phishing mediante SMS o apps                           | Mensaje móvil        |
| **Pretexting**                | Se crea una identidad o historia falsa                 | Teléfono, presencial |
| **Baiting**                   | Uso de un objeto atractivo (USB, enlaces) para engañar | Físico o digital     |
| **Tailgating / Piggybacking** | Acceso físico siguiendo a un autorizado                | Físico               |
| **Quid Pro Quo**              | Solicitar información a cambio de un “beneficio”       | Email, llamada       |
| **Impersonation**             | Hacerse pasar por empleado/proveedor                   | Digital o presencial |
| **Dumpster Diving**           | Buscar documentos sensibles en basura                  | Físico               |
| **Watering Hole Attack**      | Comprometer sitios frecuentados por la víctima         | Navegación web       |

---

## 3. Técnicas psicológicas comunes

| Táctica                      | Descripción                          | Ejemplo                                        |
| ---------------------------- | ------------------------------------ | ---------------------------------------------- |
| **Autoridad**                | Simular ser una figura con poder     | “Soy de TI, dame tu contraseña.”               |
| **Urgencia**                 | Presión temporal intensa             | “Valida tu cuenta en 10 minutos.”              |
| **Escasez**                  | Oferta limitada para forzar decisión | “Última oportunidad para renovar.”             |
| **Familiaridad / Confianza** | Lenguaje cercano o personal          | “Coincidimos en la reunión pasada…”            |
| **Miedo / Amenaza**          | Consecuencias negativas              | “Tu cuenta será suspendida.”                   |
| **Reciprocidad**             | Ofrecer algo a cambio de información | “Recibe este obsequio si confirmas tus datos.” |
| **Curiosidad**               | Despertar interés natural            | “Fotos exclusivas del evento…”                 |

---

## 4. Indicadores de ataque de ingeniería social

* Solicitud de información sensible fuera de canales oficiales
* Correos con errores, urgencia o tono emocional
* URLs sospechosas o mal escritas (typosquatting)
* Enlaces acortados o adjuntos inesperados
* Desconocidos pidiendo acceso físico
* Visitas, llamadas o solicitudes inusuales sin verificación

---

## 5. Contramedidas y defensa

### A nivel técnico

* Filtros antiphishing y análisis de correo
* Implementar **SPF, DKIM y DMARC**
* Bloqueo de URLs sospechosas y macros
* Monitoreo en SIEM de dominios y accesos anómalos

### A nivel humano

* Formación continua y concienciación
* Simulaciones periódicas de phishing
* Política clara de verificación de identidad
* Cultura de reporte de actividad sospechosa

### A nivel físico

* Supervisión y acompañamiento de visitantes
* Destrucción segura de documentos
* Control de accesos y cámaras de seguridad

