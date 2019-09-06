---
title: Adición y administración de usuarios de Media Portal
seo-title: Adición y administración de usuarios de Media Portal
description: nulo
seo-description: Descubra cómo agregar y administrar usuarios de Media Portal
uuid: 96 d 4103 c -6428-4 ce 1-b 9 e 4-231599304 f 27
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/media_ portal
discoiquuid: 5 e 933045-ce 1 a -41 b 9-ba 8 b -2151 c 396 b 7 a 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adición y administración de usuarios de Media Portal{#adding-and-managing-media-portal-users}

Como administrador puede añadir y administrar a los usuarios, decidir si pueden cambiar las contraseñas, editar su información y cargar listas de usuarios. Estas tareas se realizan desde la pantalla Administración de usuarios. Para acceder a esta pantalla, haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.

>[!NOTE]
>
>antes de agregar usuarios tendrá que configurar grupos para administrarlos. Media Portal no permite agregar un usuario sin asignarlo a uno o varios grupos. Para obtener más información, consulte [Creación y administración de grupos de Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Administración de las contraseñas de Media Portal {#handling-media-portal-passwords}

A los usuarios, colaboradores y usuarios colaboradores de Media Portal se les envía un mensaje de correo electrónico de bienvenida con una contraseña cuando usted los registra. Los administradores pueden decidir si los usuarios de Media Portal pueden cambiar esta contraseña.

1. Haga clic en **Ajustes** &gt; **Configuración de Media Portal** &gt; **Configuración general**.
1. En la pantalla Configuración general, marque o desmarque la opción **Permitir que el usuario de Media Portal cambie la contraseña**.
1. Haga clic en **Guardar**.

>[!NOTE]
>
>Los usuarios de Media Portal con permiso para cambiar su contraseña pueden hacerlo haciendo clic en **Ajustes** &gt; **Ajustes personales** y cambiando la contraseña en la pantalla Ajustes personales.

## Adición de un usuario de Media Portal {#adding-a-media-portal-user}

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. En la página Administración de usuarios, haga clic en **Agregar**.
1. En el cuadro de diálogo Agregar usuario, en el panel Información del usuario, escriba el nombre, el apellido y la dirección de correo electrónico del usuario y, a continuación, haga clic en **Siguiente**.
1. En el panel Empresa/Función, en la lista desplegable de empresas, seleccione una o varias empresas para el usuario.
1. En la lista Función, seleccione una función de Media Portal y, a continuación, haga clic en **Siguiente**.

   Consulte [Funciones de usuario en Media Portal](media-portal-user-roles.md#media_portal_user_roles).

1. En el panel Grupos de acceso, seleccione uno o varios grupos.

   Consulte [Creación y administración de grupos de Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Opcional) Haga clic en **Config. correo** y seleccione una configuración del correo electrónico distinta de la predeterminada.

   Consulte [Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Haga clic en **Agregar usuario**.

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
| Función de usuario | Mediaportaladminmedia aportalusermediaportalaporttoraveraportalcontributoruser |
| Grupos | Lista de una o varias asignaciones de grupos de cuentas de cada usuario, separadas por comas. Debe especificar el grupo, agregando como prefijo el nombre de cuenta, separado por la barra diagonal (/). Por ejemplo, PortalCo/IT, donde PortalCo es la cuenta e IT es el grupo dentro de la cuenta PortalCo. |

La siguiente hoja de cálculo de ejemplo muestra cómo diseñar un archivo CSV:

| Nombre | Apellidos | Correo electrónico | Contraseña | Función de usuario | Grupos |
|--- |--- |--- |--- |--- |--- |
| Pedro | Pérez | `petep@company.com` | bienvenido | Administrador de Media Portal | CoPortal/TI,CoPortal/Admin |
| Javier | Gómez | `kevinm@myco.com` | bienvenido | Usuario de Media Portal | PortalCo/GrupoMarketing, PortalCo/prueba |


### Carga del archivo CSV {#uploading-the-csv-file}

1. Abra la pantalla de ajuste Administración de usuarios.
1. Haga clic en **Cargar lista de usuarios**.
1. En el cuadro de diálogo Seleccione el archivo que desea cargar, seleccione el archivo CSV y haga clic en **Abrir**.

Se añaden automáticamente los usuarios de la lista a los grupos especificados y se envía un mensaje de correo electrónico de bienvenida.

>[!NOTE]
Si el archivo CSV no tiene el formato correcto, aparece el mensaje de error "Se ha producido un error al procesar el archivo CSV cargado. Compruebe si los datos del archivo son válidos". Además, si el archivo CSV contiene un usuario de IP o IPS existente, éste no se añade a la lista de usuarios.

## Generación de una lista seleccionable de usuarios de Media Portal {#generating-a-selectable-list-of-media-portal-users}

Puede ver los nombres y las direcciones de correo electrónico de los usuarios de Media Portal en una ventana emergente. Esta lista resulta útil para cortar y pegar nombres y direcciones de correo electrónico de usuarios y usarlos en otra aplicación distinta a Media Portal.

1. Haga clic en **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. En la lista desplegable **Por función de usuario**, elija el nombre de una función de usuario de Media Portal y haga clic en **Actualizar** para mostrar los nombres de una clase de usuario de Media Portal.
1. Haga clic en el botón **Lista emergente** para abrir la ventana emergente. Esta lista se puede copiar y pegar.

## Configuración del mensaje de correo electrónico de bienvenida para los usuarios de Media Portal {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Puede enviar un mensaje de correo de bienvenida cuando agregue usuarios, colaboradores y usuarios colaboradores de Media Portal. Puede configurar este mensaje de correo electrónico o indicar a Dynamic Media Classic que no lo envíe.

1. Elija **Ajustes** &gt; **Ajustes de aplicación** &gt; **Ajustes de administración** &gt; **Administración de usuarios**.
1. In the User Administration Setup screen, click **Email Settings**.
1. En el cuadro de diálogo Config. correo, especifique una de estas configuraciones:

   **Enviar mensaje de correo electrónico** Deseleccione esta opción si no desea informar por correo electrónico a los usuarios nuevos de que los ha registrado.

   **Contraseña predeterminada** Introduzca una contraseña temporal para los usuarios nuevos o deje el campo vacío para que Dynamic Media Classic genere contraseñas aleatorias. La primera vez que un usuario inicie sesión, se le pedirá que cambie la contraseña.

   **URL de sustitución** Introduzca una URL diferente de la predeterminada si los usuarios acceden a Dynamic Media Classic a través de una URL diferente.

## Otras tareas de administración de usuarios {#other-user-management-tasks}

También puede realizar las siguientes tareas desde la pantalla de ajuste Administración de usuarios:

**Filtre y ordene la lista de usuarios** Filtre la lista de usuarios de Media Portal para localizar usuarios. Consulte Filtrado y ordenación de la lista de usuarios.

**Eliminar usuarios** Elimine un usuario de la lista. Consulte Eliminación de un usuario.

**Activar y desactivar usuarios** Suspenda el acceso de un usuario a carpetas. Consulte Activación y desactivación de usuarios.

**Editar información de usuario** Introduzca información actualizada sobre un usuario. Consulte Edición de información de usuario.

**Creación de campos definidos por el usuario** Cree campos de metadatos personalizados definidos por el usuario para ayudar a organizar los recursos en Scene 7 Publishing System. Los campos también pueden activarse o desactivarse según sea necesario.

Consulte [Campos personalizables](application-setup.md#user_defined_fields).
