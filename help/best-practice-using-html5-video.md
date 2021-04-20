---
title: Práctica recomendada para utilizar el visor de vídeo HTML5
description: Obtenga información sobre las prácticas recomendadas para utilizar el visor de vídeo HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 13%

---

# Prácticas recomendadas para usar el visor de vídeo HTML5{#best-practice-using-the-html-video-viewer}

Los ajustes preestablecidos del visor de vídeo HTML5 de Dynamic Media Classic son reproductores de vídeo sólidos. En el lado de diseño del reproductor, puede crear toda la funcionalidad del reproductor de vídeo con herramientas de desarrollo web estándar. Por ejemplo, se pueden diseñar los botones, controles y el fondo de imagen de póster personalizado utilizando HTML5 y CSS para ayudarle a captar clientes con un aspecto personalizado.

En la parte de reproducción del visor, se detecta de forma automática la funcionalidad de vídeo del navegador. A continuación, sirve el vídeo utilizando HLS (HTTP Live Streaming), también conocido como flujo de vídeo adaptable. O, si ese método de envío no está presente, se utiliza HTML5 progresiva en su lugar.

Combinando en un solo reproductor las siguientes capacidades:

* Componentes de reproducción diseñados con HTML5 y CSS
* Reproducción incrustada
* Uso de flujo adaptable y progresivo basado en la capacidad del explorador

Puede ampliar el alcance del contenido multimedia enriquecido a los usuarios de escritorio y móviles. También garantiza una experiencia de vídeo optimizada.

Consulte también [Acerca de los visores HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) en la Guía de referencia de visores de Adobe.

## Reproducción de vídeo en equipos de escritorio y dispositivos móviles mediante el visor de vídeo de Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para el streaming de vídeo adaptable móvil y de escritorio, los vídeos utilizados para el cambio de velocidad de bits se basan en todos los vídeos MP4 del conjunto de vídeos adaptables.

La reproducción de vídeo se produce mediante HLS o vídeo progresivo. HLS (HTTP Live Streaming) es un estándar de Apple para el flujo de vídeo adaptable que ajusta automáticamente la reproducción en función de la capacidad de ancho de banda de la red. También permite al cliente &quot;buscar&quot; en cualquier punto del vídeo sin necesidad de esperar a que se descargue el resto del vídeo. Consulte también [Transmisión en directo HTTP](https://developer.apple.com/streaming/). El vídeo progresivo se entrega descargando y almacenando el vídeo localmente en la pantalla de escritorio o el dispositivo móvil del usuario.

En la tabla siguiente se describe el dispositivo, el navegador y el método de reproducción de los vídeos en equipos de escritorio y dispositivos móviles que utilizan el visor de vídeo de Dynamic Media Classic.

| Dispositivo | Explorador | Modo de reproducción de vídeo |
|--- |--- |--- |
| Ordenador | Internet Explorer 9 y 10 | Descarga progresiva. |
| Ordenador | Internet Explorer 11+ | Flujo continuo de vídeo HLS. |
| Ordenador | Firefox 23-44 | Descarga progresiva. |
| Ordenador | Firefox 45 o posterior | Flujo continuo de vídeo HLS. |
| Ordenador | Chrome | Flujo continuo de vídeo HLS. |
| Ordenador | Safari (Mac) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Chrome (Android™ 6 o anterior) | Descarga progresiva. |
| Dispositivos portátiles | Chrome (Android™ 7 o posterior) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Android™ (navegador predeterminado) | Descarga progresiva. |
| Dispositivos portátiles | Safari (iOS) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Chrome (iOS) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Blackberry® | Flujo continuo de vídeo HLS. |
