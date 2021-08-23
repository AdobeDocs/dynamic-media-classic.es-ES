---
title: Agregar y administrar usuarios de Media Portal
description: Aprenda a añadir y administrar usuarios de Media Portal en Dynamic Media Classic.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Colaboración,Administración de activos
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 58%

---

# Agregar y administrar usuarios de Media Portal{#adding-and-managing-media-portal-users}

Como administrador puede añadir y administrar a los usuarios, decidir si pueden cambiar las contraseñas, editar su información y cargar listas de usuarios. Estas tareas se realizan desde la pantalla Administración de usuarios. Para acceder a esta pantalla, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de administración]** > **[!UICONTROL Administración de usuarios]**.

>[!NOTE]
>
>antes de agregar usuarios tendrá que configurar grupos para administrarlos. Media Portal no permite agregar un usuario sin asignarlo a uno o varios grupos. Para obtener más información, consulte [Crear y administrar grupos de Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administración de contraseñas de Media Portal {#handling-media-portal-passwords}

A los usuarios, colaboradores y usuarios colaboradores de Media Portal se les envía un mensaje de correo electrónico de bienvenida con una contraseña cuando usted los registra. Los administradores pueden decidir si los usuarios de Media Portal pueden cambiar esta contraseña.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de Media Portal]** > **[!UICONTROL Configuración general]**.
1. En la pantalla Configuración general, marque o desmarque la opción **[!UICONTROL Permitir que el usuario de Media Portal cambie la contraseña]**.
1. Seleccione **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Los usuarios de Media Portal que pueden cambiar contraseñas pueden hacerlo seleccionando **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]** y cambiando las contraseñas en la pantalla Configuración personal.

