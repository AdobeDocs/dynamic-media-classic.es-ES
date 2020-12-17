---
title: Inicio de sesión en Adobe Analytics
seo-title: Inicio de sesión en Adobe Analytics
description: nulo
seo-description: Obtenga información sobre cómo iniciar sesión en Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 37%

---


# Inicio de sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Antes de iniciar sesión para configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Dynamic Media Classic, compruebe que se le ha agregado como miembro del grupo Acceso a servicios Web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web de Marketing Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, haga clic en **Herramientas de administración** > **Administración de usuario** > **Editar grupos**.

Al iniciar sesión, tiene la opción de introducir el ID de organización de Marketing Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, el sistema de informes de vídeo seguirá funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (Identity Management System) para iniciar sesión, la introducción de credenciales directas no funcionará.

**Inicio de sesión en Adobe Analytics**

1. Cerca de la esquina superior derecha de la página de Dynamic Media Classic, toque **[!UICONTROL Ajustes > Ajustes de aplicación]**.
1. En el panel izquierdo, en **[!UICONTROL Ajustes de aplicación]**, toque **[!UICONTROL Adobe Analytics]**.
1. En la página Configuración de Adobe Analytics, toque **[!UICONTROL Inicio de sesión de Adobe Analytics]**.
1. En el cuadro de diálogo **[!UICONTROL Inicio de sesión de Adobe Analytics]**, introduzca el nombre de la compañía, el ID de organización de Marketing Cloud (opcional), el nombre de usuario y la clave *clave secreta compartida* en el campo de texto **[!UICONTROL Contraseña]**.

   Puede recuperar la clave *secreta compartida* desde la consola de administración de Analytics. Consulte [Cómo obtener las credenciales de API para cuentas de usuario](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html).

1. Haga clic en **[!UICONTROL Inicio de sesión]**.
1. En el menú desplegable **[!UICONTROL Grupo de informes]**, elija un grupo de informes y haga clic en **[!UICONTROL Aceptar]**.

   >[!NOTE]
   >
   >Al iniciar sesión por primera vez en Adobe Analytics, la lista desplegable Grupo de informes se muestra vacía. En el primer inicio de sesión no se elige un conjunto de informes. Tras iniciar sesión por primera vez, ciérrela y, a continuación, regrese a la pantalla de Adobe Analytics. Vuelva a iniciar sesión para poder seleccionar un conjunto de informes.

>[!MORELIKETHIS]
>
>* [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

