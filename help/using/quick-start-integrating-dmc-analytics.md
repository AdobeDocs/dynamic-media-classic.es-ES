---
title: 'Inicio rápido: Integrar Adobe Dynamic Media Classic y Adobe Analytics'
description: Introducción y Inicio rápido sobre cómo integrar Adobe Dynamic Media Classic y Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T20:10:08.073Z'
TQID: 'https://experienceleague.adobe.com/DnpXpIqOz1HSLxZAoEOTHG65PSqTWLK7R--OzJj3FcY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: afc1e5c58de547307108448ae111af91f1f482e7
workflow-type: tm+mt
source-wordcount: 690
ht-degree: 17%

---

# Inicio rápido: Integrar Adobe Dynamic Media Classic y Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics es el producto líder del sector que proporciona a los especialistas en marketing una ubicación centralizada en la que pueden medir, analizar y optimizar los datos integrados de todas las iniciativas en línea en varios canales de marketing.

Después de integrar Adobe Analytics con Adobe Dynamic Media Classic, puede obtener informes sobre el comportamiento de los visitantes del sitio web mediante los visores de Adobe Dynamic Media Classic en el sitio web. Por ejemplo, cuando un visitante de un sitio web selecciona un destino de zoom en un visor de zoom de Adobe Dynamic Media Classic, Adobe Analytics registra esta acción. Los informes de Adobe Analytics pueden recopilar información acumulativa sobre la actividad del usuario en los visualizadores de Adobe Dynamic Media Classic.

Con los informes de Adobe Analytics, puede comprender la actividad de los clientes en el sitio web. Puede determinar qué presentaciones de productos generan una conversión y cuáles no atraen el interés de los clientes.

Ver también [Medir vídeo en Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Se necesita una cuenta de Adobe Analytics válida para integrar Analytics con Adobe Dynamic Media Classic y generar informes de Analytics.

Esta guía se ha diseñado para ayudarle a configurar el Kit de instrumentación de Adobe Analytics.

## &#x200B;1. Inicie sesión en Adobe Analytics desde Adobe Dynamic Media Classic y descargue las variables del informe de Adobe Analytics

>[!NOTE]
>
>Compruebe que se le agrega como miembro del grupo Acceso a servicio Web en Adobe Analytics. Realice esta verificación antes de configurar los informes de Adobe Analytics y antes de hacer coincidir las variables de informes de Adobe Analytics con los eventos de Adobe Dynamic Media Classic. Los miembros de este grupo pueden acceder a todos los informes de los grupos de informes especificados. Puede realizar esta acción mediante la API de servicios web de Experience Cloud independientemente de los permisos establecidos en la interfaz. Para agregar un miembro al grupo, en Adobe Analytics, ve a **[!UICONTROL Herramientas de administración]** > **[!UICONTROL Administración de usuarios]** > **[!UICONTROL Editar grupos]**.

Después de comprobar que es miembro del grupo Acceso a servicio web, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Adobe Analytics]** en Adobe Dynamic Media Classic. En la página Configuración de Adobe Analytics, seleccione **[!UICONTROL Inicio de sesión de Adobe Analytics]**.

Ver [Iniciar sesión en Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

En el cuadro de diálogo Inicio de sesión de Adobe Analytics, escriba su ID de organización de Experience Cloud (opcional), sus credenciales completas y, a continuación, seleccione **[!UICONTROL Iniciar sesión]**. En el menú desplegable Grupo de informes, seleccione el nombre del grupo de informes que desee utilizar.

## &#x200B;2. Asignar variables de informes de Adobe Analytics a eventos de visualizador de Adobe Dynamic Media Classic y variables de Adobe Dynamic Media Classic

En la página de configuración de Adobe Analytics, especifique la información que desee incluir en los informes de Adobe Analytics. Para cada evento de visualizador de Adobe Dynamic Media Classic del que desee obtener información, elija una variable de Adobe Analytics (del grupo de informes) y una variable de Adobe Dynamic Media Classic.

* Los eventos del visor describen la actividad de los usuarios que desea registrar en los informes.
* Las variables de Adobe Dynamic Media Classic describen los datos acerca de los eventos de usuario que desea que proporcionen los informes.

La pantalla de configuración de Adobe Analytics también incluye herramientas para activar, editar y eliminar eventos de visor.

Después de seleccionar **[!UICONTROL Guardar]** en la página Configuración de Adobe Analytics, se inserta un código de seguimiento personalizado para medir la actividad del usuario en los visores de Adobe Dynamic Media Classic. Esta funcionalidad permite realizar el seguimiento de la actividad de los usuarios en los informes de Adobe Analytics.

Consulte [Configuración de informes de Adobe Analytics](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## &#x200B;3. Publicación de los visores de Adobe Dynamic Media Classic

Publique sus visores de Adobe Dynamic Media Classic para que los visores de (con código para rastrear la actividad de los usuarios en los informes de Adobe Analytics) se carguen en los servidores de Adobe Dynamic Media Classic. Después de la publicación, esta información se incluye en los visualizadores. Utilícelo para el análisis por parte de Adobe Analytics.

Ver [Publicar información de configuración](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## &#x200B;4. Colocar visores de Adobe Dynamic Media Classic en el sitio web

Coloque los visores de Adobe Dynamic Media Classic con código de seguimiento de Adobe Analytics en el sitio web.

## &#x200B;5. Prueba de la integración de Adobe Analytics mediante un informe de Adobe Analytics

Para ver los informes de Adobe Analytics, visite el sitio web de Adobe Analytics. En la página de informes puede consultar los datos y generar gráficos y diagramas para medir la actividad de los usuarios con diferentes visores.

Ver [Probar la integración de Adobe Analytics al ver un informe de Adobe Analytics](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
