# Configuración de excepciones de acceso a dispositivos USB

## Objetivo

El objetivo de esta práctica fue configurar una política de restricción de acceso a dispositivos USB para usuarios estándar y, posteriormente, crear una excepción para un usuario concreto.

La finalidad era comprobar que:

- Los usuarios estándar sin excepción no pudieran acceder al dispositivo USB.
- Un usuario estándar específico pudiera utilizar el USB sin necesidad de pertenecer al grupo de administradores.

---

## Preparación de los usuarios

Se utilizó una cuenta con privilegios administrativos para realizar la configuración de las políticas.

Además, se crearon tres cuentas de usuario estándar:

- **USB_Permitido**
- **Usuario estándar 1**
- **Usuario estándar 2**

Los tres usuarios permanecieron como cuentas estándar, sin pertenecer al grupo de administradores.

La cuenta **USB_Permitido** se utilizó como usuario de excepción, mientras que los otros dos usuarios se utilizaron para comprobar que la restricción general seguía aplicándose correctamente.

---

## Configuración de la política para usuarios no administradores

Desde la cuenta administradora se abrió **Microsoft Management Console (MMC)**.

Se añadió el complemento:

> **Editor de objetos de directiva de grupo**

Posteriormente, se seleccionó la directiva correspondiente a:

> **No administradores**

Dentro de la consola se accedió a la siguiente ruta:

> **Configuración de usuario > Plantillas administrativas > Sistema > Acceso de almacenamiento extraíble**

Se configuraron como **Habilitadas** las siguientes políticas:

- **Discos extraíbles: denegar acceso de lectura**
- **Discos extraíbles: denegar acceso de escritura**

Con esta configuración, los usuarios estándar quedaron sin permisos para leer o escribir datos en dispositivos USB de almacenamiento extraíble.

---

## Configuración de la excepción para un usuario específico

Después de aplicar la restricción general, se creó una política específica para el usuario:

> **USB_Permitido**

Desde MMC se volvió a añadir el complemento **Editor de objetos de directiva de grupo**, seleccionando esta vez directamente al usuario **USB_Permitido**.

Se accedió de nuevo a:

> **Configuración de usuario > Plantillas administrativas > Sistema > Acceso de almacenamiento extraíble**

Para este usuario se configuraron como **Deshabilitadas** las siguientes políticas:

- **Discos extraíbles: denegar acceso de lectura**
- **Discos extraíbles: denegar acceso de escritura**

De esta forma, el usuario **USB_Permitido** quedó excluido de la restricción general aplicada a los usuarios no administradores.

---

## Aplicación de las políticas

Una vez configuradas las políticas, se actualizaron las directivas del sistema mediante:

```cmd
gpupdate /force
