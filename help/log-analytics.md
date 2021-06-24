---
title: Inicio de sesión en Adobe Analytics
description: Obtenga información sobre cómo iniciar sesión en Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 35%

---

# Inicio de sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Antes de iniciar sesión para configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Dynamic Media Classic, compruebe que es miembro del grupo Acceso a servicios web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web de Marketing Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, haga clic en **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuario]** > **[!UICONTROL Editar grupos]**.

Al iniciar sesión, tiene la opción de introducir su ID de organización de Marketing Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, los informes de vídeo seguirán funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (sistema Identity Management) para iniciar sesión, la introducción de credenciales directas no funciona.

**Inicio de sesión en Adobe Analytics:**

1. Cerca de la esquina superior derecha de la página de Dynamic Media Classic, pulse **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]**.
1. En el panel izquierdo, en **[!UICONTROL Ajustes de aplicación]**, pulse **[!UICONTROL Adobe Analytics]**.
1. En la página Configuración de Adobe Analytics, pulse **[!UICONTROL Inicio de sesión de Adobe Analytics]**.
1. En el cuadro de diálogo **[!UICONTROL Inicio de sesión de Adobe Analytics]**, introduzca el nombre de su empresa, el ID de organización de Marketing Cloud (opcional), el nombre de usuario y la clave *secreto compartido* en el campo de texto **[!UICONTROL Contraseña]**.

   Puede recuperar la clave *shared secret* del Admin Console de Analytics. Consulte [Cómo obtener las credenciales de API para las cuentas de usuario](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Haga clic en **[!UICONTROL Inicio de sesión]**.
1. En el menú desplegable **[!UICONTROL Grupo de informes]**, elija un grupo de informes y haga clic en **[!UICONTROL Aceptar]**.

   >[!NOTE]
   >
   >Al iniciar sesión por primera vez en Adobe Analytics, la lista desplegable Grupo de informes se muestra vacía. En el primer inicio de sesión no se elige un conjunto de informes. Tras iniciar sesión por primera vez, ciérrela y, a continuación, regrese a la pantalla de Adobe Analytics. Vuelva a iniciar sesión para poder seleccionar un conjunto de informes.

>[!MORELIKETHIS]
>
>* [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

