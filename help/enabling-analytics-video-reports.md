---
title: Activación de los informes de vídeo de Adobe Analytics
description: Obtenga información sobre cómo habilitar los informes de vídeo de Adobe Analytics.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 20%

---


# Activación de los informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Al utilizar el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, ya no es necesario activar los cuatro eventos del visor de vídeo (Reproducir, Pausa, Detener o Hito) al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores integrados de medios mixtos y vídeo HTML5 de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics.

* Para obtener una introducción a los medios de flujo continuo y la &quot;medición de latidos&quot;, consulte [Acerca de Adobe Analytics para medios de flujo](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* La integración de los informes de vídeo de Adobe Analytics con Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

   Consulte [Parámetros de audio y vídeo](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) para obtener más información sobre variables de solución y variables personalizadas.

* Se admiten los segmentos listos para usar en incrementos de un minuto. Sin embargo, no se admiten los informes de segmento personalizados, como hitos definidos por el usuario basados en períodos temporales, % de hitos o hitos de desplazamiento.

   Para obtener más información sobre los requisitos y la configuración de medios de flujo, consulte [Medición de medios de flujo en Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Para obtener información sobre las variables personalizadas y de solución, consulte [Habilitación de informes de medios](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Si la solución con licencia de Adobe Analytics no incluye Video Heartbeat, deberá seguir utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visor de Dynamic Media Classic.

