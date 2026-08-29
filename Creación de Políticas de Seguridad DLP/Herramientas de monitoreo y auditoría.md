# Monitoreo y Auditoría

La protección de datos sensibles no consiste únicamente en limitar quién puede acceder a ellos. También es necesario monitorizar cómo se utilizan y mantener un registro de las actividades realizadas sobre dicha información.

El **monitoreo** permite detectar comportamientos que puedan representar un riesgo para los datos de la organización, mientras que la **auditoría** permite mantener un registro de las acciones realizadas para poder revisarlas posteriormente.

## Monitoreo de datos sensibles

Las políticas DLP deben establecer qué actividades relacionadas con datos sensibles serán monitorizadas.

* Acceso a documentos o bases de datos sensibles.
* Copia de información a dispositivos USB.
* Envío de documentos sensibles mediante correo electrónico.
* Subida de archivos a servicios de almacenamiento en la nube.
* Copia y pegado de información sensible entre aplicaciones.
* Descarga de grandes cantidades de información.
* Intentos de acceso a información para la que el usuario no dispone de permisos.
* Modificaciones en los permisos de acceso.
* Transferencias de información fuera de la organización.

Dependiendo de la política definida, el sistema puede:

* Permitir la acción.
* Registrar la actividad.
* Generar una alerta.
* Solicitar una justificación al usuario.
* Bloquear la operación.

Por ejemplo, un trabajador autorizado de Recursos Humanos necesita trasladar varios documentos de nóminas desde su ordenador corporativo a otro equipo de la empresa. Para realizar esta tarea utiliza un dispositivo USB corporativo autorizado y cifrado. Cuando intenta copiar los documentos, la solución DLP detecta que contienen información clasificada como sensible y comprueba que la operación cumple con la política establecida por la organización. Al tratarse de un usuario autorizado, trabajando desde un equipo corporativo y utilizando un dispositivo USB permitido, la transferencia se realiza correctamente y queda registrada para su posterior auditoría. Una vez finalizada la copia, el trabajador extrae el dispositivo USB y lo conecta en otro equipo corporativo autorizado. Como el dispositivo está cifrado, el contenido permanece protegido durante el traslado. En el segundo equipo se vuelve a comprobar que el usuario dispone de los permisos necesarios para acceder a la información. Si las condiciones de seguridad se cumplen, el usuario puede desbloquear el dispositivo y acceder a los documentos.
De esta forma, la organización permite una transferencia legítima de información sensible sin perder el control sobre quién puede acceder a ella, qué dispositivos pueden utilizarse y qué acciones se realizan sobre los datos.

## Auditoría de actividades

Las actividades relacionadas con datos sensibles deben quedar registradas para poder conocer posteriormente qué ha ocurrido.

Los registros de auditoría deberían incluir, cuando sea posible:

* Usuario que realizó la acción.
* Fecha y hora.
* Recurso o documento al que se accedió.
* Tipo de acción realizada.
* Equipo o dispositivo desde el que se produjo.
* Destino de la información.
* Resultado de la acción.
* Regla o política DLP que fue activada.

Estos registros permiten investigar incidentes, detectar comportamientos anómalos y comprobar que las políticas de seguridad se están cumpliendo.

Los registros se almacenan de forma protegida y conservarse durante el periodo establecido por la política de seguridad de la organización.

## Herramientas DLP

Las soluciones DLP permiten identificar información sensible y controlar las acciones que los usuarios realizan sobre ella.

Algunos ejemplos son:

### Symantec DLP

Permite monitorizar el uso de información sensible y aplicar controles sobre diferentes acciones realizadas por los usuarios.

Entre sus capacidades se encuentran el control de aplicaciones, copiar y pegar, capturas de pantalla y análisis del comportamiento relacionado con los datos.

### Forcepoint DLP

Permite supervisar el uso y movimiento de información sensible y establecer políticas para detectar o impedir determinadas acciones.

Puede utilizarse para controlar datos tanto en equipos de usuario como en otros entornos de la organización.

### Digital Guardian

Permite monitorizar el uso de datos en diferentes sistemas y aplicar controles sobre las acciones realizadas con información protegida.

También dispone de capacidades de análisis del comportamiento de los usuarios.

### McAfee DLP Endpoint

Permite aplicar políticas DLP directamente sobre los equipos de los usuarios y controlar acciones relacionadas con la utilización o transferencia de información sensible.

## Herramientas SIEM

Además de las soluciones DLP, una organización puede utilizar un **SIEM (Security Information and Event Management)**.

Un SIEM centraliza registros procedentes de diferentes sistemas de la organización y permite analizar y correlacionar los eventos de seguridad.

Algunos ejemplos de soluciones SIEM son:

* Wazuh.
* Microsoft Sentinel.
* Splunk Enterprise Security.

El SIEM puede recibir eventos procedentes de:

* Soluciones DLP.
* Servidores.
* Firewalls.
* Sistemas de autenticación.
* Aplicaciones.
* Equipos de usuario.

De esta forma, un evento DLP puede analizarse junto con otra información de seguridad.

Por ejemplo:

1. Un usuario accede a una gran cantidad de documentos sensibles.
2. Poco después conecta un dispositivo USB.
3. La herramienta DLP detecta un intento de copia de los documentos.
4. Los diferentes eventos son enviados al SIEM.
5. El SIEM correlaciona los eventos y genera una alerta para el equipo de Seguridad.

## Ejemplo de política de monitoreo

Siguiendo el ejemplo anterior de los documentos de nóminas:

Un trabajador autorizado de Recursos Humanos puede consultar y modificar las nóminas desde los sistemas de la empresa.

Sin embargo, se establecerán controles adicionales cuando intente:

* Copiar las nóminas a un dispositivo externo.
* Enviarlas a una dirección de correo externa.
* Subirlas a un servicio de almacenamiento no autorizado.
* Descargar una cantidad anormalmente elevada de documentos.

Estas acciones quedarán registradas y, dependiendo de su nivel de riesgo, podrán generar una alerta o ser bloqueadas.

De esta forma, la organización no solo controla **quién puede acceder a los datos**, sino también **qué hace el usuario con esos datos una vez que ha obtenido acceso**.

