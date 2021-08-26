---
title: Configuración de administración
description: Aprenda a configurar el área de administración de Adobe Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1966'
ht-degree: 36%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Ajustes de administración{#administration-setup}

Las pantallas de Configuración de administración sirven para administrar los usuarios de Adobe Dynamic Media Classic. Utilice estas pantallas para permitir a los usuarios trabajar en Adobe Dynamic Media Classic y comunicarse por correo electrónico con los usuarios.

1. Para acceder a las opciones de configuración de administración, vaya a **Configuración** > **Configuración personal** > **Configuración de administración**.

## Administración de usuarios {#user-administration}

A todos los usuarios de Adobe Dynamic Media Classic se les asigna una función que determina sus privilegios y derechos de acceso a las funciones de Adobe Dynamic Media Classic. Los administradores determinan las distintas funciones y responsabilidades para sus empresas.

Normalmente, Adobe Dynamic Media Classic configura el primer conjunto de empresas y asigna un administrador de empresa. A continuación, el administrador de la empresa configura y administra los usuarios de Dynamic Media Classic de Adobe.

Adobe Dynamic Media Classic admite varias funciones de usuario. Estas funciones pueden acceder a las empresas configuradas para Adobe Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UsuarioPuede acceder a las empresas a las que se les haya asignado; no puede realizar ninguna tarea administrativa.

**Adobe Dynamic Media Classic Company** AdminPuede ver y administrar solo sus propias empresas. También puede realizar todas las funciones de administración (incluida la adición de administradores y usuarios). Un administrador de la empresa puede agregar un usuario a las cuentas de administrador de la empresa DMC. (Esta función es la función de usuario predeterminada).

Después de agregar un usuario, Adobe Dynamic Media Classic envía un mensaje de correo electrónico de bienvenida al usuario. El mensaje incluye una contraseña y la URL de Adobe de Dynamic Media Classic.

### Agregar un usuario o administrador {#adding-a-user-or-administrator}

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de la administración]** > **[!UICONTROL Administración de usuarios]**.
1. Seleccione **[!UICONTROL Add]**.
1. Introduzca el nombre y la dirección de correo electrónico del usuario o administrador que desea añadir y, a continuación, seleccione **[!UICONTROL Next]**.

   >[!NOTE]
   >
   >El carácter de apóstrofo (`‘`) no está permitido en las direcciones de correo electrónico.

1. Para asignar una función al usuario, elija una opción de Función.

   Consulte [Adobe Funciones de usuario y privilegios de Dynamic Media Classic](administration-setup.md#user_administration).

1. Para agregar un usuario a una empresa, seleccione un nombre de empresa.
1. Si desea agregar el usuario a un grupo (si está agregando un usuario o colaborador de Media Portal), seleccione **[!UICONTROL Siguiente]** y agregue el usuario.
1. Seleccione **[!UICONTROL Guardar]** para completar la configuración del usuario.

   Después de guardar, se le preguntará si desea agregar un usuario a otra empresa. Seleccione **[!UICONTROL Agregar]** si desea agregar el usuario a una empresa.

   A todos los usuarios nuevos se les asigna una contraseña generada aleatoriamente; los usuarios deben cambiar las contraseñas la primera vez que inician sesión en la aplicación de escritorio de Adobe Dynamic Media Classic.

   Los nuevos usuarios reciben un correo electrónico de bienvenida una vez que se han agregado al sistema. El correo electrónico proporciona una contraseña temporal y explica cómo iniciar sesión en Adobe Dynamic Media Classic.

   Si el usuario no recibe el correo electrónico de bienvenida, pídale que vaya a la página de inicio de sesión de Adobe Dynamic Media Classic (https://s7sps1.scene7.com) y seleccione **[!UICONTROL Olvidé mi contraseña]**. La contraseña se restablece y se envía un nuevo mensaje de correo electrónico. Si el usuario no recibe el correo electrónico y no se encuentra en su carpeta de correo no deseado, póngase en contacto con el servicio de asistencia técnica.

   Al agregar nuevos usuarios de Media Portal, también puede ir a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Administración de usuarios]**, seleccionar **[!UICONTROL Cargar lista de usuarios]** y seleccionar un archivo .csv que no contenga más de 500 usuarios.

### Eliminación de un usuario {#deleting-a-user}

Puede eliminar usuarios del Adobe de Adobe Dynamic Media Classic invalidándolos. Los usuarios no válidos se eliminan del sistema y de todas las cuentas.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de la administración]** > **[!UICONTROL Administración de usuarios]**.
1. Seleccione un usuario de la lista y, a continuación, seleccione **[!UICONTROL Editar]**.
1. Anule la selección de Válido.
1. Seleccione **[!UICONTROL Guardar]**.

