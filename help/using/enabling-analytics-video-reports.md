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
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Activar informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Con los informes de vídeo basados en Adobe Analytics Heartbeat, ya no es necesario activar los cuatro eventos de visualizador de vídeo (Reproducir, Pausa, Detener, Hito) al configurar Adobe Analytics en Adobe Dynamic Media Classic. Video Heartbeat funciona con los visores de vídeo y medios mixtos predeterminados de Adobe Dynamic Media Classic HTML5. El reproductor de vídeo genera datos de seguimiento para verlos en informes de vídeo de Adobe Analytics.

* Para ver una introducción a los medios de streaming y la &quot;medición de latidos&quot;, consulta [Acerca de Adobe Analytics para mídia de streaming](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* La integración de informes de vídeo de Adobe Analytics con Adobe Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

  Consulte [Parámetros de audio y vídeo](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) para obtener más información sobre las variables de solución y las variables personalizadas.

* Se admiten segmentos listos para usar de incrementos de un minuto. Sin embargo, no se admiten los informes de segmentos personalizados, como los hitos definidos por el cliente en función de incrementos de tiempo, hitos de % o hitos de desplazamiento.

  Para obtener más información acerca de los requisitos y la configuración de los medios de transmisión, vea [Medir los medios de transmisión en Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Para obtener información acerca de las variables personalizadas y de solución, vea [Habilitación de informes de contenidos](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Si la solución con licencia de Adobe Analytics no incluye Video Heartbeat, siga utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visualizador de Adobe Dynamic Media Classic.
