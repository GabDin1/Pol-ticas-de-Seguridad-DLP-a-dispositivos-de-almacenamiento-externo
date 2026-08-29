# Prevención de filtraciones

Para evitar la filtración de datos sensibles, la organización debe aplicar diferentes medidas de protección dependiendo de cómo se almacene, utilice o transmita la información.

Dos de los principales mecanismos utilizados son el **cifrado** y las herramientas de **Data Loss Prevention (DLP)**.

## Cifrado de la información

El cifrado permite proteger la información transformándola en un formato que no puede ser interpretado sin disponer de la clave necesaria.

De esta forma, aunque una persona no autorizada consiga acceder físicamente a un dispositivo o copiar determinados archivos, no podrá leer su contenido si estos se encuentran correctamente cifrados.

El cifrado puede aplicarse en diferentes situaciones:

* **Datos en reposo:** archivos almacenados en discos duros, servidores, bases de datos o dispositivos USB.
* **Datos en movimiento:** información enviada a través de la red.
* **Dispositivos extraíbles:** unidades USB utilizadas para transportar información sensible.

Por ejemplo, los dispositivos USB corporativos utilizados para transportar documentación sensible podrían estar cifrados mediante tecnologías como BitLocker To Go.

## Uso de herramientas DLP

Las herramientas DLP permiten detectar información sensible y controlar las acciones que los usuarios realizan sobre ella.

Una política DLP puede establecer reglas para acciones como:

* Copiar archivos sensibles a dispositivos USB.
* Enviar información mediante correo electrónico.
* Subir documentos a servicios de almacenamiento en la nube.
* Copiar información entre aplicaciones.
* Imprimir documentos sensibles.
* Compartir información fuera de la organización.

Dependiendo de la política establecida, la herramienta puede:

* Permitir la acción.
* Permitirla y registrarla.
* Generar una alerta.
* Solicitar una justificación.
* Bloquear la transferencia.

Por ejemplo, si un trabajador autorizado necesita copiar un documento sensible a un USB corporativo cifrado, la política DLP puede permitir la operación y registrar la transferencia.

En cambio, si intenta copiar ese mismo documento a un dispositivo USB personal no autorizado, la política podría bloquear la operación y generar una alerta para el equipo de Seguridad.

## Combinación de cifrado y DLP

El cifrado y DLP cumplen funciones diferentes pero complementarias.

El sistema DLP controla **cómo puede utilizarse o transferirse la información**, mientras que el cifrado protege **el contenido de los datos en caso de que estos sean obtenidos por una persona no autorizada**.

Por tanto, una política de prevención de filtraciones puede establecer que:

* Los datos sensibles deben almacenarse cifrados.
* Las transferencias de información sensible deben realizarse mediante canales seguros.
* Los dispositivos USB utilizados para transportar información sensible deben ser corporativos y estar cifrados.
* Las soluciones DLP deben monitorizar y controlar las transferencias de datos.
* Los intentos de transferencia no autorizados deben quedar registrados y, dependiendo del riesgo, ser bloqueados o generar una alerta.

La combinación de estas medidas reduce el riesgo de que la información sensible pueda abandonar la organización o ser utilizada por personas no autorizadas.
