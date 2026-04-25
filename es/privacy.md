---
title: Política de privacidad — HearRelay
lang: es
---

> Esta versión en español se proporciona por conveniencia. En caso de divergencia o discrepancia entre esta versión y la versión en inglés, la versión en inglés prevalecerá en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos.

# Política de privacidad

**Fecha de entrada en vigor: 2026-04-25**
**Última actualización: 2026-04-25**

HearRelay (la «Aplicación») está diseñada para ser privada de forma predeterminada. Esta política explica qué datos se procesan, y cuáles no, cuando usted utiliza HearRelay.

Si tiene alguna pregunta, contáctenos en **hearrelay-privacy@conex-cp.com**.

---

## 1. Quiénes somos

HearRelay es desarrollada por **CONEX Corporation** (株式会社CONEX), una sociedad constituida en Japón (el «Desarrollador», «nosotros», «nos», «CONEX»). La Aplicación está diseñada de manera que el audio, las grabaciones, la información de pago, los identificadores publicitarios, los datos de analítica y los datos de rastreo no se transmiten a servidores de CONEX. CONEX no opera ningún servidor backend para la Aplicación.

En la medida en que cierta información limitada de descubrimiento de dispositivos sea procesada por Apple dentro de su cuenta de Apple ID (véase §4), CONEX no accede a ese tratamiento ni lo opera. Cuando la legislación aplicable considere que dicha información constituye «datos personales», CONEX coopera de buena fe con las solicitudes de información conforme a la §10.

Para correspondencia, utilice las direcciones de correo electrónico que aparecen al final de esta página.

---

## 2. Datos que no recopilamos

CONEX **no** recopila ni recibe en sus propios servidores, ni almacena, ni comparte ninguno de los siguientes:

- Audio captado por el micrófono de su dispositivo
- Grabaciones de audio que usted cree con la Aplicación
- Información de contacto, ubicación, fotos, datos de cámara o identificadores de dispositivo
- Identificadores publicitarios (IDFA, IDFV utilizados para rastreo)
- Analíticas, telemetría de fallos enviada a servicios de terceros, ni perfiles de comportamiento
- Datos de tarjetas de pago o de facturación (Apple procesa las compras — véase §7)

HearRelay no contiene ningún SDK de terceros para analíticas, publicidad o rastreo.

---

## 3. Datos procesados localmente en su dispositivo

La Aplicación procesa los siguientes datos en su dispositivo, y **únicamente en su dispositivo**:

| Dato | Finalidad | Retención |
|---|---|---|
| Audio del micrófono (en vivo) | Monitoreo en tiempo real hacia auriculares o hacia un dispositivo emparejado en la misma red Wi-Fi | No se almacena |
| Grabaciones de audio (opcional) | Puede grabar sesiones manualmente | Se eliminan automáticamente después de 24 horas por defecto; puede extender o eliminar antes |
| Historial de conexión (nombre del par, hora de la última conexión) | Función de comodidad para reconectar rápidamente | Almacenado localmente; se borra al desinstalar la Aplicación |
| Preferencias de la Aplicación (incluyendo la fecha de inicio del periodo de prueba para el control de compras) | Recordar sus configuraciones | Almacenadas localmente |

Cuando usted desinstala la Aplicación, todos los datos anteriores se eliminan con ella.

---

## 4. Información limitada procesada por Apple iCloud (ámbito de Apple ID)

Para permitir que sus propios dispositivos Apple se descubran mutuamente en la misma red Wi-Fi, la Aplicación hace que la siguiente información limitada de descubrimiento de dispositivos se almacene en **Apple iCloud Key-Value Storage** dentro de su cuenta de Apple ID:

- Una **clave pública** criptográfica generada en su dispositivo
- Una **huella digital SHA-256** de esa clave pública
- El **nombre** de su dispositivo (tal como está configurado en Ajustes de iOS → General → Información → Nombre)
- La **plataforma**, el **modelo** de su dispositivo y la **versión** de la aplicación instalada
- La **fecha de creación** y la **fecha de la última rotación** de la clave

Esta información se almacena dentro del ámbito de su propio Apple ID, dentro del servicio iCloud de Apple, y no es visible para otros titulares de Apple ID ni para CONEX. CONEX no opera Apple iCloud y no accede a esta información en sus propios servidores. El tratamiento por parte de Apple se rige por la propia política de privacidad de Apple y por los términos de iCloud.

**Dependiendo de la legislación aplicable y de la configuración del nombre de su dispositivo, parte de esta información puede ser considerada como datos personales** — por ejemplo, si el nombre de su dispositivo contiene su nombre completo. La describimos aquí por transparencia. Puede cambiar el nombre de su dispositivo en cualquier momento en los Ajustes de iOS, y puede purgar la identidad de la Aplicación (rotando su clave y borrando la entrada) desde **Ajustes → Seguridad → Restablecer toda la seguridad del dispositivo** dentro de la Aplicación.

