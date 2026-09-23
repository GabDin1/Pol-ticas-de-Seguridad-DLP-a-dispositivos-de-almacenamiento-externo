# Prevención de filtraciones

Se implementarán medidas específicas para evitar la filtración de datos sensibles y críticos, teniendo en cuenta cómo se almacenan, utilizan y transmiten.

Las principales medidas de protección serán:

- Cifrado de la información.
- Uso de herramientas DLP.
- Restricción del uso de dispositivos extraíbles.
- Control de transferencias de datos.
- Monitorización y registro de actividades.
- Bloqueo de acciones no autorizadas.

Estas medidas se aplicarán de forma conjunta para reducir el riesgo de pérdida, exposición o extracción no autorizada de información.

## Cifrado de la información

Los datos sensibles y críticos deberán permanecer cifrados cuando estén almacenados o sean transportados mediante dispositivos extraíbles.

El cifrado permitirá proteger la información en caso de pérdida, robo o acceso no autorizado al dispositivo.

Se aplicará cifrado en los siguientes casos:

- Archivos sensibles almacenados en equipos o servidores.
- Dispositivos USB corporativos utilizados para transportar información.
- Copias de seguridad que contengan datos sensibles.
- Información transmitida mediante canales que requieran protección adicional.

Los dispositivos USB corporativos utilizados para transportar información sensible deberán estar cifrados.

En entornos Windows podrán utilizarse soluciones como **BitLocker To Go** para proteger este tipo de dispositivos.

El uso de dispositivos USB personales o no autorizados quedará restringido para la transferencia de información sensible.

## Uso de herramientas DLP

Se utilizarán herramientas **Data Loss Prevention (DLP)** para detectar información sensible y controlar cómo puede utilizarse o transferirse.

Las políticas DLP supervisarán acciones como:

- Copia de archivos sensibles a dispositivos USB.
- Envío de información mediante correo electrónico.
- Subida de documentos a servicios de almacenamiento en la nube.
- Copia de información entre aplicaciones.
- Impresión de documentos sensibles.
- Transferencia de archivos fuera de la organización.
- Uso de servicios externos no autorizados.

Dependiendo de la acción realizada, la clasificación del dato y los permisos del usuario, la política DLP podrá:

- Permitir la operación.
- Permitirla y registrarla.
- Generar una alerta.
- Solicitar una justificación.
- Bloquear la transferencia.

## Política para dispositivos USB

La transferencia de información sensible a dispositivos USB solo estará permitida cuando se cumplan las siguientes condiciones:

- El usuario está autorizado para acceder a la información.
- El usuario necesita realizar la transferencia como parte de sus funciones.
- El equipo utilizado pertenece a la organización.
- El dispositivo USB está autorizado.
- El dispositivo USB está cifrado.
- La transferencia cumple con la política DLP establecida.

Si todas las condiciones se cumplen, la transferencia será permitida y quedará registrada.

Por ejemplo:

**Documento sensible + usuario autorizado + USB corporativo cifrado**

Resultado:

- Transferencia permitida.
- Actividad registrada.
- Información protegida mediante cifrado.

En cambio:

**Documento sensible + USB personal o no autorizado**

Resultado:

- Transferencia bloqueada.
- Evento registrado.
- Alerta generada para el equipo de Seguridad.

## Control de transferencias externas

Las políticas DLP también controlarán la salida de información a través de otros canales.

Se restringirán especialmente:

- Correos electrónicos enviados a cuentas personales.
- Servicios de almacenamiento en la nube no autorizados.
- Plataformas externas de intercambio de archivos.
- Aplicaciones no aprobadas.
- Dispositivos extraíbles no gestionados.

Cuando se detecte un intento de transferencia de información sensible hacia uno de estos destinos:

- La operación podrá ser bloqueada.
- El evento quedará registrado.
- Se generará una alerta cuando el nivel de riesgo lo requiera.

## Combinación de cifrado y DLP

El cifrado y las herramientas DLP se utilizarán de forma complementaria.

La solución DLP controlará:

- Quién puede realizar una transferencia.
- Qué información intenta transferir.
- Qué dispositivo o servicio está utilizando.
- Si la operación está permitida.
- Si la acción debe registrarse, alertarse o bloquearse.

El cifrado protegerá:

- El contenido de los archivos.
- La información almacenada en dispositivos USB.
- Los datos en caso de pérdida o robo del dispositivo.

Por tanto, el flujo de protección será:

1. El usuario accede a información sensible.
2. La solución DLP identifica la clasificación del dato.
3. Se comprueba si la acción solicitada está permitida.
4. Se comprueba que el destino utilizado está autorizado.
5. Si se cumplen las condiciones, la transferencia se permite.
6. La operación queda registrada.
7. La información permanece cifrada mientras está almacenada en el dispositivo.

## Medidas generales de prevención

Como parte de la política de prevención de filtraciones:

- Los datos sensibles deberán almacenarse cifrados cuando corresponda.
- Los datos críticos requerirán medidas de protección reforzadas.
- Los dispositivos USB utilizados para información sensible deberán ser corporativos y estar cifrados.
- Se bloqueará la copia de información sensible a dispositivos no autorizados.
- Se restringirá el envío de datos sensibles a servicios externos no aprobados.
- Las transferencias relevantes quedarán registradas.
- Las actividades de riesgo podrán generar alertas para el equipo de Seguridad.
- Las políticas DLP serán revisadas periódicamente para adaptarlas a nuevas necesidades o riesgos.

La combinación de estas medidas permitirá reducir el riesgo de que información sensible abandone el entorno controlado de la organización o pueda ser utilizada por personas no autorizadas.
