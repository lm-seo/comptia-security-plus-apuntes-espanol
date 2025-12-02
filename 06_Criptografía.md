# 06 · Cryptography

## 1. Concepto general

La criptografía protege la información mediante técnicas matemáticas que garantizan distintas propiedades de seguridad.

### Propiedades fundamentales

| Propiedad            | Qué asegura                                       | Ejemplo                  |
| -------------------- | ------------------------------------------------- | ------------------------ |
| **Confidencialidad** | Solo usuarios autorizados pueden leer los datos   | Cifrar un correo con AES |
| **Integridad**       | Los datos no fueron alterados                     | Hash SHA-256             |
| **Autenticación**    | Verifica la identidad del emisor                  | Certificados digitales   |
| **No repudio**       | El emisor no puede negar haber enviado el mensaje | Firma digital            |

---

## 2. Componentes básicos

| Concepto        | Explicación sencilla      | Ejemplo           |
| --------------- | ------------------------- | ----------------- |
| **Plaintext**   | Texto original sin cifrar | `"Contraseña123"` |
| **Ciphertext**  | Texto cifrado ilegible    | `"X9t@#D21Gk"`    |
| **Key (clave)** | Valor que cifra/descifra  | “Llave secreta”   |
| **Algorithm**   | Fórmula usada para cifrar | AES, RSA, SHA-256 |

---

## 3. Tipos de cifrado

| Tipo           | Características                                                               | Ejemplo / Analogía                                                  |
| -------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| **Simétrico**  | Una sola clave para cifrar y descifrar. Muy rápido.                           | Como una llave de casa. Ej: AES, DES, 3DES, Blowfish                |
| **Asimétrico** | Par de claves: pública (cifrar) y privada (descifrar). Más seguro, más lento. | Como un buzón: cualquiera envía, solo tú abres. Ej: RSA, ECC, ECDSA |

---

## 4. Aplicaciones comunes

| Uso                          | Solución criptográfica          | Ejemplo práctico               |
| ---------------------------- | ------------------------------- | ------------------------------ |
| Protección de datos en disco | AES-256                         | BitLocker, VeraCrypt           |
| Correo electrónico seguro    | PGP, S/MIME                     | Firmar/cifrar emails           |
| Transmisión segura           | TLS/HTTPS                       | Navegación segura              |
| Autenticación digital        | Certificados y firmas digitales | Certificado SSL de un servidor |
| Integridad de archivos       | Hashing (SHA, MD5)              | Verificar descargas            |

---

## 5. Hashing (para integridad)

El **hashing** es una función unidireccional que transforma datos en un valor único e irrepetible.
No puede revertirse.
Un cambio de un solo bit altera completamente el hash.

| Algoritmo             | Longitud       | Uso                    |
| --------------------- | -------------- | ---------------------- |
| **MD5**               | 128 bits       | Obsoleto, inseguro     |
| **SHA-1**             | 160 bits       | Deprecado              |
| **SHA-256 / SHA-512** | 256 / 512 bits | Estándar seguro actual |

### Ejemplo

```
Archivo: hello.txt
Hash SHA-256: 2CF24DBA5...
```

Cambiando una letra → el hash resultante será totalmente diferente.

---

## 6. PKI – Public Key Infrastructure

La PKI gestiona claves, identidades y certificados digitales para comunicaciones seguras.

| Elemento                        | Función                                       |
| ------------------------------- | --------------------------------------------- |
| **CA (Certificate Authority)**  | Emite certificados digitales                  |
| **RA (Registration Authority)** | Verifica identidad previa a la emisión        |
| **Certificate**                 | Contiene clave pública + info del propietario |
| **CRL / OCSP**                  | Revocación de certificados comprometidos      |

### Ejemplo práctico

Cuando visitas un sitio web con **🔒 HTTPS**, el navegador valida su certificado emitido por una CA confiable.

---

## 7. Otras técnicas y herramientas

| Concepto                           | Explicación                                       | Ejemplo                               |
| ---------------------------------- | ------------------------------------------------- | ------------------------------------- |
| **Key Escrow**                     | Copia de claves guardada por terceros autorizados | Recuperar datos si se pierde la clave |
| **TPM (Trusted Platform Module)**  | Chip para almacenar claves y cifrar hardware      | Portátiles empresariales              |
| **HSM (Hardware Security Module)** | Dispositivo dedicado a custodiar claves           | Bancos, centros de datos              |
| **Steganografía**                  | Ocultar datos dentro de otros archivos            | Mensaje oculto en una imagen          |
| **Tokenización / Data Masking**    | Reemplaza datos reales por tokens                 | Enmascarar tarjetas de crédito        |