### Activar o desactivar usuarios {#activating-or-deactivating-users}

Los usuarios desactivados dejan de tener permiso para acceder a una cuenta que aparezca en la parte superior del menú para seleccionar cuentas a las que acceder.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de la administración]** > **[!UICONTROL Administración de usuarios]**.
1. En la lista de usuarios, seleccione o anule la selección de la opción **[!UICONTROL Active]** junto al nombre del usuario.

### Edición de información de usuario {#editing-user-information}

La información de usuario que puede modificar depende de su función como administrador y de la función que tenga asignada el usuario cuya información se desea editar. Las opciones que aparecen atenuadas (no disponibles) no son editables.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de la administración]** > **[!UICONTROL Administración de usuarios]**.
1. Seleccione un usuario de la lista y, a continuación, seleccione **[!UICONTROL Editar]**.
1. Seleccione la entrada en la tabla que muestra la empresa para la que intenta modificar permisos o acceso y, a continuación, seleccione **[!UICONTROL Administrar empresa]**.
1. Seleccione la función de usuario.
1. Si desea cambiar la pertenencia al grupo del usuario (si está editando o agregando un usuario o colaborador de Media Portal), seleccione **[!UICONTROL Siguiente]** y edite la pertenencia al grupo.
1. Seleccione **[!UICONTROL Guardar]**.

### Filtrado y ordenación de la lista de usuarios {#filtering-and-sorting-the-user-list}

Puede filtrar y ordenar la lista para buscar usuarios. Todos los usuarios de las cuentas que administra aparecen en la lista de los usuarios independientemente de la cuenta seleccionada en el menú de selección de cuenta a la que acceder.

Puede utilizar las siguientes técnicas de filtrado en la lista usuarios:

* **Filtrar por grupo** : seleccione el menú  **[!UICONTROL Por]** grupo y elija una opción para restringir la lista a los usuarios de un grupo.

* **Filtrar por función de usuario** : seleccione el menú  **[!UICONTROL Por]** usuario y elija una opción para restringir la lista a usuarios o administradores de distintos tipos.

* **Filtrar por nombre**  de campo: seleccione  **[!UICONTROL Activar filtro por campo]**. A continuación, seleccione el menú **[!UICONTROL By Field Name]**, elija una columna para filtrar la lista, seleccione el menú Filter Character y elija una letra. La lista se filtrará en una de las columnas según la letra elegida. Para ver la lista completa, anule la selección de la opción **[!UICONTROL Habilitar filtro por campo]**.

* **Filtrar usuarios**  no válidos: Anule la selección de  **[!UICONTROL Incluir no válido]**. En los resultados de búsqueda aparecerán solo los usuarios que están en el sistema. Los usuarios no válidos se han eliminado del sistema y las cuentas que administra.

* **Ordenar por encabezado de columna** : seleccione un encabezado para ordenar todos los usuarios por su estado, alfabéticamente por nombre, apellido o correo electrónico, por función de usuario o por estado válido/no válido.

