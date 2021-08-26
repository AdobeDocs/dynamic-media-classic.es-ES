---
title: Habilitar los informes de vídeo de Adobe Analytics
description: Obtenga información sobre cómo habilitar los informes de vídeo de Adobe Analytics en Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# Habilitar los informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Al usar los informes de vídeo basados en Adobe Analytics Heartbeat, ya no es necesario habilitar los cuatro eventos del visor de vídeo (Reproducir, Pausa, Detener, Milestone) al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos y vídeo HTML5 listos para usar de Adobe Dynamic Media Classic . El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics.

* Para obtener una introducción a la transmisión por secuencias de contenidos y a la &quot;medición de latidos&quot;, consulte [Acerca de Adobe Analytics para transmisión por secuencias](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* La integración de informes de vídeo de Adobe Analytics con Adobe Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

   Consulte [Parámetros de audio y vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obtener más información sobre variables de solución y variables personalizadas.

* Se admiten segmentos predeterminados de incrementos de un minuto. Sin embargo, no se admiten los informes de segmento personalizados, como hitos definidos por el usuario basados en períodos temporales, % de hitos o hitos de desplazamiento.

   Para obtener más información sobre los requisitos y la configuración de los medios de transmisión, consulte [Medir medios de transmisión en Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obtener información sobre variables personalizadas y de solución, consulte [Habilitación de informes de medios](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Si la solución de Adobe Analytics con licencia no incluye Video Heartbeat, debe seguir utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a los eventos y variables del visor de Dynamic Media Classic de Adobe.
