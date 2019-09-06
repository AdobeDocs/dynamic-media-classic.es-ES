---
title: Ajustes de administración
seo-title: Ajustes de administración
description: nulo
seo-description: Descubra cómo configurar el área de administración de Dynamic Media Classic.
uuid: 16 ba 9 fed-b 5 c 6-4991-83 b 3-8 d 7 d 7129013 a
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 3 c 9 ee 4 ec-dd 37-498 d -98 d 6-1339 b 80177 ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Ajustes de administración{#administration-setup}

Las pantallas Ajustes de administración sirven para administrar los usuarios de Scene7 Publishing System. Utilice estas pantallas para permitir a los usuarios trabajar en Scene7 Publishing System y para comunicarse con los usuarios por correo electrónico.

1. To access Administration Setup options, click **Setup** &gt; **Personal Setup** &gt; **Administration Setup**.

## Administración de usuarios {#user-administration}

A todos los usuarios de Dynamic Media Classic se les asigna una función que determina sus privilegios y derechos de acceso a las funciones de Scene 7 Publishing System. Los administradores determinan las distintas funciones y responsabilidades para sus empresas.

Normalmente, Dynamic Media Classic configura el primer conjunto de empresas y asigna un administrador de empresa. A continuación, el administrador de empresa configura y administra los usuarios de Scene7 Publishing System.

Scene7 Publishing System admite tres funciones de usuario. Las tres funciones de usuario pueden acceder a la configuración de empresas de Scene7 Publishing System:

**Administrador de SPS** Puede ver y administrar todas las funciones de Scene 7 Publishing System, así como configurar empresas y agregar administradores y usuarios.

**Administrador de empresa** Puede ver y administrar solo sus propias empresas. También puede realizar todas las funciones de administración (incluida la adición de administradores y usuarios). El administrador de empresa puede añadir usuarios a las cuentas de administración de la empresa de SPS. (Esta función es la función de usuario predeterminada).

**El usuario** de SPS puede acceder a las empresas a las que se les ha asignado; no puede realizar ninguna tarea administrativa.

Tras añadir un usuario, Scene7 Publishing System le envía un mensaje de correo electrónico de bienvenida. Este mensaje incluye una contraseña y la URL de Scene7 Publishing System.

### Adición de un usuario o administrador {#adding-a-user-or-administrator}

1. Haga clic en Configuración &gt; Ajustes de aplicación &gt; Ajustes de administración &gt; Administración de usuarios.
1. Haga clic en Agregar. 
1. Introduzca el nombre y la dirección de correo electrónico del usuario o administrador que desea agregar y, a continuación, haga clic en Siguiente.

   >[!NOTE]
   >
   >El carácter apóstrofe (') no está permitido en las direcciones de correo electrónico.

1. Elija la función que desea asignar al usuario.

   Consulte [Funciones y privilegios de usuario de Dynamic Media Classic](administration-setup.md#user_administration).

1. Seleccione un nombre de empresa para agregar un usuario a una empresa.
1. Si desea agregar el usuario a un grupo (si está agregando un usuario o colaborador de Media Portal), haga clic en Siguiente y agregue el usuario.
1. Haga clic en Guardar para completar la configuración de usuario.

   Después de guardar, se le preguntará si desea agregar un usuario a otra empresa. Haga clic en Agregar si desea agregar el usuario a una empresa.

   Todos los nuevos usuarios reciben una contraseña generada al azar; los usuarios deben cambiar su contraseña la primera vez que inicien sesión en Scene7 Publishing System.

   Los nuevos usuarios reciben un correo electrónico de bienvenida una vez que se han agregado al sistema. El correo electrónico proporciona una contraseña temporal y explica cómo se debe iniciar sesión en Scene7 Publishing System.

   Si el usuario no recibe el correo electrónico de bienvenida, póngalo en la página de inicio de sesión de SPS (https://s7sps1.scene7.com) y haga clic en Olvidé mi contraseña. La contraseña se restablece y se envía un nuevo mensaje de correo electrónico. Si el usuario no recibe el correo electrónico y no se encuentra en su carpeta de correo no deseado, póngase en contacto con el servicio de asistencia técnica.

   Al agregar nuevos usuarios del Media Portal, también puede ir a Ajustes &gt; Ajustes de aplicación &gt; Administración de usuarios y, a continuación, hacer clic en Cargar lista de usuarios y seleccionar un archivo .csv con un máximo de 500 usuarios.

### Eliminación de un usuario {#deleting-a-user}

Puede eliminar usuarios de Scene7 Publishing System marcándolos como no válidos. Los usuarios no válidos se eliminan del sistema y de todas las cuentas.

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. Seleccione un usuario de la lista y haga clic en **Editar**.
1. Anule la selección de Válido.
1. Haga clic en **Guardar**.

### Activación o desactivación de usuarios {#activating-or-deactivating-users}

Los usuarios desactivados dejan de tener permiso para acceder a una cuenta que aparezca en la parte superior del menú para seleccionar cuentas a las que acceder.

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. En la lista de usuarios, seleccione o anule la selección de la opción Activar que aparece junto al nombre del usuario.

### Edición de la información de usuario {#editing-user-information}

La información de usuario que puede modificar depende de su función como administrador y de la función que tenga asignada el usuario cuya información se desea editar. Las opciones que aparecen atenuadas (no disponibles) no son editables.

1. Vaya a **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. Seleccione el usuario y haga clic en **Editar**.
1. Seleccione la entrada en la tabla que muestra la empresa para la que está intentando modificar los permisos o acceso y, a continuación, haga clic en el vínculo Gestionar empresa.
1. Seleccione la función de usuario.
1. Si desea cambiar la membresía del grupo del usuario (si está editando o agregando un usuario o colaborador de Media Portal), haga clic en Siguiente y edite la membresía del grupo.
1. Haga clic en **Guardar**.

### Filtrado y ordenación de la lista de usuarios {#filtering-and-sorting-the-user-list}

Puede filtrar y ordenar la lista para buscar usuarios. Todos los usuarios de las cuentas que administra aparecen en la lista de los usuarios independientemente de la cuenta seleccionada en el menú de selección de cuenta a la que acceder.

Puede utilizar las siguientes técnicas de filtrado en la lista usuarios:

**Filtrar por grupo** Seleccione el menú Por grupo y elija una opción para reducir la lista a los usuarios de un grupo.

**Filtrar por función** de usuario Seleccione el menú Por función de usuario y elija una opción para reducir la lista a usuarios o administradores de distintos tipos.

**Filtrar por nombre de campo** Seleccione la opción Activar filtración por campo. A continuación, en el menú Por nombre de campo, seleccione la columna con la que desea filtrar la lista y elija una letra en el menú de caracteres de filtro. La lista se filtrará en una de las columnas según la letra elegida. Para volver a ver la lista completa desactive la opción Activar filtración por campos.

**Desactive los usuarios no válidos** anulando la selección de la opción Incluir no válido. En los resultados de búsqueda aparecerán solo los usuarios que están en el sistema. Los usuarios no válidos se han eliminado del sistema y las cuentas que administra.

**Ordenar por encabezado de columna** Haga clic en un encabezado para ordenar todos los usuarios por su estado, alfabéticamente por nombre, apellidos, correo electrónico, función de usuario o por estado válido/no válido.

Si tiene muchos usuarios, puede limitar el tamaño de la lista seleccionando un número en el menú Tamaño máximo de lista.

### Vinculación de identidad de usuario de IMS a una cuenta de usuario de Dynamic Media Classic IPS {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Puede vincular una identidad de usuario de Adobe IMS a una cuenta de usuario de Dynamic Media Classic IPS para poder utilizar SSO (inicio único) para iniciar sesión e iniciar Scene 7 Publishing System desde Adobe Marketing Cloud.

1. Adobe ya debe haber configurado su cuenta con una organización de Adobe Marketing Cloud y vincularla al contexto de producto de Scene 7 Publishing System. Si esta configuración aún no se ha realizado o no está seguro de si se ha realizado, póngase en contacto con el Servicio de atención al cliente de Adobe.

   Una vez finalizada la instalación, puede iniciar sesión en Adobe Marketing Cloud y vincular su identidad de Adobe Marketing Cloud a la cuenta de usuario de Dynamic Media Classic haciendo lo siguiente.

1. En Adobe Marketing Cloud, vaya a la configuración de su cuenta.
1. Haga clic **en Administrar organizaciones**.
1. Haga clic **en Vincular cuenta** o **Obtener acceso**.
1. Seleccione **Experience Manager** y, a continuación, escriba sus credenciales.

   Sus credenciales incluyen la región de la empresa de IPS, la dirección de correo electrónico y la contraseña.

1. Haga clic **en Vincular**.
1. Una vez configurado el vínculo, puede iniciar Scene 7 Publishing System desde Adobe Marketing Cloud, o bien puede iniciarlo directamente.

   Realice una de las siguientes acciones:

   * Para iniciar Dynamic Media Classic desde Adobe Marketing Cloud, en la barra izquierda de Adobe Marketing Cloud, haga clic **en Soluciones** &gt; **Experience Manager**. En la tarjeta de Dynamic Media Classic, haga clic **en Iniciar**.
   * Para iniciar sesión directamente en Scene 7 Publishing System con sus credenciales IMS, utilice el siguiente sitio web:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Sustituya «N» en la ruta anterior por el número de su región de empresa de IPS. Es decir, N = 1 para Norteamérica; 3 para EMEA; o 5 para JAPAC.

## Ancho de banda y almacenamiento {#bandwidth-storage}

Los administradores de SPS pueden generar informes sobre el ancho de banda, el almacenamiento y otros tipos de informes para las empresas que administran. Los informes están disponibles en la pantalla Ancho de banda y almacenamiento.

Para abrir esta pantalla, haga clic en Ajustes &gt; Ajustes personales. Expanda Ajustes de administración y, a continuación, haga clic en Ancho de banda y almacenamiento.

### Tipos de informes {#types-of-reports}

La tabla siguiente describe los informes que se pueden generar en la pantalla Ancho de banda y almacenamiento:

| Informe | Información | Uso |
|:--- |:--- |:--- |
| Ancho de banda | Uso del ancho de banda por la empresa | Lleve un seguimiento del uso del ancho de banda por la empresa a lo largo de intervalos de fechas específicos para determinar patrones de tráfico. |
| Almacenamiento | Uso del almacenamiento | Lleve un seguimiento de la cantidad de datos que carga la empresa. |
| Contenido de imagen | Número de solicitudes de imágenes por tipo | Lleve un seguimiento del número de solicitudes y el volumen de los diferentes tipos de imágenes. |
| Dominio | El número de solicitudes de URL por dominio | Lleve un seguimiento del uso de imágenes según el dominio de la solicitud de imagen para una empresa concreta. (Dynamic Media Classic puede proporcionar más de un dominio por cuenta. Para obtener más información, póngase en contacto con el equipo de asistencia técnica). |
| Flujo continuo de vídeo | Uso del ancho de banda para el flujo continuo de vídeo | Lleve un seguimiento del uso del flujo continuo de vídeo por empresa a lo largo de intervalos de fechas específicos para determinar patrones de tráfico. |
| Contenido de vídeo | Tiempo de reproducción de distintos vídeos | Determine cuáles son los vídeos más vistos y menos vistos. |


El informe de contenido de imagen proporciona información acerca de las solicitudes para estos tipos de imágenes:

**Solicitudes de** solicitud de imagen para imágenes.

**Solicitudes de solicitud** de miniatura para muestras o imágenes alternativas en visores.

**Solicitudes de solicitud** de máscara a imágenes que devuelven máscaras en escala de grises.

**Solicitudes** de imagen de mosaico de visor cargado por un visor.

**Solicitudes de solicitud de objeto Vnt Request** que devuelven una imagen con objetos especificados en las viñetas solicitadas.

**Solicitudes de procesamiento** de imágenes de solicitud de información Vnt que devuelven información relativa a las viñetas solicitadas.

>[!NOTE]
>
>El informe de flujo continuo de vídeo solo se aplica al flujo continuo de vídeos. No registra la visualización de vídeos progresivos.

### Generación de un informe {#generating-a-report}

Siga estos pasos para generar un informe de ancho de banda, almacenamiento, contenido de imágenes, dominio, flujo continuo de vídeo o contenido de vídeo:

1. Seleccione Ajustes &gt; Ajustes personales.
1. Expanda Ajustes de administración y, a continuación, haga clic en Ancho de banda y almacenamiento.
1. Haga clic en una ficha: Ancho de banda, Almacenamiento, Contenido de la imagen, Dominio, Flujo continuo de vídeo o Contenido de vídeo.

   Consulte [Tipos de informes](administration-setup.md#types_of_reports).

### Visualización de datos con distintos métodos {#viewing-data-in-different-ways}

Después de generar un informe en la página Ancho de banda y almacenamiento, puede elegir opciones para ver la información. Puede elegir cómo se presenta la información, ver la información en un diagrama o en una cuadrícula de datos, así como especificar un período de tiempo para la recopilación de información. En la vista Datos, también puede ordenar la información y reorganizar las columnas.

**Visualización de datos en un diagrama o cuadrícula** de datos Haga clic en la opción Vista de gráfico para ver los datos en un gráfico; haga clic en la opción Vista de datos para ver los datos en una cuadrícula de datos.

**Elección de un tipo de presentación de informe** En el menú Tipo de informe, elija Resumen, Diario o Mensual para organizar los datos en forma resumida, por día o por mes. No todos los informes ofrecen esta opción.

**Especificación de un período** de tiempo Elija opciones para definir un período de tiempo para el informe y, a continuación, haga clic en Actualizar después de definir un período de tiempo:

**Período de tiempo predefinido** En el menú Informe predefinido, elija una opción. Por ejemplo, elija Último mes para recopilar los datos del mes anterior.

**Período de tiempo personalizado** en el menú Informe predefinido, seleccione Personalizado. A continuación, elija una fecha en el menú Mes de inicio (o Fecha de inicio) y otra fecha en el menú N.º de meses (o N.º de días). En el caso de informes de dominio y de contenido de vídeo, puede elegir una fecha inicial y final específica para capturar los datos del informe.

**Ordenar datos (solo vista de datos)** Para ordenar la información de una columna, haga clic en el encabezado de la columna. Haga clic de nuevo para cambiar al orden descendente.

**Reorganización de columnas (solo vista de datos)** Para mover una columna a una ubicación diferente en la cuadrícula de datos, arrastre su encabezado.

### Exportación e impresión de informes {#exporting-and-printing-reports}

Después de generar un informe, puede exportar sus datos para utilizarlos en hojas de cálculo y en otras aplicaciones. También puede imprimir los informes.

**Exportación de datos del informe** en la vista Datos, ordene y organice los datos según sea necesario. A continuación, abra el menú Exportar y elija un formato: Delimitado por tabuladores, Separado por comas o HTML formateado. Los datos se copian en el portapapeles con el formato que elija. Ahora puede pegarlos en una hoja de cálculo o en una aplicación.

**Impresión de un informe** Haga clic en Imprimir, elija las opciones que desee en el cuadro de diálogo Imprimir y, a continuación, haga clic en Aceptar.

## Errores de imagen {#image-errors}

Los administradores de SPS pueden generar informes de errores de imagen. Estos informes proporcionan una lista de los 20 errores de imagen más frecuentes, en las últimas 24 horas, de la empresa en la que haya iniciado sesión en ese momento. Siga estos pasos para generar un informe de errores de imagen:

1. Haga clic en Ajustes &gt; Ajustes personales.
1. Expanda Ajustes de administración y, a continuación, haga clic en Errores de imagen.
1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * Haga clic en un encabezado para ordenar los errores según la información del encabezado. De manera predeterminada, los errores se ordenan, de mayor a menor, según el número de veces que aparecen.
   * Mueva el cursor sobre el campo Respuesta de un determinado error para ver el mensaje de error específico.
   * Mueva el cursor sobre el campo URL o el campo Referencia para ver el vínculo de la imagen o la página web de referencia.
   * Haga clic en Copiar URL de la columna URL para copiar el vínculo a la imagen real. Puede pegar este vínculo en una ventana del explorador para acceder a la imagen e investigar el error.
   * Haga clic en Copiar URL de la columna Referencia para copiar el vínculo a la página web de referencia.

Los errores mostrados pertenecen a la empresa en la que haya iniciado sesión en ese momento. Cada error incluye la siguiente información:

**ID de ID** de imagen para la imagen que ocasiona el error.

**Time** El intervalo de tiempo de la primera vez que se informó el error a la última vez que se informó el error, durante las últimas 24 horas.

**Recuento** El número de errores informados en la imagen.

**Respuesta** El mensaje de error específico. Los errores son 4xx o 5xx.

**Las URL** enumeran la URL de la imagen en Scene 7.

**Referente** Especifica la URL del sitio Web de donde procede la solicitud inicial. La referencia puede ser cualquier sitio web que tenga un vínculo a la imagen.

Las columnas URL y Referencia tienen asociada la opción Copiar URL para simplificar el proceso de prueba.