Si tiene muchos usuarios, puede limitar el tamaño de la lista seleccionando un número en el menú Tamaño máximo de lista.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Ancho de banda y almacenamiento {#bandwidth-storage}

Los administradores de Adobe Dynamic Media Classic pueden generar ancho de banda, almacenamiento y otros tipos de informes para las empresas que administran. Estos informes están disponibles en la página Ancho de banda y almacenamiento .

Para abrir esta página, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**. Expanda **[!UICONTROL Administration Setup]** y, a continuación, seleccione **[!UICONTROL Bandwidth &amp; Storage]**.

### Tipos de informes {#types-of-reports}

En la tabla siguiente se describen los informes que se pueden generar desde la página Ancho de banda y almacenamiento:

| Informe | Información | Uso |
|:--- |:--- |:--- |
| Ancho de banda | Uso del ancho de banda por la empresa | Lleve un seguimiento del uso del ancho de banda por la empresa a lo largo de intervalos de fechas específicos para determinar patrones de tráfico. |
| Almacenamiento | Uso del almacenamiento | Lleve un seguimiento de la cantidad de datos que carga la empresa. |
| Contenido de imagen | Número de solicitudes de imágenes por tipo | Lleve un seguimiento del número de solicitudes y el volumen de los diferentes tipos de imágenes. |
| Dominio | El número de solicitudes de URL por dominio | Lleve un seguimiento del uso de imágenes según el dominio de la solicitud de imagen para una empresa concreta. (Adobe Dynamic Media Classic puede proporcionar más de un dominio por cuenta. Para obtener más información, póngase en contacto con el equipo de asistencia técnica). |
| Flujo continuo de vídeo | Uso del ancho de banda para el flujo continuo de vídeo | Lleve un seguimiento del uso del flujo continuo de vídeo por empresa a lo largo de intervalos de fechas específicos para determinar patrones de tráfico. |
| Contenido de vídeo | Tiempo de reproducción de distintos vídeos | Determine cuáles son los vídeos más vistos y menos vistos. |

El informe de contenido de imagen proporciona información acerca de las solicitudes para estos tipos de imágenes:

* **Solicitud de imagen** : solicitudes para imágenes.

* **Solicitud de miniaturas** : solicitudes de muestras o imágenes alternativas en los visualizadores.

* **Solicitud de máscara** : solicitudes para imágenes que devuelven máscaras de escala gris.

* **Solicitud de mosaico del visualizador** : solicitudes de imagen cargadas por un visualizador.

* **Solicitud de objeto Vnt** : solicitudes de renderización de imágenes que devuelven una imagen con objetos especificados en las viñetas solicitadas.

* **Solicitud de información de Vnt** : solicitudes de procesamiento de imágenes que devuelven información sobre las viñetas solicitadas.

>[!NOTE]
>
>El informe de flujo continuo de vídeo solo se aplica al flujo continuo de vídeos. No registra la visualización de vídeos progresivos.

### Generar un informe {#generating-a-report}

Siga estos pasos para generar un informe de ancho de banda, almacenamiento, contenido de imágenes, dominio, flujo continuo de vídeo o contenido de vídeo:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.
1. Expanda Configuración de administración y, a continuación, seleccione **[!UICONTROL Ancho de banda y almacenamiento]**.
1. Seleccione una pestaña: **[!UICONTROL Ancho de banda]**, **[!UICONTROL Almacenamiento]**, **[!UICONTROL Contenido de imagen]**, **[!UICONTROL Dominio]**, **[!UICONTROL Flujo de vídeo]** o **[!UICONTROL Contenido de vídeo]**.

   Consulte [Tipos de informes](administration-setup.md#types_of_reports).

### Ver datos de diferentes maneras {#viewing-data-in-different-ways}

Después de generar un informe en la página Ancho de banda y almacenamiento, puede elegir opciones para ver la información. Puede elegir cómo se presenta la información, ver la información en un diagrama o en una cuadrícula de datos, así como especificar un período de tiempo para la recopilación de información. En la vista Datos, también puede ordenar la información y reorganizar las columnas.

* **Ver datos en un gráfico o cuadrícula**  de datos: seleccione  **[!UICONTROL Vista]** de gráfico para ver los datos en un gráfico; seleccione  **[!UICONTROL Vista]** de datos para ver los datos en una cuadrícula de datos.

* **Elija un tipo de presentación de informe** : en el menú Tipo de informe, seleccione  **[!UICONTROL Resumen]**,  **[!UICONTROL Diario]** o  **** Mes para organizar los datos en forma de resumen, por día o por mes. No todos los informes ofrecen esta opción.

* **Especifique un período de tiempo** : elija opciones para definir un período de tiempo para el informe y, a continuación, seleccione  **** Actualizar después de definir un período de tiempo:

* **Período de tiempo predefinido** : en el menú Informe predefinido, elija una opción. Por ejemplo, elija Último mes para recopilar los datos del mes anterior.

* **Período de tiempo personalizado** : en el menú Informe predefinido, seleccione  **[!UICONTROL Personalizado]**. A continuación, elija una fecha en el menú **[!UICONTROL Mes de inicio]** (o **[!UICONTROL Fecha de inicio]**) y una fecha en el menú N.º de meses (o N.º de días). En el caso de informes de dominio y de contenido de vídeo, puede elegir una fecha inicial y final específica para capturar los datos del informe.

* **Ordenar datos (solo vista de datos)** : para ordenar la información en una columna, seleccione el encabezado de la columna. Seleccione de nuevo para ordenar en orden descendente.

* **Reorganizar columnas (solo vista de datos)** : para mover una columna a una ubicación diferente de la cuadrícula de datos, arrastre su encabezado.

### Exportación e impresión de informes {#exporting-and-printing-reports}

Después de generar un informe, puede exportar sus datos para utilizarlos en hojas de cálculo y en otras aplicaciones. También puede imprimir los informes.

* **Exportar datos del informe** : en la vista Datos, ordene y organice los datos según sea necesario. A continuación, abra el menú **[!UICONTROL Export]** y elija un formato: **[!UICONTROL Delimitado por tabulaciones]**, **[!UICONTROL Separado por comas]** o **[!UICONTROL HTML con formato]**. Los datos se copian en el portapapeles con el formato que elija. Ahora puede pegarlos en una hoja de cálculo o en una aplicación.

* **Imprimir un informe** : seleccione  **[!UICONTROL Imprimir]**, elija las opciones que desee en el cuadro de diálogo Imprimir y, a continuación, seleccione  **[!UICONTROL Aceptar]**.

## Errores de imagen {#image-errors}

Los administradores de Adobe Dynamic Media Classic pueden generar informes de errores de imagen. Estos informes proporcionan una lista de los 20 errores de imagen más frecuentes, en las últimas 24 horas, de la empresa en la que haya iniciado sesión en ese momento. Para generar un informe de error de imagen, haga lo siguiente:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.
1. Expanda Configuración de administración y, a continuación, seleccione **[!UICONTROL Errores de imagen]**.
1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * Para ordenar los errores por la información del encabezado, seleccione un encabezado. De manera predeterminada, los errores se ordenan, de mayor a menor, según el número de veces que aparecen.
   * Mueva el cursor sobre el campo Respuesta de un determinado error para ver el mensaje de error específico.
   * Para ver el vínculo a la página web de la imagen o del referente, mueva el cursor sobre el campo URL o el campo Referente .
   * Para copiar el vínculo a la imagen real, seleccione **[!UICONTROL URL Copy URL]**. Puede pegar este vínculo en una ventana del explorador para acceder a la imagen e investigar el error.
   * Para copiar el vínculo a la página web del referente, seleccione **[!UICONTROL URL de copia del referente]**.

Los errores mostrados pertenecen a la empresa en la que haya iniciado sesión en ese momento. Cada error incluye la siguiente información:

* **ID de imagen** : ID de la imagen ofensiva.

* **Hora** : intervalo de tiempo de la primera vez que se informó del error hasta la última vez que se notificó, en las últimas 24 horas.

* **Recuento** : el número de errores notificados en la imagen.

* **Respuesta** : el mensaje de error específico. Los errores son 4xx o 5xx.

* **URL** : enumera la dirección URL de la imagen en Adobe Dynamic Media Classic.

* **Referente** : especifica la dirección URL del sitio web del que provino la solicitud inicial. La referencia puede ser cualquier sitio web que tenga un vínculo a la imagen.

Las columnas URL y Referencia tienen asociada la opción Copiar URL para simplificar el proceso de prueba.