---

## 5. Comunicación en red

HearRelay se comunica **únicamente** con otros dispositivos Apple que estén:

1. Iniciados con la misma Apple ID, **y**
2. Conectados a la misma red Wi-Fi / red local

La comunicación se cifra con el **HearRelay Secure Channel** (acuerdo de claves X25519 ECDH + ChaCha20-Poly1305 AEAD con protección contra repetición). HearRelay **no** envía datos a través de Internet a servidores remotos, ni admite el monitoreo remoto entre redes. El uso remoto está prohibido deliberadamente para prevenir la vigilancia encubierta.

---

## 6. Grabaciones de audio que usted crea

Si activa la función de grabación:

- Las grabaciones se guardan **únicamente en el dispositivo que las creó**
- Se almacenan dentro del sandbox de la Aplicación con **cifrado a nivel de archivo** (`NSFileProtectionComplete`)
- Se **eliminan automáticamente 24 horas** después de su creación, salvo que decida explícitamente conservarlas
- Puede compartirlas o exportarlas mediante la hoja de compartir de iOS, bajo su control
- La Aplicación nunca sube las grabaciones a CONEX ni a ningún tercero

Usted es responsable de confirmar que cualquier grabación o monitoreo en vivo que realice cumple con todas las leyes aplicables — incluyendo los requisitos de consentimiento que puedan aplicarse en su lugar. Consulte nuestras [Condiciones de uso](/es/terms/) y [Soporte](/es/support/) para más información.

---

## 7. Terceros, pagos y la App Store

- CONEX **no** comparte datos con ningún tercero.
- La Aplicación **no** utiliza SDK de publicidad, analíticas ni perfilado.
- CONEX **no** vende ni alquila datos de ningún tipo.

La distribución y los pagos son gestionados por Apple a través de la App Store y de las Compras Integradas. **HearRelay Full Access es una compra única, no consumible, no una suscripción de renovación automática.** Los precios, impuestos, reembolsos y la facturación son procesados por Apple bajo los términos de la App Store y de Apple Media Services. CONEX no recibe números de tarjetas de pago ni datos de facturación. Puede restaurar una compra anterior utilizando la opción **Restore Purchases** dentro de la Aplicación.

Cuando Apple procesa su compra o entrega actualizaciones, la propia política de privacidad de Apple se aplica a esa actividad. Cualquier información de diagnóstico que Apple recopile de su dispositivo (por ejemplo, los registros de fallos enviados mediante «Compartir con desarrolladores de la app») se rige por sus Ajustes de iOS y por los términos para desarrolladores de Apple.

---

## 8. Nuestro sitio web

El sitio web de HearRelay en <https://hearrelay.app/> es un sitio informativo estático alojado en GitHub Pages. **No** utilizamos cookies publicitarias, cookies de analítica, píxeles de rastreo, ni etiquetas de marketing de terceros. Si esto cambia, actualizaremos esta Política y proporcionaremos los avisos u opciones que requiera la legislación aplicable.

---

## 9. Usuarios internacionales

Dado que HearRelay no transfiere datos fuera de sus dispositivos hacia servidores de CONEX, no hay ninguna transferencia internacional de datos personales realizada por CONEX.

### 9.1 Usuarios en el Espacio Económico Europeo (EEE), Reino Unido, Suiza

La Aplicación está diseñada de modo que CONEX no recopila ni recibe en sus propios servidores audio, grabaciones, información de pago, datos de analítica, identificadores publicitarios ni datos de rastreo.

Cierta información limitada de descubrimiento de dispositivos puede almacenarse en Apple iCloud dentro de su cuenta de Apple ID (§4). CONEX no opera Apple iCloud y no accede a esta información en sus propios servidores. Cuando la legislación aplicable considere que esta información constituye datos personales, las **finalidades** de cualquier tratamiento se limitan a permitir el descubrimiento de dispositivos, la autenticación mutua, la seguridad y la comunicación local entre pares de sus propios dispositivos; la **base jurídica** es su consentimiento para utilizar la Aplicación con esa finalidad, y su interés legítimo en conectar de forma privada sus propios dispositivos.

CONEX ha evaluado el requisito establecido en el Artículo 27 del GDPR de designar a un representante en la UE y ha concluido que la naturaleza limitada, ocasional y de bajo riesgo de cualquier tratamiento queda comprendida en la exención del Artículo 27(2)(a). Esta determinación se documenta internamente y se revisa cuando cambian los hechos materiales. Si usted es una autoridad de control o un interesado en el EEE que necesita comunicarse con nosotros, utilice **hearrelay-privacy@conex-cp.com** — nos comprometemos a responder dentro de los plazos legales.

### 9.2 Usuarios en Brasil

