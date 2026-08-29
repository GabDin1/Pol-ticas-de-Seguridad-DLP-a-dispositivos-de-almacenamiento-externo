# Principio de menor privilegio

Pongamos como ejemplo una organización ficticia llamada **YGriegas**.

Los datos de Recursos Humanos relacionados con las **nóminas** deberían ser accesibles únicamente para aquellos trabajadores de Recursos Humanos que necesiten esa información para realizar su trabajo.

Un empleado de otro departamento que no necesite consultar esa información en sus funciones habituales no debería tener acceso a ella, aunque forme parte de la misma organización.

Por ejemplo, un usuario de Recursos Humanos cuyo trabajo sea elaborar las nóminas debería disponer de permisos de **lectura, creación y modificación** sobre esos documentos.

En cambio, un auditor externo encargado de revisar la documentación legal de la empresa podría necesitar consultar las nóminas, pero no modificarlas ni crear nuevos documentos. En ese caso, debería disponer únicamente de permisos de **lectura**.

A esto se le conoce como **principio de menor privilegio**.

El principio de menor privilegio establece que cada usuario, proceso o sistema debe disponer únicamente de los permisos mínimos necesarios para realizar sus funciones. De esta forma, se reduce el riesgo de accesos indebidos, errores, modificaciones no autorizadas o exposición de información sensible.

# Flujo de revisión de permisos

Los permisos de acceso a los diferentes datos de la empresa no deben considerarse permanentes. Deben revisarse periódicamente y también cuando cambie la situación, el puesto o las responsabilidades de un usuario.

El objetivo de estas revisiones es comprobar que cada usuario conserva únicamente los permisos necesarios para realizar sus funciones y retirar aquellos accesos que ya no estén justificados.

# Equipos implicados en el control y revisión de accesos

En una organización, hay distintos equipos que participan en el control y revisión de permisos, cada uno con responsabilidades diferentes:

**Equipo IAM**

El equipo de Identity and Access Management (IAM) se encarga de gestionar las identidades digitales de los usuarios y sus permisos.

Entre sus funciones se encuentran:

Crear y eliminar cuentas.
Asignar usuarios a grupos y roles.
Conceder o revocar permisos.
Revisar accesos existentes.
Gestionar políticas de autenticación.
Mantener registros de los cambios realizados.

**Equipo de IT**

El equipo de IT puede encargarse de aplicar técnicamente los cambios de acceso sobre los sistemas, servidores, aplicaciones, carpetas compartidas o dispositivos.

Por ejemplo, puede modificar permisos sobre una carpeta, eliminar el acceso de un usuario o configurar grupos de seguridad.

Responsables de departamento

Los responsables de cada departamento deben validar si un trabajador necesita realmente determinados accesos para realizar sus funciones.

Por ejemplo, el responsable de Recursos Humanos puede confirmar qué empleados necesitan acceso a la documentación de nóminas.

Esto es importante porque el equipo IAM o IT puede conocer los permisos técnicos de un usuario, pero no necesariamente si esos permisos siguen siendo necesarios para su trabajo diario.

**Equipo de Seguridad**

El equipo de Seguridad puede revisar especialmente los accesos relacionados con:

Datos sensibles.
Datos críticos.
Cuentas privilegiadas.
Servidores.
Sistemas administrativos.
Información protegida por políticas DLP.

Su función es detectar accesos excesivos, configuraciones inseguras o privilegios que puedan suponer un riesgo para la organización.

**Recursos Humanos**

Recursos Humanos tiene un papel importante porque debe comunicar cambios que puedan afectar a los permisos de los usuarios, como:

Alta de un nuevo trabajador.
Cambio de puesto.
Cambio de departamento.
Baja de un empleado.

Esta información permite que IAM o IT modifiquen los permisos de acuerdo con la nueva situación del usuario.

**Auditoría o Compliance**

En organizaciones que dispongan de estos equipos, Auditoría o Compliance pueden comprobar que las revisiones de acceso se realizan correctamente y que los permisos cumplen con las políticas internas y los requisitos de seguridad establecidos.

**Flujo básico de revisión**

Un ejemplo de como se podría aplicar un flujo básico de revisión.

IAM obtiene el listado de usuarios, roles y permisos actuales.
El responsable de cada departamento confirma qué accesos siguen siendo necesarios.
Seguridad revisa especialmente los accesos privilegiados, sensibles o críticos.
Recursos Humanos informa de cambios de puesto, departamento o bajas.
IAM o IT modifica o elimina los permisos que ya no sean necesarios.
Los cambios quedan registrados.
Auditoría o Compliance puede comprobar posteriormente que el proceso se ha realizado correctamente.

De esta forma, la revisión de accesos no depende de una única persona o equipo y se mantiene una separación de responsabilidades. La división de responsabilidades también es en sí una medida de prevención en el filtrado de información ya que una decisión es revisada por varios equipos diferentes. Al no ser solo 1 persona es más dificil acceder a la información necesaria para causar daños a la empresa.
