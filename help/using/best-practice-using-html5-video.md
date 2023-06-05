---
title: Práctica recomendada para utilizar el visualizador de vídeo HTML5
description: Conozca las prácticas recomendadas para utilizar el visualizador de vídeo HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 12%

---

# Prácticas recomendadas para utilizar el visualizador de vídeo HTML5{#best-practice-using-the-html-video-viewer}

Los ajustes preestablecidos del visualizador de vídeo Adobe Dynamic Media Classic HTML5 son reproductores de vídeo sólidos. En el lado del diseño del reproductor, puede crear toda la funcionalidad del reproductor de vídeo con las herramientas de desarrollo web estándar. Por ejemplo, se pueden diseñar los botones, controles y el fondo de imagen de póster personalizado utilizando HTML5 y CSS para ayudarle a captar clientes con un aspecto personalizado.

En la parte de reproducción del visor, se detecta de forma automática la funcionalidad de vídeo del navegador. A continuación, sirve el vídeo mediante HLS (flujo en directo HTTP), también conocido como flujo de vídeo adaptable. O bien, si ese método de envío no está presente, se utiliza HTML 5 progresivo en su lugar.

Al combinar en un solo jugador las siguientes habilidades:

* Componentes de reproducción diseñados con HTML5 y CSS
* Reproducción integrada
* Uso de flujo adaptable y progresivo basado en la capacidad del explorador

El alcance del contenido multimedia enriquecido se amplía a los usuarios de equipos de escritorio y dispositivos móviles. También garantiza una experiencia de vídeo optimizada.

Consulte también [Acerca de los visores HTML 5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) en la Guía de referencia de visores de Adobe.

Consulte también [Ajustes preestablecidos de visor](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vídeo de formación.

## Reproducción de vídeo en equipos de escritorio y dispositivos móviles mediante el Visor de vídeo de Adobe Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

En el caso de la transmisión de vídeo adaptable de escritorio y móvil, los vídeos utilizados para la conmutación de velocidad de bits se basan en todos los vídeos MP4 del conjunto de vídeos adaptable.

La reproducción de vídeo se produce mediante HLS o vídeo progresivo. HLS (HTTP Live Streaming) es un estándar de Apple para el streaming de vídeo adaptable que ajusta automáticamente la reproducción en función de la capacidad del ancho de banda de la red. También permite al cliente &quot;buscar&quot; cualquier punto del vídeo sin necesidad de esperar a que se descargue el resto del vídeo. Consulte también [HTTP Live Streaming](https://developer.apple.com/streaming/). El vídeo progresivo se proporciona descargando y almacenando el vídeo localmente en la pantalla de escritorio o el dispositivo móvil del usuario.

En la tabla siguiente se describe el dispositivo, el navegador y el método de reproducción de vídeos en equipos de escritorio y dispositivos móviles mediante el Visor de vídeo de Adobe Dynamic Media Classic.

| Dispositivo | Explorador | Modo de reproducción de vídeo |
|--- |--- |--- |
| Ordenador | Internet Explorer 9 y 10 | Descarga progresiva. |
| Ordenador | Internet Explorer 11+ | Flujo de vídeo HLS. |
| Ordenador | Firefox 23-44 | Descarga progresiva. |
| Ordenador | Firefox 45 o posterior | Flujo de vídeo HLS. |
| Ordenador | Chrome | Flujo de vídeo HLS. |
| Ordenador | Safari (Mac) | Flujo de vídeo HLS. |
| Dispositivos portátiles | Chrome (Android™ 6 o anterior) | Descarga progresiva. |
| Dispositivos portátiles | Chrome (Android™ 7 o posterior) | Flujo de vídeo HLS. |
| Dispositivos portátiles | Android™ (explorador predeterminado) | Descarga progresiva. |
| Dispositivos portátiles | Safari (iOS) | Flujo de vídeo HLS. |
| Dispositivos portátiles | Chrome (iOS) | Flujo de vídeo HLS. |
| Dispositivos portátiles | Blackberry® | Flujo de vídeo HLS. |