La postura de tratamiento de la Aplicación bajo la LGPD coincide con la §9.1. CONEX no tiene constancia de que se traten datos personales en sus propios servidores. CONEX no ha designado un Encarregado (DPO) local sobre la base de que no se realiza tratamiento de datos personales a gran escala o de alto riesgo a través de CONEX. El contacto indicado anteriormente sirve como punto de contacto para las solicitudes bajo la LGPD.

### 9.3 Usuarios en Japón

CONEX no incluye en la Aplicación SDK de terceros para publicidad, analíticas o rastreo, y no transmite información relacionada con el usuario a sus propios servidores. Apple iCloud Key-Value Storage se utiliza únicamente para sincronizar la información limitada de descubrimiento de dispositivos descrita en la §4 dentro de su propia cuenta de Apple ID; CONEX no recibe esta información en sus propios servidores. Nos referimos a esta configuración de buena fe al evaluar el régimen japonés de notificación de transmisiones externas establecido en la Ley de Empresas de Telecomunicaciones.

### 9.4 Usuarios en Hong Kong / Taiwán

Se aplica la misma postura de tratamiento. CONEX es consciente de que la PDPO (Hong Kong) y la Personal Information Protection Act (Taiwán) definen los datos personales y la información personal de manera amplia; consulte las §4 y §10 para conocer nuestra posición y los derechos que puede ejercer.

---

## 10. Privacidad de los menores

HearRelay es una utilidad destinada a personas adultas, normalmente padres, madres o cuidadores. **No está dirigida a menores de 13 años**, y CONEX no recopila conscientemente datos personales de menores. El tratamiento que realiza la Aplicación es local en su dispositivo, por lo que no se recopilan, almacenan ni transmiten a CONEX datos personales de menores.

---

## 11. Sus derechos

Dado que CONEX no conserva datos personales sobre usted en sus servidores, normalmente no hay nada que podamos acceder, corregir, eliminar, exportar ni restringir. No obstante, según su ubicación (EEE, Reino Unido, California, Brasil, Japón, Hong Kong, Taiwán, etc.), puede tener derechos legales, incluyendo:

- Derecho de acceso
- Derecho de rectificación
- Derecho de supresión
- Derecho a oponerse o restringir el tratamiento
- Derecho a la portabilidad de los datos
- Derecho a optar por no participar en la «venta» o el «intercambio» — CONEX no vende ni comparte datos personales
- Derecho a presentar una reclamación ante su autoridad de control local

Para ejercer cualquier derecho, contáctenos en **hearrelay-privacy@conex-cp.com**. Tenga en cuenta que para eliminar todos los datos que la Aplicación ha almacenado localmente, basta con desinstalar la Aplicación de su dispositivo. Para purgar la identidad de la Aplicación específica del dispositivo desde Apple iCloud (§4), utilice **Ajustes → Seguridad → Restablecer toda la seguridad del dispositivo** dentro de la Aplicación.

---

## 12. Seguridad

Utilizamos protecciones estándar de la industria:

- **HearRelay Secure Channel** (X25519 ECDH + ChaCha20-Poly1305 AEAD) para toda la comunicación entre dispositivos
- Claves de identidad **P-256** generadas y almacenadas en el **Secure Enclave** cuando esté disponible, con respaldo en Keychain
- **Fijación de clave pública** mediante una lista de confianza con alcance de iCloud para evitar que dispositivos impostores se conecten
- **Protección de archivos** (`NSFileProtectionComplete`) para las grabaciones locales

Ningún método de transmisión o almacenamiento es perfectamente seguro. Para reportar una vulnerabilidad, consulte nuestra [página de Seguridad](/es/security/) y envíe un correo a **hearrelay-security@conex-cp.com**.

---

## 13. Cambios a esta política

Podemos revisar esta Política de privacidad. La fecha de revisión se actualizará en la parte superior de esta página, y los cambios materiales se anunciarán en las notas de versión de la Aplicación. Cuando la legislación aplicable lo requiera, obtendremos su consentimiento o le proporcionaremos un aviso previo razonable y una oportunidad significativa de dejar de usar la Aplicación antes de que el cambio entre en vigor.

---

## 14. Contacto

- Privacidad: **hearrelay-privacy@conex-cp.com**
- Soporte: **hearrelay-support@conex-cp.com**
- Seguridad: **hearrelay-security@conex-cp.com**
- Web: <https://hearrelay.app/>

---

**Las traducciones están disponibles en:** [日本語](/ja/privacy/) · [Français](/fr/privacy/) · [Español](/es/privacy/) · [Português (Brasil)](/pt-BR/privacy/) · [简体中文](/zh-Hans/privacy/)

Cuando esta Política se proporcione en cualquier idioma distinto al inglés, la **versión en inglés prevalecerá** en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos de su país o región.
