---
title: Prueba de la integración viendo un informe de Adobe Analytics
description: Obtenga información sobre cómo probar la integración en Adobe Dynamic Media Classic consultando un informe de Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:14:40.601Z'
TQID: 'https://experienceleague.adobe.com/BwQe9AuhBfi-bLCuO-j48kE-3gw9rgtz5GEI9nIBRjE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 345
ht-degree: 5%

---

# Prueba de la integración viendo un informe de Adobe Analytics{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Después de crear las variables necesarias en Adobe Analytics, vincularlas a eventos de Adobe Dynamic Media Classic y completar los pasos de implementación necesarios, puede probar la configuración. Puede probar y comprobar que los datos se capturan en el propio Adobe Analytics. Si la configuración funciona en SiteCatalyst, no serán necesarios más pasos. Suponiendo que ha seguido los pasos anteriores y ha vinculado los datos de evento de Adobe Dynamic Media Classic a una o más variables de tráfico personalizado, siga este flujo de trabajo para probar los datos dentro de Adobe Analytics.

**Para probar la integración mediante la visualización de un informe de Adobe Analytics:**

1. Inicie un visualizador de Adobe Dynamic Media Classic desde su cuenta, especialmente uno que difunda la métrica que desea obtener e interactúe con él para crear algunos datos de evento.

   Por ejemplo, si desea medir vistas alternativas populares en un conjunto de imágenes, previsualice un conjunto de imágenes y haga clic en las distintas miniaturas de imágenes.

1. En Adobe Analytics, ve a **[!UICONTROL Tráfico personalizado]** > **[!UICONTROL Tráfico personalizado 1-10]** > [Nombre de prop], y selecciona el nombre de la prop de tráfico en las opciones del menú.

   Por ejemplo, para acceder a la propiedad **[!UICONTROL LoadAsset]** en la cuenta de ejemplo, la opción de menú adecuada es **[!UICONTROL Tráfico personalizado]** > **[!UICONTROL Tráfico personalizado 1-10]** > **[!UICONTROL LoadAsset]**. Si tiene más de diez propiedades personalizadas, también verá otras opciones de menú.

1. Consulte la tabla generada por Adobe Analytics. Este gráfico suele ser solo los datos de una única métrica. Si también desea saber con qué recurso están asociados estos datos, obtenga los datos de recursos de este evento. Por ejemplo, a menudo resulta útil saber qué vídeo se ve solo el 50 % o qué imagen de un conjunto es popular.

>[!NOTE]
>
>Todos los datos del visualizador de Adobe Dynamic Media Classic se muestran y se comunican en los informes Tráfico personalizado o Conversión personalizada de Adobe Analytics.

Para obtener más información, consulte [Tutoriales de Analytics](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).