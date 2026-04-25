---
title: Soporte — HearRelay
lang: es
---

> Esta versión en español se proporciona por conveniencia. En caso de divergencia o discrepancia entre esta versión y la versión en inglés, la versión en inglés prevalecerá en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos.

# Soporte

**Versión del documento: v3.2026-04-26**

Gracias por usar **HearRelay**. Esta página reúne consejos de resolución de problemas, avisos importantes sobre el uso lícito y cómo contactarnos.

---

## Avisos importantes

### Las leyes de grabación y monitoreo varían según el lugar

Las leyes sobre grabación y monitoreo en vivo varían según el país, estado, provincia y lugar de uso. Algunos lugares exigen el consentimiento de **todas** las partes antes de grabar. El monitoreo en lugares de trabajo, escuelas, alojamientos en alquiler, ámbitos médicos, cuidado de personas mayores, cuidado infantil y espacios públicos puede requerir avisos especiales, consentimiento por escrito o autorización. **No grabe conversaciones ni espacios privados a menos que tenga permitido legalmente hacerlo.** En caso de duda, no grabe.

Usted es responsable de confirmar que cualquier grabación o monitoreo en vivo que realice con HearRelay cumple con toda la ley aplicable. Consulte la [Sección 3 de las Condiciones de uso](/es/terms/) para conocer la lista de usos prohibidos.

### HearRelay no es un dispositivo de seguridad, médico ni de emergencia

HearRelay es una utilidad de consumo para monitoreo de conveniencia. **No** es un dispositivo médico, un dispositivo de emergencia, una alarma de seguridad, un dispositivo de seguridad para el cuidado infantil, un dispositivo de seguridad para el cuidado de personas mayores, un dispositivo de soporte vital, ni ningún equipo certificado para uso crítico de seguridad. **Nunca utilice HearRelay como único medio de supervisión o detección de emergencias.** Combínelo siempre con una supervisión directa responsable y con cualquier equipo de seguridad certificado para tal fin.

### Por qué HearRelay no funciona a través de Internet

HearRelay exige deliberadamente que ambos dispositivos estén **iniciados en la misma Apple ID** *y* **conectados a la misma red Wi-Fi / red local**. No existe una opción de retransmisión por Internet, ni un modo de monitoreo remoto, ni una ruta «en la nube». Se trata de una decisión de seguridad y privacidad, no de una funcionalidad faltante:

- Evita la vigilancia remota encubierta — un iPhone robado o prestado no puede transmitir audio fuera de la casa de alguien.
- Mantiene el audio fuera de los servidores de CONEX (no operamos ninguno) y fuera de la Internet pública.
- Limita el impacto de una vulneración de Apple ID a los dispositivos ya emparejados con esa Apple ID.

Si necesita monitoreo entre redes, HearRelay no es la herramienta adecuada — utilice un producto certificado para ese fin, con el aviso parental, laboral u otro aviso legal correspondiente.

---

## Ayuda rápida

### «No se han encontrado dispositivos» al intentar emparejar

Ambos dispositivos deben:

1. Tener iniciada sesión con **la misma Apple ID**
2. Estar conectados a la **misma red Wi-Fi** (misma subred)
3. Tener **iCloud** activado en los Ajustes de iOS
4. Haber concedido a HearRelay los permisos de **Micrófono** y **Red local**

Si aún no ve el otro dispositivo, pulse el botón de actualizar en el selector de emparejamiento, o reinicie la Aplicación en ambos dispositivos.

### El audio tartamudea o se corta

- Acérquese a su router Wi-Fi, o cambie a una red de 5 GHz
- Los auriculares Bluetooth con mala recepción pueden causar cortes — pruebe con auriculares con cable o con otro modelo
- El tráfico de red intenso (descargas grandes, videollamadas) en la misma Wi-Fi puede afectar al audio en tiempo real

### El sonido de los AirPods suena extrañamente con baja calidad en modo Standalone

HearRelay restringe el micrófono al **micrófono integrado** en modo Standalone para evitar forzar el Bluetooth a un modo de bajo ancho de banda (HFP). Use el micrófono integrado como entrada y los AirPods solo como salida. Es así por diseño.

### La grabación no se ha conservado

Las grabaciones se eliminan automáticamente **24 horas después de su creación** a menos que pulse **Conservar** sobre la grabación. Una vez conservadas, permanecen hasta que usted las elimine.

