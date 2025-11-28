# 02 · Threat Actors and Motivations

## 1. Tipos de Threat Actors

| Tipo                   | Descripción                                                                                              | Recursos / Capacidad                                               | Motivación                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------- |
| **Nation-State / APT** | Atacantes patrocinados por gobiernos. Usan malware avanzado, ataques prolongados y técnicas de evasión.  | Muy altos (financiación estatal, 0-days, infraestructura dedicada) | Espionaje, sabotaje, obtención de secretos militares o industriales |
| **Hacktivist**         | Actúan por razones políticas o ideológicas. Publican datos o modifican sitios para visibilizar su causa. | Medios                                                             | Activismo digital, protesta, exposición mediática                   |
| **Insider Threat**     | Personas con acceso legítimo que abusan de sus privilegios, intencional o accidentalmente.               | Acceso interno                                                     | Revancha, lucro personal, negligencia                               |
| **Organized Crime**    | Redes criminales organizadas orientadas al beneficio económico (RaaS, Phishing-as-a-Service).            | Altos                                                              | Ganancia financiera, extorsión, robo de datos                       |
| **Script Kiddie**      | Poca experiencia, usan herramientas de terceros.                                                         | Bajos                                                              | Curiosidad, notoriedad, diversión                                   |
| **Shadow IT**          | Uso de servicios no autorizados por TI (SaaS no controlado).                                             | Variable                                                           | Aumentar productividad sin respetar controles                       |

---

## 2. Atributos del atacante

### Interno vs Externo

* **Interno**: empleado, proveedor o socio con acceso legítimo
* **Externo**: atacante sin acceso autorizado

Otros factores clave:

* **Recursos y financiación**: determinan el alcance del ataque
* **Nivel de sofisticación**: herramientas propias vs software público
* **Capacidad de persistencia**: duración y continuidad del ataque

---

## 3. Motivaciones más comunes

* **Financieras**: robo de datos, fraude, ransomware
* **Espionaje**: obtención de información estratégica
* **Disrupción**: sabotaje y desestabilización
* **Ideológicas / Políticas**: protestas digitales
* **Venganza / Descontento**: empleados resentidos
* **Prestigio / Diversión**: reconocimiento social o curiosidad

---

## 4. Técnicas y comportamientos típicos

| Técnica                       | Descripción                                                                                  | Asociada a                                   |
| ----------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------- |
| **Phishing / Spear Phishing** | Correos fraudulentos para robar credenciales o instalar malware. Spear phishing es dirigido. | Todos, especialmente APT y crimen organizado |
| **Credential Dumping**        | Robo de contraseñas almacenadas (ej. Mimikatz).                                              | APT, insiders, crimen organizado             |
| **Living off the Land (LoL)** | Uso de herramientas legítimas del sistema (PowerShell, WMI).                                 | APT, insiders                                |
| **Command and Control (C2)**  | Comunicación con servidor atacante para control remoto.                                      | APT, botnets                                 |
| **Zero-Day Exploits**         | Explotación de vulnerabilidades desconocidas.                                                | APT, nation-state                            |
| **Social Engineering**        | Manipulación psicológica (pretexting, baiting, tailgating).                                  | Todos                                        |
| **Lateral Movement**          | Movimiento dentro de la red tras compromiso inicial.                                         | APT, crimen organizado                       |
| **Data Exfiltration**         | Robo sigiloso de datos.                                                                      | APT, crimen organizado                       |
| **Persistencia**              | Creación de accesos ocultos o tareas automáticas.                                            | APT, insiders                                |

---

## 5. Mitigaciones clave

* Segmentación de red y control de accesos
* Autenticación multifactor (**MFA**)
* Detección de comportamiento anómalo (SIEM, UEBA)
* Principio de menor privilegio
* Concienciación y formación continua
* Monitorización de cuentas privilegiadas
* Auditoría y revisión de logs
