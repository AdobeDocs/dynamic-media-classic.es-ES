---
title: Activación de los informes de vídeo de Adobe Analytics
description: Obtenga información sobre cómo habilitar los informes de vídeo de Adobe Analytics.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 23%

---


# Activación de los informes de vídeo de Adobe Analytics{#enabling-adobe-analytics-video-reports}

Al utilizar el sistema de informes de vídeo basado en Adobe Analytics Heartbeat, ya no es necesario activar los cuatro eventos del visor de vídeo (Reproducir, Pausa, Detener o Hito) al configurar Adobe Analytics en Dynamic Media Classic. Video Heartbeat funciona con los visores integrados de medios mixtos y vídeo HTML5 de Dynamic Media Classic. El reproductor de vídeo genera el seguimiento de datos para visualizarlos dentro de los informes de vídeo de Adobe Analytics.

* La integración de los informes de vídeo de Adobe Analytics con Dynamic Media Classic admite variables de solución, pero no variables personalizadas.

   Consulte [Configuración del Sistema de informes de vídeo de Analytics](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) para obtener más información sobre variables de solución y variables personalizadas.

* Se admiten los segmentos listos para usar en incrementos de un minuto. Sin embargo, no se admiten los informes de segmento personalizados, como hitos definidos por el usuario basados en períodos temporales, % de hitos o hitos de desplazamiento.

Para obtener más información sobre los requisitos y la configuración de Video Heartbeat, consulte [Medición de vídeo en Adobe Analytics mediante Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Si la solución con licencia de Adobe Analytics no incluye Video Heartbeat, deberá seguir utilizando los pasos descritos en este capítulo para asignar variables de Adobe Analytics a eventos y variables de visor de Dynamic Media Classic.

