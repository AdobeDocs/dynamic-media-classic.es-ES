---
title: Activar informes de vídeo de Adobe Analytics
description: Obtenga información sobre cómo habilitar informes de vídeo de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 5%

---

# Activar informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Con los informes de vídeo basados en Adobe Analytics Heartbeat, ya no es necesario activar los cuatro eventos de visualizador de vídeo (Reproducir, Pausa, Detener, Hito) al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics.

* Para ver una introducción a los medios de streaming y la &quot;medición de latidos&quot;, consulte [Acerca de Adobe Analytics para mídia de streaming](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* La integración de informes de vídeo de Adobe Analytics con Adobe Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

  Consulte [Parámetros de audio y vídeo](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) para obtener más información sobre las variables de solución y las variables personalizadas.

* Se admiten segmentos listos para usar de incrementos de un minuto. Sin embargo, no se admiten los informes de segmentos personalizados, como los hitos definidos por el cliente en función de incrementos de tiempo, hitos de % o hitos de desplazamiento.

  Para obtener más información sobre los requisitos y la configuración de los medios de streaming, consulte [Medición de Streaming Media en Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Para obtener información sobre las variables personalizadas y de solución, consulte [Habilitación de informes de contenidos](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Si la solución con licencia de Adobe Analytics no incluye Video Heartbeat, debe seguir siguiendo los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic.
