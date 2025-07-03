Este BOT se integra con las API de ISPBrain de Crenein.
By Ruben Castillo -> Update GPT: Luis Sánchez 06-2025

✅ Endpoint > Autenticar > Solicitar Token
✅ Endpoint > Autenticar > Validar por teléfono
✅ Endpoint > Autenticar > Validar por DNI
✅ Endpoint > ISP > Últimos tickets > buscar tickets
✅ Endpoint > Administración > plan buscar > Validar Conexiones (muestra los planes del cliente)
✅ Endpoint > Administración > mis comprobantes > comprobantes
✅ Endpoint > Soporte técnico > Visita técnica > Crear Ticket en ISP
✅ Endpoint > Soporte técnico > Últimos tickets > buscar tickets

Ajustes API de ISPBrain

Actualizar variables para Token
1.1 isp_url: {{secreto_1}}
1.2 isp_user: {{secreto_2}}
1.3 isp_password: {{secreto_3}}

Soporte técnico > Visita técnica > Webhook > Crear ticket en ISP
Actualizar variables para Crear ticket

3.1 isp_ticket_category_id
3.2 isp_ticket_status_id
3.3 isp_ticket_spaces (nombre de la sucursal)

Ajustes al Bot:

Variable > Empresa
Configuración de Endpoints
Derivaciones > Asignar departamentos > departamentos
Derivaciones > Asignar departamentos administración > departamentos
Derivaciones > Validar feriados > marcar como abierta la conversación
Derivaciones > Validar feriados administración > marcar como abierta la conversación
Derivaciones > Validar horario laboral > marcar como abierta la conversación
Derivaciones > Validar horario laboral administración > marcar como abierta la conversación
Transferir con un agente administración > marcar como abierta la conversación
Derivaciones > Horarios laborales
Administración > accesos al portal > {{portal_url}}
Administración > informar pago > Asignar la conversación departamento de "Administración".
Administración > informar pago > marcar como abierta la conversación.
Administración > plan > Asignar la conversación departamento de "Administración".
Ventas > contratar servicio > marcar como abierta la conversación

Departamentos:
Ventas (por defecto)
Administración
Soporte técnico

Etiquetas:
informar_pago
modificar_plan
solicitar_factura
servicio_lento
sin_servicio
asistencia_técnica
error_ticket_isp
contratar_servicio
otras_consultas
