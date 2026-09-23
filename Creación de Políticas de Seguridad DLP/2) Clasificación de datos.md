# Clasificación de datos

Se implementará un sistema de clasificación de la información basado en su nivel de sensibilidad y en el impacto que podría provocar una pérdida, modificación o acceso no autorizado.

Toda la información gestionada por la organización se clasificará en tres niveles principales:

- **Datos Internos**
- **Datos Sensibles**
- **Datos Críticos**

La clasificación asignada determinará las medidas de protección que se aplicarán sobre cada tipo de información, incluyendo controles de acceso, cifrado, monitorización, restricciones de copia y transferencia, y medidas de auditoría.

## Datos Internos

Se clasificarán como **Datos Internos** aquellos documentos e informaciones destinados exclusivamente al uso dentro de la organización y que no deban hacerse públicos.

Dentro de esta categoría se incluirán, entre otros:

- Procedimientos internos.
- Organigramas.
- Manuales de trabajo.
- Comunicaciones entre departamentos.
- Documentación técnica no confidencial.
- Inventarios de equipos.

El acceso a esta información quedará limitado a empleados y colaboradores autorizados.

Estos datos podrán compartirse dentro de la organización cuando sea necesario para el desempeño de las funciones profesionales, pero no deberán enviarse a destinatarios externos ni almacenarse en servicios no autorizados.

## Datos Sensibles

Se clasificarán como **Datos Sensibles** aquellos cuya exposición, modificación o pérdida pueda causar daños a la organización, a sus clientes, empleados o colaboradores.

Dentro de esta categoría se incluirán:

- Datos personales de clientes y empleados.
- Información bancaria.
- Nóminas.
- Contratos.
- Historiales de clientes.
- Información financiera.
- Bases de datos con información personal.
- Documentación legal.

El acceso a estos datos se concederá únicamente a los usuarios que necesiten utilizarlos para desempeñar sus funciones.

Sobre esta información se aplicarán las siguientes medidas:

- Control de acceso basado en roles.
- Aplicación del principio de menor privilegio.
- Registro de accesos y operaciones realizadas.
- Cifrado de la información almacenada o transportada.
- Monitorización mediante herramientas DLP.
- Restricción de copia a dispositivos USB no autorizados.
- Restricción del envío a cuentas de correo externas no autorizadas.
- Restricción del uso de servicios de almacenamiento no aprobados.
- Revisión periódica de los permisos de acceso.

Cuando un usuario autorizado necesite transportar información sensible mediante un dispositivo USB, deberá utilizar un **USB corporativo autorizado y cifrado**.

La transferencia deberá quedar registrada para su posterior auditoría.

## Datos Críticos

Se clasificarán como **Datos Críticos** aquellos cuya pérdida, modificación o exposición pueda comprometer directamente la seguridad de los sistemas o provocar consecuencias graves para la organización.

Dentro de esta categoría se incluirán:

- Contraseñas administrativas.
- Claves privadas.
- Tokens de acceso.
- Credenciales de servidores.
- Copias completas de bases de datos.
- Secretos empresariales.
- Información estratégica especialmente confidencial.

El acceso a los datos críticos quedará limitado a un número reducido de usuarios expresamente autorizados.

Sobre esta información se aplicarán controles adicionales:

- Autenticación multifactor.
- Acceso basado en roles.
- Aplicación estricta del principio de menor privilegio.
- Cifrado obligatorio.
- Registro y auditoría de los accesos.
- Restricción de copia a dispositivos extraíbles.
- Monitorización mediante herramientas de seguridad.
- Revisión periódica de permisos privilegiados.
- Revocación inmediata de accesos cuando dejen de ser necesarios.

Los datos críticos no podrán almacenarse en dispositivos personales ni transferirse mediante servicios externos no autorizados.

## Aplicación de la clasificación

La clasificación asignada a cada dato determinará el nivel de protección que se aplicará.

De forma general:

- **Datos Internos:** acceso restringido al personal autorizado de la organización.
- **Datos Sensibles:** acceso limitado según función, con cifrado, monitorización y controles DLP.
- **Datos Críticos:** acceso estrictamente limitado, cifrado obligatorio, autenticación reforzada y auditoría.

Este sistema permitirá aplicar medidas de seguridad proporcionales al nivel de riesgo asociado a cada tipo de información.
