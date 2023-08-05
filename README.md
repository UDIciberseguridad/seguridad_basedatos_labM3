# seguridad_basedatos_labM3
## Instrucciones
El resultado del laboratorio consiste en:
Documento en formato Word que incluye:
Página de presentación con los datos del estudiante.
El laboratorio consiste en la implementación de diferentes medidas de seguridad en un servidor SQL Server Express el cual debe ser instalado en una computadora. Por temas de facilidad se recomienda completar el laboratorio en una computadora con Windows 10 o Windows 11.  En caso que el estudiante desee instalar el Windows Server Express en otro sistema operativo, puede hacerlo, pero debe buscar por su cuenta las instrucciones de como completar cada paso.
El estudiante también debe instalar el software SQL Server Management Studio.
Se debe incluir una explicación de cada medida de seguridad a implementar y cuál es el beneficio que se busca lograr con cada medida. Para lograr completar cada medida se deben seguir cada paso descrito. Se deben incluir capturas de pantalla para documentar el proceso.
1.	Configurar la autenticación fuerte:
•	Ir a la carpeta "Seguridad" en el Explorador de objetos de SQL Server Management Studio.
•	Haga clic con el botón derecho del ratón en "Inicios de sesión" y seleccione "Nuevo inicio de sesión".
•	Seleccione la opción "Windows Authentication" y proporcione el nombre de usuario y la contraseña correspondientes.
•	En la sección "Opciones de inicio de sesión", seleccione "Enforce password policy" y "Enforce password expiration".
•	Haga clic en "Aceptar" para guardar los cambios.

2.	Configurar el firewall de Windows: Configurar el firewall de Windows:
•	Ir al Panel de control de Windows y seleccione "Firewall de Windows".
•	Haga clic en "Configuración avanzada" y seleccione "Reglas de entrada".
•	Seleccione "Nueva regla" y seleccione "Puerto" como tipo de regla.
•	Especifique el número de puerto utilizado por SQL Server (por defecto, el puerto es 1433).
•	Seleccione "Permitir la conexión" y haga clic en "Siguiente".
•	Seleccione "Todos" para aplicar la regla a cualquier dirección IP y haga clic en "Siguiente".
•	Proporcione un nombre para la regla y haga clic en "Finalizar".

3.	Configurar la encriptación de datos:
•	Ir a la carpeta "Seguridad" en el Explorador de objetos de SQL Server Management Studio.
•	Haga clic con el botón derecho del ratón en "Certificados" y seleccione "Nuevo certificado".
•	Seleccione "Crear un certificado autofirmado" y especifique un nombre para el certificado.
•	Seleccione "Añadir" en la sección "Contenido protegido".
•	Seleccione las tablas o columnas que desea encriptar y haga clic en "Aceptar".
•	Seleccione "Añadir" en la sección "Destinatarios de la clave".
•	Seleccione la cuenta de servicio de SQL Server y haga clic en "Aceptar".
•	Seleccione "Aceptar" para crear el certificado.


4.	Configurar la auditoría de seguridad
•	Ir a la carpeta "Seguridad" en el Explorador de objetos de SQL Server Management Studio.
•	Haga clic con el botón derecho del ratón en "Auditorías" y seleccione "Nueva auditoría".
•	Proporcione un nombre para la auditoría y seleccione la opción "Escribir en un archivo".
•	Seleccione la ubicación del archivo de auditoría y haga clic en "Aceptar".
•	Haga clic con el botón derecho del ratón en la auditoría y seleccione "Propiedades".
•	Seleccione la opción "Eventos de auditoría" y seleccione los eventos que desea auditar (por ejemplo, inicio de sesión, intentos fallidos de inicio de sesión, cambios en permisos, etc.).
•	Haga clic en "Aceptar" para guardar la configuración.

5.	Configurar las políticas de contraseñas:
•	Abra el Editor de directivas de seguridad local de Windows (se puede acceder a él a través del Panel de control).
•	Seleccione "Directivas de cuenta" y luego "Directivas de contraseña".
•	Configure las políticas de contraseña según sus necesidades. Por ejemplo, puede establecer una longitud mínima de contraseña, requerir caracteres especiales y números, y especificar un período de expiración de la contraseña.
•	Haga clic en "Aceptar" para guardar los cambios.

6.	Configurar el cifrado de red:
•	Abra el Administrador de configuración de SQL Server.
•	Seleccione "Configuración de red de SQL Server".
•	Seleccione la instancia de SQL Server que desea configurar.
•	Seleccione "Protocolos de red" y luego "TCP/IP".
•	Seleccione la pestaña "Cifrado" y configure las opciones de cifrado según sus necesidades.
•	Haga clic en "Aceptar" para guardar los cambios.

 