## Agregar un usuario de Media Portal {#adding-a-media-portal-user}

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de administración]** > **[!UICONTROL Administración de usuarios]**.
1. En la página Administración de usuarios, seleccione **Agregar**.
1. En el cuadro de diálogo Agregar usuario, en el panel Información de usuario, introduzca el nombre, los apellidos y la dirección de correo electrónico del usuario y, a continuación, seleccione **[!UICONTROL Siguiente]**.
1. En el panel Empresa/Función, en la lista desplegable de empresas, seleccione una o varias empresas para el usuario.
1. En la lista Rol, seleccione una función de Media Portal y, a continuación, seleccione **[!UICONTROL Siguiente]**.

   Consulte [Funciones de usuario en Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. En el panel Grupos de acceso, seleccione uno o varios grupos.

   Consulte [Crear y administrar grupos de Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Seleccione **[!UICONTROL Configuración de correo electrónico]** para elegir la configuración de correo electrónico diferente de la predeterminada.

   Consulte [Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Seleccione **[!UICONTROL Agregar usuario]**.

Tras añadir un usuario, Media Portal envía al usuario un mensaje de correo electrónico de bienvenida. El mensaje incluye una contraseña temporal y la dirección URL de Media Portal.

## Carga de una lista de usuarios de Media Portal {#uploading-a-media-portal-user-list}

Si desea agregar varios usuarios, puede cargar una lista de usuarios. Los usuarios se añaden automáticamente a la cuenta seleccionada.

Cree una lista de usuarios en un archivo CSV (valores separados por comas) que contenga la información de usuario. Una vez se haya cargado el archivo, los usuarios de la lista se añaden automáticamente a la cuenta con las asignaciones de grupo que se han especificado. Todos los usuarios nuevos reciben un mensaje de correo electrónico de bienvenida. En este mensaje se incluye un vínculo a Media Portal y una contraseña temporal.

### Creación de un archivo CSV {#creating-the-csv-file}

Cree un archivo CSV (nombrearchivo.csv) conforme al formato y los campos que se indican a continuación. La primera fila debe contener los encabezados de columna que aparecen en esta tabla. Puede ordenar las columnas como desee. Todas las columnas son obligatorias.

| Nombre de columna | Descripción |
|--- |--- |
| Nombre | El nombre. |
| Apellidos | Los apellidos. |
| Correo electrónico | Una dirección de correo electrónico válida. |
| Contraseña | Contraseña con distinción entre mayúsculas y minúsculas. |
| Función de usuario | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUsuario |
| Grupos | Lista de una o varias asignaciones de grupos de cuentas de cada usuario, separadas por comas. Debe especificar el grupo, agregando como prefijo el nombre de cuenta, separado por la barra diagonal (/). Por ejemplo, PortalCo/IT, donde PortalCo es la cuenta e IT es el grupo dentro de la cuenta PortalCo. |

La siguiente hoja de cálculo de ejemplo muestra cómo diseñar un archivo CSV:

| Nombre | Apellidos | Correo electrónico | Contraseña | Función de usuario | Grupos |
|--- |--- |--- |--- |--- |--- |
| Prairie | Kat | `prairiek@company.com` | bienvenido | Administrador de Media Portal | CoPortal/TI,CoPortal/Admin |
| Rick | Abandonos | `rickb@myco.com` | bienvenido | Usuario de Media Portal | PortalCo/GrupoMarketing, PortalCo/prueba |

### Carga de un archivo CSV {#uploading-the-csv-file}

1. Abra la pantalla de ajuste Administración de usuarios.
1. Seleccione **[!UICONTROL Cargar lista de usuarios]**.
1. En el cuadro de diálogo Seleccionar archivo para cargar, seleccione el archivo CSV y, a continuación, seleccione **[!UICONTROL Abrir]**.

Se añaden automáticamente los usuarios de la lista a los grupos especificados y se envía un mensaje de correo electrónico de bienvenida.

>[!NOTE]
>
>Si el archivo CSV no tiene el formato correcto, aparece el mensaje de error &quot;Se ha producido un error al procesar el archivo CSV cargado. Compruebe si los datos del archivo son válidos&quot;. Además, si el archivo CSV contiene un usuario de IP o IPS existente, éste no se añade a la lista de usuarios.

## Generación de una lista seleccionable de usuarios de Media Portal {#generating-a-selectable-list-of-media-portal-users}

Puede ver los nombres y las direcciones de correo electrónico de los usuarios de Media Portal en una ventana emergente. Esta lista resulta útil para cortar y pegar nombres y direcciones de correo electrónico de usuarios y usarlos en otra aplicación distinta a Media Portal.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de administración]** > **[!UICONTROL Administración de usuarios]**.
1. En la lista desplegable **[!UICONTROL By User Role]**, elija el nombre de una función de usuario de Media Portal y seleccione **[!UICONTROL Refresh]** para mostrar los nombres de una clase de usuario de Media Portal.
1. Seleccione **[!UICONTROL Lista emergente]**. Copie y pegue esta lista.

## Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Puede enviar un mensaje de correo de bienvenida cuando agregue usuarios, colaboradores y usuarios colaboradores de Media Portal. Puede configurar este mensaje de correo electrónico o indicar a Dynamic Media Classic que no lo envíe.

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de administración]** > **[!UICONTROL Administración de usuarios]**.
1. En la pantalla Configuración de administración de usuarios, seleccione **[!UICONTROL Configuración de correo electrónico]**.
1. En el cuadro de diálogo Config. correo, especifique una de estas configuraciones:

   * **[!UICONTROL Enviar correo electrónico]** : anule la selección de esta opción si no desea informar a los nuevos usuarios por correo electrónico de que los ha suscrito.

   * **[!UICONTROL Contraseña predeterminada]** : introduzca una contraseña temporal para nuevos usuarios o deje vacío el campo para que Dynamic Media Classic genere contraseñas aleatorias. Se pide a los usuarios que cambien sus contraseñas la primera vez que inicien sesión.

   * **[!UICONTROL URL de reemplazo]** : introduzca una URL diferente del predeterminada si los usuarios acceden a Dynamic Media Classic a través de una URL diferente.

## Otras tareas de administración de usuarios {#other-user-management-tasks}

También puede realizar las siguientes tareas desde la pantalla de ajuste Administración de usuarios:

* **[!UICONTROL Filtrar y ordenar la lista de usuarios]** : filtre la lista de usuarios de Media Portal para localizar usuarios.

* **[!UICONTROL Eliminar usuarios]** : eliminar un usuario de la lista.

* **[!UICONTROL Activar y desactivar usuarios]** : impedir que un usuario acceda a carpetas.

* **[!UICONTROL Editar información de usuario]** : introduzca información actualizada sobre un usuario.

* **[!UICONTROL Crear campos definidos por el usuario]** : cree campos de metadatos personalizados y definidos por el usuario para que puedan ayudarle a organizar los recursos en Dynamic Media Classic. Los campos también pueden activarse o desactivarse según sea necesario.

Consulte [Campos personalizables](application-setup.md#user_defined_fields).
