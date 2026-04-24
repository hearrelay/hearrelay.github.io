---
title: Seguridad — HearRelay
lang: es
---

# Seguridad

Gracias por ayudarnos a mantener seguros a los usuarios de HearRelay. Esta página explica cómo reportar vulnerabilidades y resume la postura de seguridad de HearRelay.

> Esta traducción se proporciona por conveniencia. En caso de discrepancia con la [versión en inglés](/en/security/), prevalecerá la versión en inglés.

---

## Reporte de vulnerabilidades

Envíe un correo a **hearrelay-security@conex-cp.com** con la siguiente información:

- Una descripción clara del problema
- Pasos para reproducir (o prueba de concepto)
- La versión de HearRelay y la versión de iOS / iPadOS utilizadas
- Cualquier mitigación sugerida que tenga en mente
- Si desea recibir crédito público

Preferimos el correo para el reporte inicial. Si es necesario, podemos habilitar un **GitHub Security Advisory (divulgación privada)** para coordinar el seguimiento.

**No publique** los detalles de una vulnerabilidad antes de que hayamos tenido la oportunidad de responder y publicar una corrección.

---

## Qué consideramos dentro del alcance

Entran en el alcance de los reportes:

- La aplicación HearRelay para iOS / iPadOS
- El handshake criptográfico y el transporte TLS utilizado entre dispositivos emparejados
- El proceso de descubrimiento de pares basado en iCloud Key-Value Storage
- La gestión local de archivos (almacenamiento de grabaciones y borrado automático)
- El sitio web del proyecto en `hearrelay.github.io`

---

## Fuera del alcance

- Vulnerabilidades en los sistemas operativos, frameworks o infraestructura de iCloud de Apple — repórtelas directamente a Apple
- Vulnerabilidades en routers Wi-Fi, auriculares Bluetooth u otro hardware de terceros
- Ataques de ingeniería social contra el desarrollador u otros usuarios
- Falta de cabeceras de seguridad en GitHub Pages más allá de lo que la plataforma nos permite configurar
- Problemas que requieren un dispositivo con jailbreak o que esté comprometido de algún modo

---

## Objetivos de respuesta

| Gravedad | Primera respuesta | Resolución objetivo |
|---|---|---|
| Crítica | en 24 horas | en 7 días |
| Alta | en 3 días | en 30 días |
| Media / Baja | en 7 días | en la próxima versión regular |

Son objetivos, no garantías.

---

## Divulgación coordinada

- Le mantendremos informado mientras investigamos.
- Acordaremos juntos una fecha de divulgación pública, normalmente cuando se publique una corrección.
- Al lanzarla, publicaremos un aviso de seguridad y (con su permiso) le daremos crédito.

---

## Resumen de la postura de seguridad

HearRelay está diseñada en torno a tres principios:

1. **Minimización de datos** — ningún audio ni grabación sale de su dispositivo; no hay SDK de analítica ni publicidad.
2. **Solo red local** — los dispositivos emparejados se comunican exclusivamente por la misma Wi-Fi / red local, nunca por Internet.
3. **Identidad criptográfica del par** — los dispositivos se identifican mutuamente con claves **Curve25519 / P-256**, protegidas en el **Secure Enclave** cuando es posible, y se descubren mediante iCloud Key-Value Storage con el alcance de su Apple ID.

El transporte se cifra con **TLS 1.3** utilizando solo las suites AEAD proporcionadas por iOS.

Para una descripción interna más completa, consulte la documentación de diseño del proyecto.

---

## Contacto

- Reportes de seguridad: **hearrelay-security@conex-cp.com**
- Contacto general: **hearrelay-support@conex-cp.com**

---

**English version:** [Security](/en/security/)
