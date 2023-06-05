---
title: Inicio de sesión en Adobe Analytics
description: Obtenga información sobre cómo iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# Inicio de sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Antes de iniciar sesión para configurar informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Adobe Dynamic Media Classic, compruebe que es miembro del grupo Acceso a servicio web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web del Experience Cloud, independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, vaya a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Al iniciar sesión, tiene la opción de introducir el ID de organización de Experience Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, el sistema de informes de vídeo seguirá funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (sistema Identity Management) para iniciar sesión, no funcionará al introducir credenciales directas.

## Inicie sesión en Adobe Analytics desde Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Comience por integrar Dynamic Media Classic con Adobe Analytics OAuth. La integración de Adobe Analytics OAuth con Dynamic Media Classic suele realizarse solo una vez por usuario.

1. Acceso [Consola de Adobe Developer](https://developer.adobe.com/console). Asegúrese de que su cuenta tenga permisos de administrador para la organización para la que se requiere la integración.
1. Cerca de la esquina superior derecha de la página principal, en la lista desplegable, seleccione la empresa adecuada. (La captura de pantalla siguiente es solo con fines informativos; el nombre real de la compañía que seleccione puede variar).

   ![Cree un nuevo proyecto](assets/analytics-oauth1.png)

1. Realice una de las siguientes acciones:

   * En la parte superior de la página, en **[!UICONTROL Inicio]** pestaña, seleccione **[!UICONTROL Crear nuevo proyecto]**.
   * En la parte superior de la página, en **[!UICONTROL Proyectos]** pestaña. Cerca de la esquina derecha de la página, seleccione **[!UICONTROL Crear nuevo proyecto]**.

1. En la página del proyecto, seleccione **[!UICONTROL Añadir API]**.
1. En el **[!UICONTROL Añadir una API]** página, seleccione **[!UICONTROL Adobe Analytics]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.

   ![Añadir una API](assets/analytics-oauth2.png)

1. En el **[!UICONTROL Configurar API]** página, seleccione **[!UICONTROL AUTENTICACIÓN DE USUARIO OAuth]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.
1. En el **[!UICONTROL Configurar API]** página, seleccione **[!UICONTROL Web de OAUTH 2.0]**.
1. En el **[!UICONTROL URI de redirección predeterminado]** Campo de texto, introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. En el **[!UICONTROL Patrón de URI de redirección]** Campo de texto, introduzca la siguiente ruta exactamente como se muestra:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Guardar API configurada]**.
1. En el panel de navegación, en la parte izquierda de la página de Adobe Analytics, debajo de **[!UICONTROL Credenciales]**, seleccione **[!UICONTROL Web de OAuth]**.
1. En **[!UICONTROL Detalles de credenciales]**, haga lo siguiente:
   * En **[!UICONTROL ID de cliente]**, seleccione **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Analytics en la aplicación de escritorio de Dynamic Media Classic que se va a seguir.
   * En **[!UICONTROL Secreto del cliente]**, seleccione **[!UICONTROL Recuperar secreto de cliente]** para mostrar el valor asociado. Seleccionar **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic que se va a seguir.

## Configuración de Adobe Analytics en Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Después de la configuración inicial de Adobe Analytics en Dynamic Media Classic, las únicas veces que debe rehacer la configuración son en los siguientes casos:
>
>* Se agrega un nuevo informe en Analytics y el usuario desea comenzar a enviar datos a ese nuevo informe.
>* El servidor de seguimiento se actualiza en Adobe Analytics.
>* Se introduce una nueva variable de seguimiento en un informe y se desea vincular una variable específica del visualizador en la interfaz de usuario de Dynamic Media Classic a esa nueva variable de Analytics.
>


1. Cerca de la esquina superior derecha de la aplicación de escritorio de Adobe Dynamic Media Classic, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]**.
1. En el panel izquierdo, debajo de **[!UICONTROL Ajustes de aplicación]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. En el **[!UICONTROL Configuración de Adobe Analytics]** página, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.
1. En el **[!UICONTROL Inicio de sesión de Adobe Analytics]** , en el **[!UICONTROL ID DE CLIENTE]** y el **[!UICONTROL SECRETO DEL CLIENTE]** , pegue los valores respectivos que ha copiado anteriormente.
1. En la esquina inferior derecha del cuadro de diálogo, seleccione **[!UICONTROL Iniciar sesión]** y realizar el inicio de sesión en Adobe IMS (Identity Management Services).

   Cuando inicia sesión correctamente, vuelve a aparecer el cuadro de diálogo Inicio de sesión de Adobe Analytics junto con el **[!UICONTROL EMPRESAS]** lista desplegable, iniciada por las empresas disponibles para usted.

1. Desde el **[!UICONTROL EMPRESAS]** , seleccione una empresa.

   Después de seleccionar una empresa, la variable **[!UICONTROL SUITES]** La lista desplegable, iniciada por los Grupos de informes disponibles para la empresa seleccionada, queda visible.

1. Desde el **[!UICONTROL SUITES]** , elija un grupo de informes.

   >[!NOTE]
   >
   >De forma predeterminada, el usuario debe tener en cuenta que tanto **[!UICONTROL EMPRESAS]** y **[!UICONTROL SUITES]** las listas desplegables están vacías. Como tal, el usuario debe seleccionar un valor de cada lista.

1. Seleccionar **[!UICONTROL OK]** para poder guardar la configuración.

   >[!NOTE]
   >
   >El **[!UICONTROL Servidor de Adobe Analytics]** el campo se rellena con un servidor de seguimiento de terceros sugerido que coincide con el área de nombres de analytics cuando selecciona **[!UICONTROL OK]**. Si utiliza un servidor de seguimiento diferente, actualícelo en este campo para evitar la pérdida de datos.

1. En la esquina inferior izquierda de la página Configuración de Adobe Analytics, seleccione **[!UICONTROL Guardar]** para asegurarse de que se ha actualizado la configuración de la cuenta de Adobe Analytics.

>[!MORELIKETHIS]
>
>* [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

