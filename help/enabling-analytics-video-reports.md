---
title: Activación de los informes de vídeo de Adobe Analytics
seo-title: Activación de los informes de vídeo de Adobe Analytics
description: nulo
seo-description: Obtenga información sobre cómo activar los informes de vídeo de Adobe Analytics.
uuid: 078594 b 2-7 d 53-4714-8128-ff 3 b 5 c 3 a 5 e 36
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 18644 a 53-92 da -40 ab-b 961-318 d 8332 c 54 d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Activación de los informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Al utilizar los informes de vídeo basados en Heartbeat de Adobe Analytics, ya no necesita activar los cuatro eventos de visor de vídeo (Reproducir, Pausa, Detener, Hito) al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores de medios mixtos tradicionales de Media Media Classic y HTML 5. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics.

* La integración de los informes de vídeo de Adobe Analytics con Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

   Consulte [Configuración de informes de vídeo de Analytics](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) para obtener más información sobre variables de soluciones y variables personalizadas.

* Se admiten los segmentos listos para usar en incrementos de un minuto. Sin embargo, no se admiten los informes de segmento personalizados, como hitos definidos por el usuario basados en períodos temporales, % de hitos o hitos de desplazamiento.

Para obtener más información sobre los requisitos y la configuración de Video Heartbeat, consulte [Medición de vídeo en Adobe Analytics mediante Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Si su solución con licencia de Adobe Analytics no incluye Video Heartbeat, deberá seguir utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visor de Dynamic Media Classic.

