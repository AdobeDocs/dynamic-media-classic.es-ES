---
title: '"Inicio rápido: Integrar Adobe Dynamic Media Classic y Adobe Analytics"'
description: Introducción e inicio rápido sobre cómo integrar Adobe Dynamic Media Classic y Adobe Analytics para ayudarle a poner en marcha rápidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# Inicio rápido: Integración de Adobe Dynamic Media Classic y Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics es un producto líder de la industria que ofrece a los vendedores un lugar donde pueden medir, analizar y optimizar datos integrados de todas las iniciativas en línea a través de múltiples canales de marketing.

Después de integrar Adobe Analytics con Adobe Dynamic Media Classic, puede obtener informes sobre el comportamiento de los visitantes del sitio web mediante los visores de Adobe Dynamic Media Classic en su sitio web. Por ejemplo, cuando un visitante de un sitio web hace clic en un destino de zoom en un visor de zoom Dynamic Media Classic de Adobe, Adobe Analytics registra esta acción. Los informes de Adobe Analytics pueden recopilar información acumulativa sobre la actividad del usuario en los visores de Adobe de Dynamic Media Classic.

Con el uso de los informes de Adobe Analytics, podrá obtener una imagen clara de la actividad de los clientes en su sitio web. Puede determinar qué presentaciones de productos generan conversiones y cuáles no atraen el interés del cliente.

Consulte también [Medir vídeo en Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Se necesita una cuenta de Adobe Analytics válida para integrar Analytics con Adobe Dynamic Media Classic y generar informes de Analytics.

Este inicio rápido se ha diseñado para ayudarle en el uso inicial del kit de instrumentación de Adobe Analytics.

## 1. Inicie sesión en Adobe Analytics mediante el Adobe de Dynamic Media Classic y descargue las variables de informes de Adobe Analytics

>[!NOTE]
>
>Antes de configurar los informes de Adobe Analytics y hacer coincidir las variables de informes de Adobe Analytics con los eventos de Adobe Dynamic Media Classic, compruebe que se ha agregado como miembro del grupo Acceso a servicios web en Adobe Analytics. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados mediante la API de servicios web del Experience Cloud, independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, vaya a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Después de comprobar que es miembro del grupo Acceso a servicio Web, en Adobe Dynamic Media Classic, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Adobe Analytics]**. En la página Configuración de Adobe Analytics, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.

Consulte [Inicio de sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

En el cuadro de diálogo Inicio de sesión de Adobe Analytics, escriba su ID de organización de Experience Cloud (opcional) y sus credenciales completas y, a continuación, seleccione **[!UICONTROL Inicio de sesión]**. En el menú desplegable Grupo de informes, seleccione el nombre del grupo de informes que desee utilizar.

## 2. Asigne variables de informes de Adobe Analytics a los eventos del visor de Dynamic Media Classic de Adobe y a las variables de Dynamic Media Classic de Adobe

En la página de configuración de Adobe Analytics, especifique la información que desee incluir en los informes de Adobe Analytics. Para cada evento del visor de Dynamic Media Classic de Adobe del que desee información, elija una variable de Adobe Analytics (del grupo de informes) y una variable de Dynamic Media Classic de Adobe.

* Los eventos del visor describen la actividad de los usuarios que desea registrar en los informes.
* Adobe Las variables de Dynamic Media Classic describen los datos sobre los eventos de usuario que desea que envíen los informes.

La pantalla de configuración de Adobe Analytics también incluye herramientas para activar, editar y eliminar eventos de visor.

Después de seleccionar **[!UICONTROL Guardar]** en la página Configuración de Adobe Analytics, se inserta un código de seguimiento personalizado para la medición de la actividad del usuario en los visores de Dynamic Media Classic de Adobe. Esta funcionalidad permite realizar el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics.

Consulte [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publique los visores de Adobe Dynamic Media Classic

Publique los visores de Adobe de Dynamic Media Classic para que los visualizadores (con código para el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics) se carguen en los servidores de Adobe Dynamic Media Classic. Después de la publicación, esta información se incluye en los visores y puede emplearse en los análisis de Adobe Analytics.

Consulte [Publicar información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Coloque los visores de Adobe Dynamic Media Classic en su sitio web

Coloque los visores de Adobe Dynamic Media Classic con código de seguimiento de Adobe Analytics en el sitio web.

## 5. Pruebe la integración de Adobe Analytics consultando un informe de Adobe Analytics

Para ver los informes de Adobe Analytics, visite el sitio web de Adobe Analytics. En la página de informes puede consultar los datos y generar gráficos y diagramas para medir la actividad de los usuarios con diferentes visores. 

Consulte [Probar la integración de Adobe Analytics viendo un informe de Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
