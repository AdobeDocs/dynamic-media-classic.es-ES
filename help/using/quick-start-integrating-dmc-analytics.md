---
title: "Inicio rápido: Integración de Adobe Dynamic Media Classic y Adobe Analytics"
description: Introducción y Inicio rápido sobre cómo integrar Adobe Dynamic Media Classic y Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 21%

---

# Inicio rápido: Integrar Adobe Dynamic Media Classic y Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics es un producto líder de la industria que ofrece a los vendedores un lugar donde pueden medir, analizar y optimizar datos integrados de todas las iniciativas en línea a través de múltiples canales de marketing.

Después de integrar Adobe Analytics con Adobe Dynamic Media Classic, puede obtener informes sobre el comportamiento de los visitantes del sitio web mediante los visores de Adobe Dynamic Media Classic en el sitio web. Por ejemplo, cuando un visitante de un sitio web selecciona un destino de zoom en un visor de zoom de Adobe Dynamic Media Classic, Adobe Analytics registra esta acción. Los informes de Adobe Analytics pueden recopilar información acumulativa sobre la actividad del usuario en los visualizadores de Adobe Dynamic Media Classic.

Con el uso de los informes de Adobe Analytics, podrá obtener una imagen clara de la actividad de los clientes en su sitio web. Puede determinar qué presentaciones de productos generan una conversión y cuáles no atraen el interés de los clientes.

Consulte también [Medir vídeo en Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Se necesita una cuenta de Adobe Analytics válida para integrar Analytics con Adobe Dynamic Media Classic y generar informes de Analytics.

Este inicio rápido está diseñado para ayudarle a empezar rápidamente con el kit de instrumentación de Adobe Analytics.

## 1. Inicie sesión en Adobe Analytics mediante Adobe Dynamic Media Classic y descargue las variables del informe de Adobe Analytics

>[!NOTE]
>
>Compruebe que se le agrega como miembro del grupo Acceso a servicio Web en Adobe Analytics. Antes de configurar los informes de Adobe Analytics, realice esta verificación. Y antes de relacionar las variables de informes de Adobe Analytics con los eventos de Adobe Dynamic Media Classic. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados. Puede hacerlo mediante la API de servicios web del Experience Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, vaya a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Después de comprobar que es miembro del grupo Acceso a servicio Web, vaya a Adobe Dynamic Media Classic **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Adobe Analytics]**. En la página Configuración de Adobe Analytics, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.

Consulte [Iniciar sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

En el cuadro de diálogo Inicio de sesión de Adobe Analytics, escriba su ID de organización de Experience Cloud (opcional), sus credenciales completas y, a continuación, seleccione **[!UICONTROL Iniciar sesión]**. En el menú desplegable Grupo de informes, seleccione el nombre del grupo de informes que desee utilizar.

## 2. Asigne variables de informes de Adobe Analytics a eventos de visualizador de Adobe Dynamic Media Classic y variables de Adobe Dynamic Media Classic

En la página de configuración de Adobe Analytics, especifique la información que desee incluir en los informes de Adobe Analytics. Para cada evento de visualizador de Adobe Dynamic Media Classic del que desee obtener información, elija una variable de Adobe Analytics (del grupo de informes) y una variable de Adobe Dynamic Media Classic.

* Los eventos del visor describen la actividad de los usuarios que desea registrar en los informes.
* Las variables de Adobe Dynamic Media Classic describen los datos acerca de los eventos de usuario que desea que proporcionen los informes.

La pantalla de configuración de Adobe Analytics también incluye herramientas para activar, editar y eliminar eventos de visor.

Después de seleccionar **[!UICONTROL Guardar]** en la página Configuración de Adobe Analytics, se inserta un código de seguimiento personalizado para medir la actividad del usuario en los visores de Adobe Dynamic Media Classic. Esta funcionalidad permite realizar el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics.

Consulte [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publique sus visores de Adobe Dynamic Media Classic

Publique sus visores de Adobe Dynamic Media Classic para que los visores de (con código para rastrear la actividad de los usuarios en los informes de Adobe Analytics) se carguen en los servidores de Adobe Dynamic Media Classic. Después de la publicación, esta información se incluye en los visualizadores. Utilícelo para el análisis por parte de Adobe Analytics.

Consulte [Publicar información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Coloque los visores de Adobe Dynamic Media Classic en el sitio web

Coloque los visores de Adobe Dynamic Media Classic con código de seguimiento de Adobe Analytics en el sitio web.

## 5. Pruebe la integración de Adobe Analytics consultando un informe de Adobe Analytics

Para ver los informes de Adobe Analytics, visite el sitio web de Adobe Analytics. En la página de informes puede consultar los datos y generar gráficos y diagramas para medir la actividad de los usuarios con diferentes visores. 

Consulte [Prueba de la integración de Adobe Analytics mediante la visualización de un informe de Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
