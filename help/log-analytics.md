---
title: Inicio de sesión en Adobe Analytics
description: Obtenga información sobre cómo iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Inicio de sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Antes de iniciar sesión para configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Dynamic Media Classic de Adobe, compruebe que es miembro del grupo Acceso a servicios web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web del Experience Cloud, independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, vaya a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Al iniciar sesión, tiene la opción de introducir su ID de organización de Experience Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, los informes de vídeo seguirán funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (Identity Management System) para iniciar sesión, la introducción de credenciales directas no funciona.

**Para iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic:**

Comience por integrar Dynamic Media Classic con Adobe Analytics OAuth. La integración de Adobe Analytics OAuth con Dynamic Media Classic solo se realiza una vez por usuario.

1. Acceda a [Consola de desarrollador de Adobe](https://developer.adobe.com/console). Asegúrese de que su cuenta tiene permisos de administrador para la organización para la que se requiere la integración.
1. Cerca de la esquina superior derecha de la página principal, en la lista desplegable, seleccione la empresa adecuada. (La captura de pantalla siguiente es solo con fines informativos; el nombre real de la empresa que seleccione puede variar).

   ![Cree un nuevo proyecto](assets/analytics-oauth1.png)

1. Realice una de las siguientes acciones:

   * En la parte superior de la página, en la pestaña **[!UICONTROL Home]**, seleccione **[!UICONTROL Crear nuevo proyecto]**.
   * En la parte superior de la página, en la pestaña **[!UICONTROL Proyectos]**. Cerca de la esquina derecha de la página, seleccione **[!UICONTROL Crear nuevo proyecto]**.

1. En la página del proyecto, seleccione **[!UICONTROL Agregar API]**.
1. En la página **[!UICONTROL Add an API]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.

   ![Añadir una API](assets/analytics-oauth2.png)

1. En la página **[!UICONTROL Configurar API]**, seleccione **[!UICONTROL AUTENTICACIÓN DE USUARIO OAuth]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.
1. En la página **[!UICONTROL Configurar API]**, seleccione **[!UICONTROL OAUTH 2.0 Web]**.
1. En el campo de texto **[!UICONTROL Default redirect URI]** , introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. En el campo de texto **[!UICONTROL Redirect URI pattern]** , introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Guardar API configurada]**.
1. En el panel de navegación, en el lado izquierdo de la página de Adobe Analytics, en **[!UICONTROL Credentials]**, seleccione **[!UICONTROL OAuth Web]**.
1. En **[!UICONTROL Detalles de credenciales]**, haga lo siguiente:
   * En **[!UICONTROL Client ID]**, seleccione **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Analytics en la aplicación de escritorio de Dynamic Media Classic que debe seguir.
   * En **[!UICONTROL Secreto del cliente]**, seleccione **[!UICONTROL Recuperar secreto del cliente]** para mostrar el valor asociado. Seleccione **[!UICONTROL Copy]** para copiar el valor. Necesita este valor para la configuración posterior de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic que debe seguir.

**Configuración de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic**

>[!NOTE]
>
>Después de la configuración inicial de Adobe Analytics en Dynamic Media Classic, las únicas veces que debe rehacer la configuración son en los siguientes casos:
>
>* Se agrega un nuevo informe en Analytics y el usuario desea comenzar a enviar datos a ese nuevo informe.
>* El servidor de seguimiento se actualiza en Adobe Analytics.
>* Se introduce una nueva variable de seguimiento en un informe y desea vincular una variable de visualizador específica en la interfaz de usuario de Dynamic Media Classic a esa nueva variable de Analytics.

>


1. Cerca de la esquina superior derecha de la aplicación de escritorio de Dynamic Media Classic de Adobe, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]**.
1. En el panel izquierdo, en **[!UICONTROL Ajustes de aplicación]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. En la página **[!UICONTROL Configuración de Adobe Analytics]**, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.
1. En el cuadro de diálogo **[!UICONTROL Inicio de sesión de Adobe Analytics]**, en el campo ID de cliente y en el campo Secreto de cliente , pegue los valores respectivos que ha copiado anteriormente.
1. Realice el inicio de sesión de IMS.

   Cuando haya iniciado sesión correctamente, la lista desplegable **[!UICONTROL COMPANIES]**, iniciada por las empresas que están a su disposición, será visible.

1. En la lista desplegable **[!UICONTROL COMPANIES]**, elija una empresa.

   Después de seleccionar una empresa, se vuelve visible la lista desplegable **[!UICONTROL SUITES]**, iniciada por los grupos de informes disponibles para la empresa seleccionada.

1. En la lista desplegable **[!UICONTROL SUITES]**, elija un grupo de informes.

   >[!NOTE]
   >
   >De forma predeterminada, el usuario debe tener en cuenta que las listas desplegables **[!UICONTROL COMPANIES]** y **[!UICONTROL SUITES]** están vacías. Como tal, el usuario debe seleccionar un valor de cada lista. —>

1. Seleccione **[!UICONTROL Aceptar]** para poder guardar la configuración.

>[!MORELIKETHIS]
>
>* [Configurar informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

