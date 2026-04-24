---
title: Soporte — HearRelay
lang: es
---

# Soporte

Gracias por usar **HearRelay**. Esta página reúne consejos de resolución de problemas y cómo contactarnos.

> Esta traducción se proporciona por conveniencia. En caso de discrepancia con la [versión en inglés](/en/support/), prevalecerá la versión en inglés.

---

## Ayuda rápida

### "No se han encontrado dispositivos" al intentar emparejar

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

Las grabaciones se eliminan automáticamente **24 horas después de su creación** a menos que pulse **Conservar**. Una vez conservadas, permanecen hasta que usted las elimine.

### HearRelay dejó de grabar cuando bloqueé la pantalla

HearRelay continúa capturando y retransmitiendo audio en segundo plano mientras la pantalla está bloqueada. Si la captura se detiene:

- Asegúrese de que **Actualización en segundo plano** esté permitida para HearRelay (Ajustes iOS → General → Actualización en segundo plano)
- Asegúrese de que el **modo de bajo consumo** no esté suspendiendo agresivamente las tareas en segundo plano
- Algunas versiones de iOS suspenden las sesiones de audio cuando otra app de audio toma el control — detenga esa otra app

### El icono en la Isla Dinámica / pantalla bloqueada ha desaparecido

Las Live Activities tienen una duración máxima impuesta por el sistema (alrededor de 8 horas). Una vez alcanzada, el indicador puede dejar de actualizarse aunque HearRelay siga funcionando. Vuelva a abrir la Aplicación para refrescarlo.

---

## Lista de permisos

| Permiso | Necesario para | Ruta de ajustes |
|---|---|---|
| Micrófono | Cualquier monitoreo | Ajustes → HearRelay → Micrófono |
| Red local | Modo emparejado (envío / recepción con otros dispositivos) | Ajustes → HearRelay → Red local |
| iCloud (con sesión iniciada) | Modo emparejado (descubrir sus otros dispositivos) | Ajustes → \[Su nombre\] → iCloud |
| Actualización en segundo plano | Monitoreo continuo con la pantalla apagada | Ajustes → General → Actualización en segundo plano |

Si no está disponible Red local o iCloud, aún puede usar el modo **Standalone**.

---

## Contacto

- **Correo:** hearrelay-support@conex-cp.com
- Procuramos responder en unos pocos días hábiles. Incluya su versión de iOS, modelo de dispositivo y una descripción de los pasos que siguió.

Para preguntas de privacidad, vea la [Política de privacidad](/es/privacy/) o escriba a **hearrelay-privacy@conex-cp.com**.
Para reportes de seguridad, vea la [página de Seguridad](/es/security/) o escriba a **hearrelay-security@conex-cp.com**.

---

**English version:** [Support](/en/support/)
