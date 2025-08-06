# ✅ ACTA DE VALIDACIÓN Y ENTREGA DE CHATBOT

## 🧾 Datos del Proyecto: Upgrade Bot Boplay IVR a GPT

- **Nombre del proyecto**: boplay_gpt_v1 ID: 63533
- **Cliente**: BOPLAY
- **Fecha de entrega**: {{dd/mm/aaaa}}
- **Versión del bot entregado**: v1.0 / 07-2025
- **Modelo GPT**: 4o
- **Temperatura**: 0.1
- **Desarrollado por**: Asisteclick / L. Sánchez
- **Revisión y Aprobación**: BOPLAY / Wilson Brest
- **Canales habilitados**: ✅ asignado, ❌ sin asignar, ⚠️ pendiente por definir, 🚫 No será usado
  - Web
  - 🚫 Email
  - Facebook Messenger
  - Instagram
  - Whatsapp
  - Telegram
  - 🚫 Teams
  - 🚫 Tiendanube

## 🧪 Validación de Funcionalidades (UAT - User Acceptance Testing)

Durante las pruebas de aceptación, se validaron las funcionalidades críticas del chatbot. Se utilizó la siguiente leyenda para calificar los resultados:

### 🔁 Leyenda de Estados

| Emoji | Estado      | Descripción                                                                |
| ----- | ----------- | --------------------------------------------------------------------------- |
| ✅    | Correcto    | La funcionalidad cumple completamente lo esperado.                          |
| ⚠️  | Parcial     | La funcionalidad opera parcialmente o con errores menores.                  |
| ❌    | Falla       | La funcionalidad no cumple lo esperado o presenta errores críticos.        |
| 🔕    | Desactivada | El cliente decidió desactivar esta funcionalidad en esta versión del bot. |

---

### 📋 Resultados de Validación

