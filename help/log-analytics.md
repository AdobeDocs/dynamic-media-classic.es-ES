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
source-git-commit: 876b4c61167b28f7d5e50a656564eafcbe5b9eab
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 1%

---

# Inicio de sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Antes de iniciar sesión para configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Adobe Dynamic Media Classic, compruebe que es miembro del grupo Acceso a servicios web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web del Experience Cloud, independientemente de los permisos establecidos en la interfaz. Para añadir un miembro al grupo, en Adobe Analytics, vaya a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Al iniciar sesión, tiene la opción de introducir su ID de organización de Experience Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, los informes de vídeo seguirán funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (Identity Management System) para iniciar sesión, la introducción de credenciales directas no funciona.

**Para iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic:**

Comience por integrar Dynamic Media Classic con Adobe Analytics OAuth. La integración de Adobe Analytics OAuth con Dynamic Media Classic se realiza normalmente solo una vez por usuario.

1. Acceso [Adobe Developer Console](https://developer.adobe.com/console). Asegúrese de que su cuenta tiene permisos de administrador para la organización para la que se requiere la integración.
1. Cerca de la esquina superior derecha de la página principal, en la lista desplegable, seleccione la empresa adecuada. (La captura de pantalla siguiente es solo con fines informativos; el nombre real de la empresa que seleccione puede variar).

   ![Cree un nuevo proyecto](assets/analytics-oauth1.png)

1. Realice una de las siguientes acciones:

   * En la parte superior de la página, desde la **[!UICONTROL Página principal]** , seleccione **[!UICONTROL Crear nuevo proyecto]**.
   * En la parte superior de la página, desde la **[!UICONTROL Proyectos]** pestaña . Cerca de la esquina derecha de la página, seleccione **[!UICONTROL Crear nuevo proyecto]**.

1. En la página del proyecto, seleccione **[!UICONTROL Añadir API]**.
1. En el **[!UICONTROL Añadir una API]** página, seleccione **[!UICONTROL Adobe Analytics]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.

   ![Añadir una API](assets/analytics-oauth2.png)

1. En el **[!UICONTROL Configuración de API]** página, seleccione **[!UICONTROL AUTENTICACIÓN DE USUARIO OAuth]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.
1. En el **[!UICONTROL Configuración de API]** página, seleccione **[!UICONTROL OAUTH 2.0 Web]**.
1. En el **[!UICONTROL URI de redirección predeterminado]** , introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. En el **[!UICONTROL Patrón de URI de redirección]** , introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Guardar la API configurada]**.
1. En el panel de navegación, en el lado izquierdo de la página de Adobe Analytics, debajo de **[!UICONTROL Credenciales]**, seleccione **[!UICONTROL Web de OAuth]**.
1. En **[!UICONTROL Detalles de la credencial]**, haga lo siguiente:
   * En **[!UICONTROL ID de cliente]**, seleccione **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Analytics en la aplicación de escritorio de Dynamic Media Classic que debe seguir.
   * En **[!UICONTROL Secreto del cliente]**, seleccione **[!UICONTROL Recuperar secreto de cliente]** para mostrar el valor asociado. Select **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic que debe seguir.

**Configuración de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic**

>[!NOTE]
>
>Después de la configuración inicial de Adobe Analytics en Dynamic Media Classic, las únicas veces que debe rehacer la configuración son en los siguientes casos:
>
>* Se agrega un nuevo informe en Analytics y el usuario desea comenzar a enviar datos a ese nuevo informe.
>* El servidor de seguimiento se actualiza en Adobe Analytics.
>* Se introduce una nueva variable de seguimiento en un informe y desea vincular una variable de visualizador específica en la interfaz de usuario de Dynamic Media Classic a esa nueva variable de Analytics.

>


1. Cerca de la esquina superior derecha de la aplicación de escritorio de Adobe Dynamic Media Classic, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]**.
1. En el panel izquierdo, debajo de **[!UICONTROL Configuración de la aplicación]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. En el **[!UICONTROL Configuración de Adobe Analytics]** página, seleccione **[!UICONTROL Inicio de sesión en Adobe Analytics]**.
1. En el **[!UICONTROL Inicio de sesión en Adobe Analytics]** en el **[!UICONTROL ID DE CLIENTE]** y **[!UICONTROL SECRETO DEL CLIENTE]** pegue los valores respectivos que ha copiado anteriormente.
1. En la esquina inferior derecha del cuadro de diálogo, seleccione Iniciar sesión y realice el inicio de sesión de Adobe IMS (Servicios de Identity Management).

   Cuando inicia sesión correctamente, vuelve a aparecer el cuadro de diálogo Inicio de sesión de Adobe Analytics junto con la variable **[!UICONTROL EMPRESAS]** lista desplegable, iniciada por las empresas disponibles para usted.

1. En el **[!UICONTROL EMPRESAS]** lista desplegable, elija una empresa.

   Después de seleccionar una empresa, la variable **[!UICONTROL SUITES]** lista desplegable, iniciada por los grupos de informes disponibles para la empresa seleccionada, se vuelve visible.

1. En el **[!UICONTROL SUITES]** lista desplegable, elija un grupo de informes.

   >[!NOTE]
   >
   >De forma predeterminada, el usuario debe tener en cuenta que ambas **[!UICONTROL EMPRESAS]** y **[!UICONTROL SUITES]** las listas desplegables están vacías. Como tal, el usuario debe seleccionar un valor de cada lista.

1. Select **[!UICONTROL OK]** para que pueda guardar la configuración.

   >[!NOTE]
   >
   >La variable **[!UICONTROL Adobe Analytics Server]** se rellena con un servidor de seguimiento de terceros sugerido que coincide con el espacio de nombres de analytics al seleccionar **[!UICONTROL OK]**. Si utiliza un servidor de seguimiento diferente, actualícelo en este campo para evitar la pérdida de datos.

1. En la esquina inferior izquierda de la página Configuración de Adobe Analytics , seleccione **[!UICONTROL Guardar]** para asegurarse de que se actualiza la configuración de la cuenta de Adobe Analytics.

>[!MORELIKETHIS]
>
>* [Configurar informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

