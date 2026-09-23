# Memoria de prueba de restricción de acceso a dispositivos USB

## Objetivo

El objetivo de esta prueba fue comprobar que las restricciones de acceso a dispositivos USB se aplican correctamente a usuarios estándar de Windows sin privilegios administrativos.

Para realizar la validación, se creó un usuario regular y se comprobó su comportamiento al intentar acceder a un dispositivo USB conectado a la máquina virtual.

---

## Creación del usuario estándar

Se creó un nuevo usuario local en Windows desde:

> **Configuración > Cuentas > Familia y otros usuarios**

Durante el proceso se seleccionó la opción de crear un usuario sin cuenta de Microsoft.

El usuario fue configurado como una **cuenta estándar**, sin privilegios administrativos.

Para comprobar que la cuenta no pertenecía al grupo de administradores, se revisaron los grupos y usuarios con privilegios del sistema.

---

## Prueba de acceso al dispositivo USB

Una vez creado el usuario estándar, se realizaron los siguientes pasos:

1. Se cerró la sesión del usuario anterior.
2. Se inició sesión con la nueva cuenta estándar.
3. Se conectó el dispositivo USB a la máquina virtual mediante VirtualBox.
4. Se comprobó que el dispositivo estaba disponible en el sistema.
5. Se intentó acceder a su contenido utilizando la cuenta estándar.

---

## Verificación de la restricción

La prueba consistió en comprobar si el usuario estándar podía acceder al dispositivo USB.

La política aplicada debía impedir el acceso al dispositivo para usuarios sin los permisos necesarios.

Al intentar acceder al dispositivo, el sistema debía:

- Denegar la operación.
- Mostrar un mensaje de acceso restringido.
- Impedir el uso del dispositivo.

De esta forma, se comprobó que la restricción de acceso se aplicaba en función de los permisos del usuario.

---
