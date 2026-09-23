# Principio de menor privilegio

Se aplicará el **principio de menor privilegio** a todos los usuarios, procesos y sistemas de la organización.

Cada usuario dispondrá únicamente de los permisos mínimos necesarios para realizar sus funciones. Los accesos se asignarán en función del puesto, las responsabilidades y la necesidad real de consultar o modificar determinada información.

Por ejemplo, los datos de Recursos Humanos relacionados con las **nóminas** solo podrán ser accesibles para aquellos trabajadores que necesiten esa información para desempeñar sus funciones.

Un empleado de otro departamento que no necesite consultar esta información no tendrá acceso a ella, aunque forme parte de la misma organización.

Los permisos también se limitarán según las acciones que cada usuario necesite realizar.

Por ejemplo:

- Un trabajador de Recursos Humanos encargado de elaborar las nóminas dispondrá de permisos de **lectura, creación y modificación**.
- Un auditor externo encargado únicamente de revisar la documentación dispondrá de permisos de **solo lectura**.
- Un usuario que no necesite trabajar con esta información no dispondrá de acceso.

De esta forma, se reducirá el riesgo de accesos indebidos, modificaciones no autorizadas, errores o exposición de información sensible.

# Flujo de revisión de permisos

Los permisos de acceso no se considerarán permanentes.

Se establecerá un proceso de revisión periódica para comprobar que cada usuario conserva únicamente los permisos necesarios para realizar sus funciones.

Las revisiones también se realizarán cuando se produzcan cambios como:

- Cambio de puesto.
- Cambio de departamento.
- Modificación de responsabilidades.
- Finalización de un proyecto.
- Baja de un empleado.
- Finalización de un acceso temporal.

Durante cada revisión se comprobará si los permisos actuales siguen estando justificados.

Los accesos que ya no sean necesarios deberán ser:

- Reducidos.
- Modificados.
- Revocados.

Todos los cambios realizados deberán quedar registrados para mantener trazabilidad sobre la gestión de permisos.

# Equipos implicados en el control y revisión de accesos

La gestión y revisión de permisos se repartirá entre distintos equipos de la organización.

Cada uno tendrá responsabilidades diferentes dentro del proceso de control de accesos.

## Equipo IAM

El equipo de **Identity and Access Management (IAM)** será responsable de gestionar las identidades digitales de los usuarios y sus permisos.

Entre sus funciones estarán:

- Crear y eliminar cuentas.
- Asignar usuarios a grupos y roles.
- Conceder y revocar permisos.
- Revisar los accesos existentes.
- Gestionar políticas de autenticación.
- Mantener registros de los cambios realizados.

El equipo IAM será uno de los principales responsables de aplicar y mantener el principio de menor privilegio.

## Equipo de IT

El equipo de IT será responsable de aplicar técnicamente los cambios de acceso sobre los distintos sistemas de la organización.

Entre sus funciones estarán:

- Modificar permisos sobre carpetas y recursos compartidos.
- Configurar grupos de seguridad.
- Aplicar permisos sobre servidores y aplicaciones.
- Eliminar accesos cuando dejen de ser necesarios.
- Desactivar cuentas cuando corresponda.

## Responsables de departamento

Los responsables de cada departamento deberán validar si los trabajadores de su área necesitan realmente los accesos que tienen asignados.

Por ejemplo, el responsable de Recursos Humanos deberá confirmar qué empleados necesitan mantener acceso a la documentación de nóminas.

Esta validación será necesaria porque los equipos IAM o IT pueden conocer los permisos técnicos asignados a un usuario, pero el responsable del departamento será quien pueda determinar si esos permisos siguen siendo necesarios para el desempeño de sus funciones.

## Equipo de Seguridad

El equipo de Seguridad revisará especialmente los accesos relacionados con:

- Datos sensibles.
- Datos críticos.
- Cuentas privilegiadas.
- Servidores.
- Sistemas administrativos.
- Información protegida mediante políticas DLP.

Su función será detectar permisos excesivos, configuraciones inseguras o privilegios que puedan representar un riesgo para la organización.

También podrá solicitar la reducción o revocación de permisos cuando detecte accesos que no estén correctamente justificados.

## Recursos Humanos

Recursos Humanos deberá comunicar cualquier cambio en la situación laboral de un empleado que pueda afectar a sus permisos.

Entre estos cambios se incluyen:

- Alta de nuevos trabajadores.
- Cambio de puesto.
- Cambio de departamento.
- Modificación de responsabilidades.
- Baja de empleados.

Esta información permitirá que IAM o IT actualicen los accesos de acuerdo con la situación actual de cada usuario.

## Auditoría o Compliance

Cuando existan estos equipos, Auditoría o Compliance comprobarán que las revisiones de acceso se están realizando correctamente.

También verificarán que los permisos asignados cumplen con:

- Las políticas internas de seguridad.
- El principio de menor privilegio.
- Los procedimientos establecidos de control de acceso.
- Los requisitos de seguridad y cumplimiento aplicables.

# Flujo básico de revisión

El proceso de revisión de permisos seguirá el siguiente flujo:

1. **IAM** obtendrá el listado actualizado de usuarios, roles y permisos.
2. Los **responsables de departamento** confirmarán qué accesos siguen siendo necesarios.
3. El **equipo de Seguridad** revisará especialmente los accesos privilegiados, sensibles o críticos.
4. **Recursos Humanos** informará de cambios de puesto, departamento, responsabilidades o bajas.
5. **IAM o IT** modificarán, reducirán o eliminarán los permisos que ya no sean necesarios.
6. Todos los cambios realizados quedarán registrados.
7. **Auditoría o Compliance** podrá revisar posteriormente que el proceso se haya realizado correctamente.

Este proceso permitirá mantener los permisos actualizados y evitar que los usuarios acumulen accesos innecesarios con el paso del tiempo.

La separación de responsabilidades también actuará como una medida adicional de seguridad.

La solicitud, validación, aplicación y revisión de permisos no recaerá en una única persona o equipo. De esta forma, los cambios de acceso podrán ser comprobados por distintos responsables antes de ser aplicados, reduciendo el riesgo de errores, abusos de privilegios o concesiones de acceso no justificadas.
