---
title: Iniciar sesión en Adobe Analytics
description: Obtenga información sobre cómo iniciar sesión en Adobe Analytics desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Iniciar sesión en Adobe Analytics{#log-in-to-adobe-analytics}

Compruebe que es miembro del grupo Acceso a servicio Web de Adobe Analytics. Hágalo antes de iniciar sesión para configurar informes de Adobe Analytics y relacionar variables de informes de Adobe Analytics con eventos de Adobe Dynamic Media Classic. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados. Para ello, utilice la API de servicios web del Experience Cloud, independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, ve a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Al iniciar sesión, tiene la opción de introducir el ID de organización de Experience Cloud para utilizar la implementación de análisis de vídeo más reciente. Si decide no introducir su ID, el sistema de informes de vídeo seguirá funcionando. Sin embargo, puede hacer que los datos no se integren correctamente con otros datos de ese cliente desde fuera de Adobe Dynamic Media Classic.

>[!NOTE]
>
>Si su cuenta de Adobe Analytics se ha migrado a la autenticación basada en IMS de Adobe (sistema Identity Management) para iniciar sesión, no funcionará al introducir credenciales directas.

## Inicie sesión en Adobe Analytics desde Adobe Dynamic Media Classic {#log-in-to-analytics-from-dmc}

Comience por integrar Dynamic Media Classic con Adobe Analytics OAuth. La integración de Adobe Analytics OAuth con Dynamic Media Classic suele realizarse solo una vez por usuario.

1. Acceder a [Adobe Developer Console](https://developer.adobe.com/console). Asegúrese de que su cuenta tenga permisos de administrador para la organización para la que se requiere la integración.
1. Cerca de la esquina superior derecha de la página principal, en la lista desplegable, seleccione la empresa adecuada. (La captura de pantalla siguiente es solo con fines informativos; el nombre real de la compañía que seleccione puede variar).

   ![Crear un nuevo proyecto](assets/analytics-oauth1.png)

1. Realice una de las siguientes acciones:

   * En la parte superior de la página, en la ficha **[!UICONTROL Inicio]**, seleccione **[!UICONTROL Crear un nuevo proyecto]**.
   * En la parte superior de la página, en la ficha **[!UICONTROL Proyectos]**. Cerca de la esquina derecha de la página, seleccione **[!UICONTROL Crear un nuevo proyecto]**.

1. En la página del proyecto, seleccione **[!UICONTROL Agregar API]**.
1. En la página **[!UICONTROL Agregar una API]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.

   ![Agregar una API](assets/analytics-oauth2.png)

1. En la página **[!UICONTROL `Configure API`]**, seleccione **[!UICONTROL AUTENTICACIÓN DE USUARIO OAuth]**.
1. Cerca de la esquina inferior derecha de la página, seleccione **[!UICONTROL Siguiente]**.
1. En la página **[!UICONTROL `Configure API`]**, seleccione **[!UICONTROL OAUTH 2.0 Web]**.
1. En el campo de texto **[!UICONTROL URI de redirección predeterminado]**, escriba la siguiente ruta exactamente como se muestra:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. En el campo de texto **[!UICONTROL Patrón de URI de redireccionamiento]**, escriba la siguiente ruta exactamente como se muestra:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Guardar la API configurada]**.
1. En el panel de navegación, en la parte izquierda de la página Adobe Analytics, en **[!UICONTROL Credenciales]**, seleccione **[!UICONTROL OAuth Web]**.
1. En **[!UICONTROL Detalles de credencial]**, haga lo siguiente:
   * En **[!UICONTROL ID de cliente]**, seleccione **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Analytics en la aplicación de escritorio de Dynamic Media Classic que se va a seguir.
   * En **[!UICONTROL Secreto de cliente]**, seleccione **[!UICONTROL Recuperar secreto de cliente]** para mostrar el valor asociado. Seleccione **[!UICONTROL Copiar]** para copiar el valor. Necesita este valor para la configuración posterior de Adobe Analytics en la aplicación de escritorio de Dynamic Media Classic que se va a seguir.

## Configuración de Adobe Analytics en Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Después de la configuración inicial de Adobe Analytics en Dynamic Media Classic, la única vez que debe rehacer la configuración es en los siguientes casos:
>
>* Se agrega un nuevo informe en Analytics y el usuario desea comenzar a enviar datos a ese nuevo informe.
>* El servidor de seguimiento se actualiza en Adobe Analytics.
>* Se introduce una nueva variable de seguimiento en un informe y se desea vincular una variable específica del visualizador en la interfaz de usuario de Dynamic Media Classic a esa nueva variable de Analytics.
>

1. Cerca de la esquina superior derecha de la aplicación de escritorio de Adobe Dynamic Media Classic, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]**.
1. En el panel izquierdo, en **[!UICONTROL Configuración de aplicación]**, seleccione **[!UICONTROL Adobe Analytics]**.
1. En la página **[!UICONTROL Configuración de Adobe Analytics]**, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.
1. En el cuadro de diálogo **[!UICONTROL Inicio de sesión de Adobe Analytics]**, en el campo **[!UICONTROL ID DE CLIENTE]** y en el campo **[!UICONTROL SECRETO DE CLIENTE]**, pegue los valores respectivos que ha copiado anteriormente.
1. En la esquina inferior derecha del cuadro de diálogo, seleccione **[!UICONTROL Login]** y realice su inicio de sesión en Adobe IMS (Identity Management Services).

   Cuando inicia sesión correctamente, vuelve a aparecer el cuadro de diálogo Inicio de sesión de Adobe Analytics junto con la lista desplegable **[!UICONTROL COMPAÑÍAS]**, iniciada por las empresas disponibles para usted.

1. En la lista desplegable **[!UICONTROL COMPAÑÍAS]**, elija una empresa.

   Después de seleccionar una compañía, se hace visible la lista desplegable **[!UICONTROL SUITES]**, iniciada por los grupos de informes que están disponibles para la compañía seleccionada.

1. En la lista desplegable **[!UICONTROL GRUPOS]**, elija un grupo de informes.

   >[!NOTE]
   >
   >De manera predeterminada, el usuario debe tener en cuenta que las listas desplegables **[!UICONTROL COMPANIES]** y **[!UICONTROL SUITES]** están vacías. Como tal, el usuario debe seleccionar un valor de cada lista.

1. Seleccione **[!UICONTROL Aceptar]** para guardar la configuración.

   >[!NOTE]
   >
   >El campo **[!UICONTROL Adobe Analytics Server]** se rellena con un servidor de seguimiento de terceros sugerido que coincide con el área de nombres de Analytics cuando selecciona **[!UICONTROL Aceptar]**. Si utiliza un servidor de seguimiento diferente, actualícelo en este campo para evitar la pérdida de datos.

1. En la esquina inferior izquierda de la página Configuración de Adobe Analytics, seleccione **[!UICONTROL Guardar]** para asegurarse de que se ha actualizado la configuración de la cuenta de Adobe Analytics.

>[!MORELIKETHIS]
>
>* [Configurar informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
