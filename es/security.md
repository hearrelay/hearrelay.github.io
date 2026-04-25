---
title: Seguridad — HearRelay
lang: es
---

> Esta versión en español se proporciona por conveniencia. En caso de divergencia o discrepancia entre esta versión y la versión en inglés, la versión en inglés prevalecerá en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos.

# Seguridad

**Versión del documento: v3.2026-04-26**

Gracias por ayudarnos a mantener seguros a los usuarios de HearRelay. Esta página explica cómo reportar vulnerabilidades y resume la postura de seguridad de HearRelay.

---

## Reporte de vulnerabilidades

Envíe un correo a **hearrelay-security@conex-cp.com** con la siguiente información:

- Una descripción clara del problema
- Pasos para reproducir (o prueba de concepto)
- La versión de HearRelay y la versión de iOS / iPadOS utilizadas
- Cualquier mitigación sugerida que tenga en mente
- Si desea recibir crédito público

Preferimos el correo para el reporte inicial. Si es necesario, podemos habilitar un **GitHub Security Advisory (Divulgación Privada)** para coordinar el seguimiento.

**No publique** los detalles de una vulnerabilidad antes de que hayamos tenido la oportunidad de responder y publicar una corrección.

---

## Refugio seguro para investigación de seguridad de buena fe

Actualmente no ofrecemos un programa de recompensas por errores ni recompensas monetarias.

Al probar o reportar vulnerabilidades, le pedimos que:

- **No** acceda, modifique, elimine ni extraiga datos que no le pertenezcan.
- **No** realice pruebas de denegación de servicio, spam, phishing, ataques de ingeniería social ni ningún ataque físico.
- **No** pruebe contra los servicios de Apple, hardware de terceros ni ningún sistema que no sea de su propiedad.
- Limite las pruebas a sus propios dispositivos y a su propia Apple ID.

Si presenta un reporte de buena fe dentro del alcance de esta política y cumple con estas reglas, **CONEX no emprenderá intencionalmente acciones legales en su contra basadas únicamente en dicho reporte**, sujeto a la ley aplicable.

**Limitaciones importantes.** Esta política **no** autoriza el acceso a ningún sistema, servicio, cuenta, dispositivo o dato sin permiso. **No** renuncia ni limita ninguna ley penal, autoridad regulatoria ni derechos de terceros. **No** vincula a Apple, GitHub, proveedores de correo, proveedores en la nube, fuerzas del orden, fiscales, reguladores ni a ningún otro tercero.

Podremos adoptar las acciones que correspondan — incluyendo notificar a las partes afectadas o a las autoridades — en casos que involucren extorsión, amenazas, explotación activa, daño a usuarios, acceso no autorizado a sistemas de terceros o **incumplimiento sustancial de esta política tras una notificación, cuando el problema pueda corregirse razonablemente**.

---

## Qué consideramos dentro del alcance

Entran en el alcance de los reportes:

- La aplicación HearRelay para iOS / iPadOS
- El handshake del HearRelay Secure Channel (X25519 ECDH + P-256 ECDSA + ChaCha20-Poly1305 AEAD)
- El proceso de descubrimiento de pares basado en iCloud Key-Value Storage
- La gestión local de archivos (almacenamiento de grabaciones y borrado automático)
- El sitio web del proyecto en `hearrelay.app`

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

1. **Minimización de datos** — el audio y las grabaciones nunca salen de su dispositivo; no hay SDK de analítica ni publicidad.
2. **Solo red local** — los dispositivos emparejados se comunican exclusivamente por la misma Wi-Fi / red local, nunca por Internet.
3. **Identidad criptográfica del par** — los dispositivos se identifican mutuamente con claves de firma **P-256** (almacenadas en el **Secure Enclave** cuando esté disponible, con respaldo en Keychain), y se descubren mediante iCloud Key-Value Storage con el alcance de su Apple ID.

### Visión general del flujo de datos

```text
[Micrófono del dispositivo A]
         |
         | solo procesamiento local
         v
[App del dispositivo A] <─── canal cifrado P2P en la misma Wi-Fi ───> [App del dispositivo B]
         |
         | solo metadatos de descubrimiento de dispositivos (clave pública, huella,
         | nombre del dispositivo, plataforma/modelo, versión de la app, fechas de la clave)
         v
[Almacenamiento clave-valor de Apple iCloud, ámbito del Apple ID]

[Apple App Store + Compras Integradas]   ─── Apple procesa los pagos
[Servidor de CONEX]                      ─── ninguno
[SDK de terceros de análisis / publicidad / seguimiento]   ─── ninguno
```

CONEX no opera ningún servidor y no tiene acceso operativo a los datos almacenados en Apple iCloud ni procesados por Apple IAP. Los únicos datos que CONEX recibe directamente son los que los usuarios envían voluntariamente por correo electrónico (consulte la [Política de privacidad §4](/es/privacy/)).

El transporte utiliza el **HearRelay Secure Channel**: X25519 ECDH para el acuerdo de claves con secreto hacia adelante, ChaCha20-Poly1305 AEAD con protección contra repetición y nonces derivados de un contador por trama.

Puede rotar la clave de identidad de su dispositivo, olvidar un dispositivo par o borrar todo el estado de seguridad del dispositivo en cualquier momento desde **Ajustes → Seguridad** dentro de la Aplicación.

Para una descripción interna más completa, consulte la documentación de diseño del proyecto.

---

## Contacto

- Reportes de seguridad: **hearrelay-security@conex-cp.com**
- Contacto general: **hearrelay-support@conex-cp.com**

---

**Las traducciones están disponibles en:** [日本語](/ja/security/) · [Français](/fr/security/) · [Español](/es/security/) · [Português (Brasil)](/pt-BR/security/) · [简体中文](/zh-Hans/security/)

Cuando esta página se proporcione en cualquier idioma distinto al inglés, la **versión en inglés prevalecerá** en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos de su país o región.
