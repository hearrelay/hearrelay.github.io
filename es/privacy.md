---
title: Política de privacidad — HearRelay
lang: es
---

# Política de privacidad

**Fecha de entrada en vigor: 24 de abril de 2026**
**Última actualización: 24 de abril de 2026**

> Esta traducción se proporciona por conveniencia. En caso de discrepancia entre esta traducción y la [versión en inglés](/en/privacy/), prevalecerá la versión en inglés.

HearRelay (la «Aplicación») está diseñada para respetar la privacidad de forma predeterminada. Esta política explica qué datos se procesan, y cuáles no, cuando utiliza HearRelay.

Si tiene alguna pregunta, contáctenos en **hearrelay-privacy@conex-cp.com**.

---

## 1. Quiénes somos

HearRelay es desarrollada por **CONEX Corporation** (株式会社CONEX), una sociedad constituida en Japón (el «Desarrollador», «nosotros»). Dado que HearRelay no procesa datos personales en nuestros servidores, no actuamos como «responsable del tratamiento» en un sentido material — somos el editor de la aplicación. Para cualquier consulta, utilice las direcciones de correo electrónico que aparecen al final de esta página.

---

## 2. Datos que no recopilamos

**No** recopilamos, almacenamos, transmitimos a nuestros servidores ni compartimos ninguno de los siguientes datos:

- Audio captado por el micrófono de su dispositivo
- Grabaciones de audio que usted cree con la Aplicación
- Datos de contacto, ubicación, fotos, datos de cámara o identificadores de dispositivo
- Identificadores publicitarios (IDFA, IDFV utilizados para rastreo)
- Analíticas, telemetría de fallos enviada a servicios de terceros, ni perfiles de comportamiento

HearRelay no contiene SDK de terceros para analíticas, publicidad o rastreo.

---

## 3. Datos procesados localmente en su dispositivo

La Aplicación procesa los siguientes datos en su dispositivo, y **únicamente en su dispositivo**:

| Dato | Finalidad | Retención |
|---|---|---|
| Audio del micrófono (en vivo) | Monitoreo en tiempo real hacia auriculares o hacia un dispositivo emparejado en la misma red Wi-Fi | No se almacena |
| Grabaciones de audio (opcional) | Puede grabar sesiones manualmente | Se eliminan automáticamente después de 24 horas por defecto; puede extender o eliminar antes |
| Historial de conexión (nombre del par, última conexión) | Función de comodidad para reconectar rápidamente | Almacenado localmente; se elimina al desinstalar |
| Preferencias de la aplicación | Recordar sus configuraciones | Almacenadas localmente |

Cuando desinstala la Aplicación, todos los datos anteriores se eliminan con ella.

---

## 4. Datos tratados brevemente por la infraestructura de Apple

Para permitir que sus propios dispositivos Apple se descubran mutuamente en la misma red Wi-Fi, HearRelay utiliza **iCloud Key-Value Storage**, provisto por Apple, para publicar:

- Una **clave pública** criptográfica generada en su dispositivo
- Una **huella digital** (SHA-256) de esa clave
- El **nombre**, la **plataforma**, el **modelo** del dispositivo y la **versión de la aplicación**

Estos datos se almacenan dentro del ámbito de su propio Apple ID, dentro del servicio iCloud de Apple, y no son visibles para otros titulares de Apple ID ni para nosotros. El Desarrollador no opera ningún servidor y no tiene acceso a estos datos. El tratamiento por parte de Apple se rige por la política de privacidad de Apple.

---

## 5. Comunicación en red

HearRelay se comunica **únicamente** con otros dispositivos Apple que estén:

1. Iniciados con la **misma Apple ID**, **y**
2. Conectados a la **misma red Wi-Fi / red local**

La comunicación se cifra con **TLS 1.3**. HearRelay **no** envía datos a través de Internet a servidores remotos, ni admite el monitoreo remoto entre redes. El uso remoto está prohibido deliberadamente para prevenir la vigilancia encubierta.

---

## 6. Grabaciones que usted crea

Si activa la función de grabación:

- Las grabaciones se guardan **únicamente en el dispositivo que las creó**
- Se almacenan dentro del sandbox de la Aplicación con **cifrado a nivel de archivo** (`NSFileProtectionComplete`)
- Se **eliminan automáticamente 24 horas** después de su creación, salvo que decida explícitamente conservarlas
- Puede compartirlas o exportarlas mediante la hoja de compartir de iOS, bajo su control
- Las grabaciones nunca se suben a nosotros ni a terceros desde la Aplicación

---

## 7. Terceros

- **No** compartimos datos con terceros.
- **No** utilizamos SDK de publicidad, analíticas ni perfilado.
- **No** vendemos ni alquilamos datos de ningún tipo.

La distribución y el pago son gestionados por Apple a través del App Store según los términos de Apple. Cuando Apple procesa su compra o entrega actualizaciones, la política de privacidad de Apple se aplica a esa actividad.

---

## 8. Usuarios internacionales

Dado que HearRelay no transfiere datos fuera de sus dispositivos, no se realiza ninguna transferencia internacional de datos personales por nuestra parte.

---

## 9. Privacidad de los menores

HearRelay es una utilidad destinada a adultos, normalmente padres, madres o cuidadores. **No está dirigida a menores de 13 años** y no recopilamos conscientemente datos personales de menores. El procesamiento de la Aplicación es local en su dispositivo, por lo que no se recopilan, almacenan ni transmiten datos personales de menores.

---

## 10. Sus derechos

Dado que no conservamos datos personales sobre usted, normalmente no hay nada que acceder, corregir, eliminar, exportar o restringir. No obstante, según su ubicación (EEE, Reino Unido, California, Brasil, Japón, etc.), puede tener derechos legales, incluyendo:

- Derecho de acceso
- Derecho de rectificación
- Derecho de supresión
- Derecho a oponerse o restringir el tratamiento
- Derecho a la portabilidad de los datos
- Derecho a presentar una reclamación ante su autoridad de control local

Para ejercer cualquier derecho, contáctenos en **hearrelay-privacy@conex-cp.com**. Para eliminar todos los datos que la Aplicación ha almacenado localmente, basta con desinstalar la Aplicación de su dispositivo.

---

## 11. Seguridad

Utilizamos protecciones estándar de la industria:

- **TLS 1.3** para toda la comunicación entre dispositivos
- Claves **Curve25519 / P-256** generadas y almacenadas en el **Secure Enclave** cuando es posible
- **Fijación de clave pública** para evitar que dispositivos impostores se conecten
- **Protección de archivos** (`NSFileProtectionComplete`) para las grabaciones locales

Ningún método de transmisión o almacenamiento es perfectamente seguro. Para reportar una vulnerabilidad, consulte nuestra [página de seguridad](/es/security/) y envíe un correo a **hearrelay-security@conex-cp.com**.

---

## 12. Cambios a esta política

Podemos revisar esta política de privacidad. La fecha de revisión se actualizará en la parte superior de esta página, y los cambios importantes se anunciarán en las notas de versión de la Aplicación. Continuar usando la Aplicación después de la entrada en vigor de los cambios constituye la aceptación de los mismos.

---

## 13. Contacto

- Privacidad: **hearrelay-privacy@conex-cp.com**
- Soporte: **hearrelay-support@conex-cp.com**
- Seguridad: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.github.io/>

---

**English version:** [Privacy Policy](/en/privacy/)