### HearRelay dejó de grabar cuando bloqueé la pantalla

HearRelay continúa capturando y retransmitiendo audio en segundo plano mientras la pantalla está bloqueada. Si la captura se detiene:

- Asegúrese de que **Background App Refresh** esté permitida para HearRelay (Ajustes de iOS → General → Background App Refresh)
- Asegúrese de que el **modo de bajo consumo** no esté suspendiendo agresivamente las tareas en segundo plano
- Algunas versiones de iOS suspenden las sesiones de audio cuando otra app de audio toma el control — detenga esa otra app

### El icono en la Isla Dinámica / pantalla bloqueada ha desaparecido

Las Live Activities tienen una duración máxima impuesta por el sistema (alrededor de 8 horas). Una vez alcanzada, el indicador puede dejar de actualizarse aunque HearRelay siga funcionando. Vuelva a abrir la Aplicación para refrescarlo.

**Importante:** Incluso si una Live Activity o el widget de la Pantalla bloqueada deja de actualizarse debido a los límites del sistema, **la captura de audio en segundo plano puede continuar mientras el monitoreo está activo**. Use esta función únicamente en situaciones de monitoreo lícitas y previamente divulgadas. No coloque un dispositivo en un lugar donde pueda captar a personas que no hayan recibido el aviso o consentimiento legalmente requerido. iOS también puede mostrar sus indicadores de micrófono / privacidad del sistema mientras la captura de audio está activa.

---

## Compras y suscripciones

### ¿HearRelay es una suscripción?

**No.** HearRelay Full Access es una **compra única, no consumible** (una IAP de pago único). **No** es una suscripción de renovación automática. Tras el periodo de prueba gratuito de 14 días, una sola compra desbloquea la Aplicación durante todo el tiempo en que mantenga su sesión iniciada con su Apple ID.

### Family Sharing

El desbloqueo está habilitado para **Family Sharing**, de modo que los miembros de su grupo de Family Sharing pueden usar HearRelay Full Access sin coste adicional.

### ¿Cómo restauro una compra anterior?

Abra la Aplicación → pulse el banner bloqueado → **Restore Purchases**. Apple verificará en su Apple ID el desbloqueo previo y lo volverá a aplicar.

### ¿Cómo obtengo un reembolso?

Las solicitudes de reembolso de compras realizadas en la App Store deben presentarse a través del proceso estándar de reembolsos de Apple en <https://reportaproblem.apple.com>. Apple procesa los reembolsos conforme a los términos de la App Store y de Apple Media Services. CONEX no recibe números de tarjetas de pago ni datos de facturación. Nada en este párrafo limita los derechos imperativos de protección al consumidor que pueda tener frente a CONEX en virtud de la ley aplicable.

---

## Lista de permisos

| Permiso | Necesario para | Ruta de ajustes |
|---|---|---|
| Micrófono | Cualquier monitoreo | Ajustes → HearRelay → Micrófono |
| Red local | Modo emparejado (envío / recepción con otros dispositivos) | Ajustes → HearRelay → Red local |
| iCloud (con sesión iniciada) | Modo emparejado (descubrir sus otros dispositivos) | Ajustes → \[Su nombre\] → iCloud |
| Background App Refresh | Monitoreo continuo con la pantalla apagada | Ajustes → General → Background App Refresh |

Si no está disponible Red local o iCloud, aún puede usar el modo **Standalone**.

---

## Contacto

- **Correo:** hearrelay-support@conex-cp.com
- Procuramos responder en unos pocos días hábiles. Incluya su versión de iOS, modelo de dispositivo y una descripción de los pasos que siguió.

Para preguntas de privacidad, vea la [Política de privacidad](/es/privacy/) o escriba a **hearrelay-privacy@conex-cp.com**.
Para reportes de seguridad, vea la [página de Seguridad](/es/security/) o escriba a **hearrelay-security@conex-cp.com**.

---

**Las traducciones están disponibles en:** [日本語](/ja/support/) · [Français](/fr/support/) · [Español](/es/support/) · [Português (Brasil)](/pt-BR/support/) · [简体中文](/zh-Hans/support/)

Cuando esta página se proporcione en cualquier idioma distinto al inglés, la **versión en inglés prevalecerá** en la medida permitida por la ley aplicable. Esta regla de precedencia no limita los derechos que le otorgan las leyes imperativas de protección al consumidor, privacidad o protección de datos de su país o región.
