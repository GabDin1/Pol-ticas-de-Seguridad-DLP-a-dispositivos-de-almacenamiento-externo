# Monitoreo y Auditoría

Se implementará un sistema de **monitoreo y auditoría** sobre las actividades relacionadas con datos sensibles y críticos.

El objetivo será detectar comportamientos de riesgo, registrar las acciones realizadas sobre la información y disponer de evidencias que permitan investigar incidentes o comprobar el cumplimiento de las políticas de seguridad.

El monitoreo permitirá detectar actividades potencialmente peligrosas, mientras que la auditoría permitirá mantener un registro detallado de lo ocurrido para su posterior revisión.

## Monitoreo de datos sensibles

Se monitorizarán especialmente las acciones relacionadas con información clasificada como sensible o crítica.

Entre las actividades que serán supervisadas se incluyen:

- Acceso a documentos o bases de datos sensibles.
- Copia de información a dispositivos USB.
- Envío de documentos sensibles mediante correo electrónico.
- Subida de archivos a servicios de almacenamiento en la nube.
- Copia y pegado de información sensible entre aplicaciones.
- Descarga de grandes cantidades de información.
- Intentos de acceso a información sin permisos suficientes.
- Modificaciones en permisos de acceso.
- Transferencias de información fuera de la organización.

Dependiendo del tipo de información, del usuario y de la acción realizada, las políticas DLP podrán:

- Permitir la acción.
- Permitirla y registrarla.
- Generar una alerta.
- Solicitar una justificación.
- Bloquear la operación.

Por ejemplo, si un trabajador autorizado necesita trasladar documentos de nóminas entre dos equipos corporativos, deberá utilizar un dispositivo USB corporativo autorizado y cifrado.

Cuando se realice la copia, la solución DLP comprobará que:

- El usuario está autorizado.
- El archivo está clasificado como información sensible.
- El equipo de origen es corporativo.
- El dispositivo USB está autorizado.
- La transferencia cumple con la política establecida.

Si todas las condiciones se cumplen, la copia será permitida y la actividad quedará registrada.

Posteriormente, cuando el dispositivo USB se conecte a otro equipo corporativo, se volverán a aplicar los controles de acceso necesarios antes de permitir el uso de la información.

De esta forma, se podrá realizar una transferencia legítima de información sensible manteniendo trazabilidad sobre el usuario, el dispositivo y las acciones realizadas.

# Auditoría de actividades

Todas las actividades relevantes relacionadas con datos sensibles o críticos deberán quedar registradas.

Los registros de auditoría incluirán, cuando sea posible:

- Usuario que realizó la acción.
- Fecha y hora.
- Documento o recurso afectado.
- Clasificación de la información.
- Tipo de acción realizada.
- Equipo desde el que se realizó.
- Dispositivo utilizado.
- Destino de la información.
- Resultado de la acción.
- Política o regla DLP activada.

Estos registros permitirán:

- Investigar incidentes.
- Detectar comportamientos anómalos.
- Identificar intentos de acceso no autorizado.
- Revisar transferencias de información.
- Verificar el cumplimiento de las políticas de seguridad.

Los registros deberán almacenarse de forma protegida y conservarse durante el periodo definido por la política de seguridad de la organización.

El acceso a estos registros también estará restringido a los equipos responsables de seguridad, administración y auditoría.

# Herramientas DLP

Se utilizarán soluciones DLP para identificar información sensible y controlar las acciones realizadas sobre ella.

Estas herramientas deberán permitir:

- Detectar información clasificada como sensible.
- Monitorizar el uso de archivos.
- Controlar transferencias hacia dispositivos USB.
- Supervisar envíos por correo electrónico.
- Controlar subidas a servicios externos.
- Registrar las acciones realizadas.
- Generar alertas.
- Bloquear transferencias no autorizadas.

Algunas soluciones que pueden utilizarse para estas funciones son:

- **Symantec DLP**
- **Forcepoint DLP**
- **Digital Guardian**
- **McAfee DLP Endpoint**

La herramienta seleccionada deberá integrarse con los sistemas de autenticación, control de acceso y monitorización utilizados por la organización.

# Herramientas SIEM

Además de las herramientas DLP, se utilizará una solución **SIEM (Security Information and Event Management)** para centralizar y analizar los eventos de seguridad generados por los distintos sistemas.

El SIEM recibirá registros procedentes de:

- Soluciones DLP.
- Servidores.
- Firewalls.
- Sistemas de autenticación.
- Aplicaciones.
- Equipos de usuario.
- Sistemas de control de acceso.

Entre las soluciones que pueden utilizarse se encuentran:

- **Wazuh**
- **Microsoft Sentinel**
- **Splunk Enterprise Security**

El SIEM permitirá correlacionar diferentes eventos para detectar comportamientos que, de forma aislada, podrían no resultar sospechosos.

Por ejemplo:

1. Un usuario accede a una cantidad elevada de documentos sensibles.
2. Poco después conecta un dispositivo USB.
3. La herramienta DLP detecta un intento de copia.
4. Los eventos se envían al SIEM.
5. El SIEM correlaciona la actividad.
6. Se genera una alerta para el equipo de Seguridad.

# Reglas de monitoreo

Se establecerán reglas específicas para controlar el uso de información sensible.

Por ejemplo:

## Acceso normal a información sensible

Un usuario autorizado podrá acceder a la información necesaria para realizar sus funciones.

La acción será:

- Permitida.
- Registrada.

## Copia a USB corporativo autorizado

Si un usuario autorizado copia información sensible a un dispositivo USB corporativo y cifrado:

- La transferencia será permitida.
- La acción quedará registrada.
- Se almacenará información sobre el usuario, archivo y dispositivo utilizado.

## Copia a USB no autorizado

Si un usuario intenta copiar información sensible a un dispositivo USB personal o no autorizado:

- La transferencia será bloqueada.
- Se generará una alerta.
- El evento quedará registrado.

## Envío de información a servicios externos

Si un usuario intenta enviar información sensible a una cuenta de correo personal o subirla a un servicio externo no autorizado:

- La acción será bloqueada.
- Se generará una alerta.
- El evento será enviado al sistema de monitorización.

## Descarga anormal de información

Si un usuario descarga una cantidad inusual de documentos sensibles en un periodo corto de tiempo:

- La actividad será registrada.
- Se generará una alerta.
- El equipo de Seguridad revisará el comportamiento.

# Revisión de eventos

El equipo de Seguridad revisará periódicamente las alertas y eventos generados por las herramientas DLP y SIEM.

Las actividades de mayor riesgo serán analizadas para determinar si corresponden a:

- Una actividad legítima.
- Un error del usuario.
- Un incumplimiento de las políticas.
- Un posible incidente de seguridad.

Cuando se detecte una actividad no autorizada, se aplicarán los procedimientos de respuesta a incidentes establecidos.

De esta forma, la organización no solo controlará quién puede acceder a la información, sino también qué acciones realiza sobre ella y si esas acciones cumplen con las políticas de seguridad definidas.
