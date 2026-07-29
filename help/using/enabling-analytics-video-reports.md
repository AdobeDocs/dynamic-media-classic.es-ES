---
title: Activar informes de vídeo de Adobe Analytics
description: Obtenga información sobre cómo habilitar informes de vídeo de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: a157ef90a1ff3051fe0939b859d1ba7a63537b82
workflow-type: tm+mt
source-wordcount: 265
ht-degree: 0%

---

# Activar informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Con los informes de vídeo basados en Adobe Analytics Heartbeat, ya no es necesario habilitar los cuatro eventos de visualizador de vídeo (Reproducir, Pausa, Detener, Hito) al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con visores de vídeo y medios mixtos estándar de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en informes de vídeo de Adobe Analytics.

* Para ver una introducción a los medios de streaming y la &quot;medición de latidos&quot;, consulta [Acerca de Adobe Analytics para medios de streaming](https://experienceleague.adobe.com/es/docs/media-analytics/using/media-overview).

* La integración de informes de vídeo de Adobe Analytics con Adobe Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

  Consulte [Parámetros de audio y vídeo](https://experienceleague.adobe.com/es/docs/media-analytics/using/reporting/dimensions/overview) para obtener más información sobre las variables de solución y las variables personalizadas.

* Se admiten segmentos estándar de incrementos de un minuto. Sin embargo, no se admiten los informes de segmentos personalizados, como los hitos definidos por el cliente en función de incrementos de tiempo, hitos de % o hitos de desplazamiento.

  Para obtener más información acerca de los requisitos y la configuración de los medios de transmisión, consulte [Medir los medios de transmisión en Adobe Analytics](https://experienceleague.adobe.com/es/docs/media-analytics/using/media-overview).

* Para obtener información acerca de las variables personalizadas y de solución, vea [Habilitación de informes de contenidos](https://experienceleague.adobe.com/es/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/media-management).

>[!NOTE]
>
>Si la solución con licencia de Adobe Analytics no incluye Video Heartbeat, siga utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic.