| N° | Funcionalidad                                                                         | Resultado Esperado                                                                                             | Resultado Obtenido | Validado por el cliente |
| --- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------ | ----------------------- |
| 1   | Respuesta a saludo inicial                                                            | El bot responde con mensaje de bienvenida                                                                      | ✅ Correcto        | ✅                      |
| 2   | Validar cliente por DNI                                                               | El bot valida con la API de ISP Brain                                                                          | ✅ Correcto        | ✅                      |
| 3   | Validar Cliente por Teléfono                                                         | El bot valida con la API de ISP Brain                                                                          | ✅ Correcto        | ✅                      |
| 4   | Informar datos al validarse por dni                                                   | El bot informa deuda de pago, plan y link de pago - se pregunta si desea opciones de administracion y soporte  | ✅ Correcto        | ✅                      |
| 5   | Informar datos al validarse por telefono                                              | El bot informa deuda de pago, plan y link de pago - se pregunta si desea opciones de administracion y soporte | ✅ Correcto        | ✅                      |
| 6   | Si api_connections_labels tiene INFOBOT notificar que hay falla validado por dni      | EL bot indica que hay un mantenimiento a su red, cierra el caso ejemplo dni: 33214158                          | ✅ Correcto        | ✅                      |
| 7   | Si api_connections_labels tiene INFOBOT notificar que hay falla validado por telefono | EL bot indica que hay un mantenimiento a su red, cierra el caso                                                | ✅ Correcto        | ✅                      |
| 8   | Menu administracion - gestionar mi plan                                               | muestra los planes actuales del cliente                                                                        | ✅ Correcto        | ✅                      |
| 9   | Menu administracion - cambiar de plan                                                 | pasa la solcitud a administracion - sigue diciendo nombres planes                                              | ✅ Correcto        | ✅ Correcto             |
| 10  | Menu administracion - hablar con personal administrativo                              | si es cliente se pasa a administracion, si no lo es se pasa a atencion al cliente                              | ✅ Correcto        | ✅                      |
| 11  | Soporte - menu                                                                        |                                                                                                                | ✅ Correcto        | ✅                      |
| 12  | Soporte - sin servicio                                                                |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 13  | Soporte - servicio lento                                                              |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 14  | Soporte - test velocidad                                                              |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 15  | Soporte - cambio de contraseña wifi                                                  |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 16  | Soporte - hablar con personal tecnico                                                 |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 17  | Soporte - agendar visita                                                              | se agrega nueva logica usando hablar con un tecnico                                                            | ✅ Correcto        | ✅ Correcto             |
| 18  | Ventas - menu                                                                         |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 19  | Ventas - planes                                                                       |                                                                                                                | ✅ Correcto        | ✅ Correcto             |
| 20  | Ventas - quiero contratar                                                             | ⚠️ pendiente revisar con ubicacion con google map desde whatsapp                                             | ✅ Correcto        | ✅ Correcto             |
| 21  | Ventas - otras consultas                                                              |                                                                                                                | ✅ Correcto        |                         |
| 22  | Ventas - tipos de servicios                                                           |                                                                                                                | ✅ Correcto        |                         |
| 23  | Ventas - ubicacion maps                                                               |                                                                                                                | ✅ Correcto        |                         |
| 24  | Ventas - marketing                                                                    |                                                                                                                | ✅ Correcto        |                         |
| 25  | Ventas - Otras consultas - reconexion                                                 | ✅ 1. flujo cuando tiene los equipos, ✅ 2. flujo cuando no tiene los equipos nueva contratacion               | ✅ Correcto       |                         |
| 26  | Ventas - Otras consultas - otras consultas                                            | ✅ se separó de productos                                                                                     | ✅ Correcto        | ✅ Correcto             |
| 27  | 🟢 Ventas de productos                                                                | ⚠️ se agrega flujo para ventas de productos, tiene errores                                                   |                    |                         |
| 28  | 🟢 Quiero Pagar - donde pago                                                          | ⚠️ Se ajusta el prompt con un flujo basico                                                                   |                    |                         |
| 29  | 🟢 Mudanzas traslados                                                                 | ⚠️ No existe el flujo,                                                                                       |                    |                         |
| 30  | 🟢 Darse de baja, solicitar baja                                                      | ⚠️ No existe el flujo                                                                                       |                    |                         |
|     | Faltan los datos de la direccion de boplay                                            |                                                                                                                |                    |                         |

> *Los ítems marcados con ⚠️ o ❌ deben ser corregidos o mejorados en una versión posterior o quedar registrados como requerimientos futuros.*

## 🧩 Requerimientos Fuera de Alcance / Cambios Solicitados

### 🔁 Leyenda de Estados

A continuación, se enumeran solicitudes o cambios reportados durante las pruebas o reuniones, que **no forman parte del alcance de esta versión**, pero quedan registrados para evaluación o desarrollo en versiones futuras:

| Emoji | Estado                                     | Descripción                                                          |
| ----- | ------------------------------------------ | --------------------------------------------------------------------- |
| ⚠️  | **Pendiente**                        | El cambio fue recibido pero aún no ha sido evaluado.                 |
| ⏳    | **En análisis**                     | Se está revisando su viabilidad técnica o funcional.                |
| 🚫    | **No viable**                        | No es posible implementarlo por restricciones técnicas o de negocio. |
| 🔲    | **No priorizado**                    | Se documenta pero no se desarrollará por ahora.                      |
| 🟢    | **Aprobado para cotización futura** | Se acordó evaluar esfuerzo y costo para una próxima versión.       |

| N° | Descripción del requerimiento                                                                                                                                   | Solicitado por | Fecha    | Estado | Observaciones |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | -------- | ------ | ------------- |
| 1   | aca solo archivo y creo un tiket en ispbrain. Lo cual no esta mal pero deberia derivar esto a soporte tecnico para lograr validad si se puede o no . NO ARCHIVAR |                |          |        |               |
| 2   | 🟢 se actualiza flujo de reconexiones.                                                                                                                           | Wilson         | 1/8/2025 | 🟢     |               |
| 3   |                                                                                                                                                                  |                |          |        |               |
