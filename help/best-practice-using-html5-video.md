---
title: Práctica recomendada para utilizar el visor de vídeo HTML5
description: Obtenga información sobre las prácticas recomendadas para utilizar el visor de vídeo HTML5.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 26%

---


# Prácticas recomendadas para utilizar el visor de vídeo HTML5{#best-practice-using-the-html-video-viewer}

Los ajustes preestablecidos del visor de vídeo HTML5 de Dynamic Media Classic son reproductores de vídeo sólidos. En el lado de diseño del reproductor, puede crear toda la funcionalidad del reproductor de vídeo con herramientas de desarrollo web estándar. Por ejemplo, se pueden diseñar los botones, controles y el fondo de imagen de póster personalizado utilizando HTML5 y CSS para ayudarle a captar clientes con un aspecto personalizado.

En la parte de reproducción del visor, se detecta de forma automática la funcionalidad de vídeo del navegador. A continuación, se muestra el vídeo mediante HLS (flujo de vídeo adaptable). O bien, si ese método de envío no está presente, se utiliza HTML5 progresivo en su lugar.

Al combinar en un solo reproductor la capacidad para diseñar los componentes reproducción mediante HTML5 y CSS, tener la reproducción incorporada y usar flujo adaptable y progresivo en función de la capacidad del navegador, se amplía el alcance del contenido de medios enriquecidos para los usuarios móviles y escritorio y se garantiza una experiencia optimizada de vídeo.

Consulte también [Acerca de los visores HTML5](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) en la Guía de referencia de visores de Adobe.

## Reproducción de vídeo en equipos de escritorio y dispositivos móviles mediante el visor de vídeo Dynamic Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para el flujo continuo de vídeo adaptable móvil y de escritorio, los vídeos utilizados para el cambio de velocidad de bits se basan en todos los vídeos MP4 del conjunto de vídeos adaptable.

La reproducción de vídeo se produce mediante HLS o vídeo progresivo. HLS (HTTP Live Streaming) es un estándar de Apple para el flujo de vídeo adaptable que ajusta automáticamente la reproducción en función de la capacidad de ancho de banda de la red. También permite al cliente &quot;buscar&quot; en cualquier punto del vídeo sin necesidad de esperar a que se descargue el resto del vídeo. Consulte también [HTTP Live Streaming](https://developer.apple.com/streaming/). El vídeo progresivo se entrega descargando y almacenando el vídeo localmente en la pantalla de escritorio o en el dispositivo móvil del usuario.

En la tabla siguiente se describe el dispositivo, el navegador y el método de reproducción de vídeos en equipos de escritorio y dispositivos móviles que utilizan el visor de vídeo Dynamic Media Classic.

| Dispositivo | Explorador | Modo de reproducción de vídeo |
|--- |--- |--- |
| Escritorio | Internet Explorer 9 y 10 | Descarga progresiva. |
| Ordenador | Internet Explorer 11+ | Flujo continuo de vídeo HLS. |
| Ordenador | Firefox 23-44 | Descarga progresiva. |
| Ordenador | Firefox 45 o posterior | Flujo continuo de vídeo HLS. |
| Ordenador | Chrome | Flujo continuo de vídeo HLS. |
| Ordenador | Safari (Mac) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Chrome (Android 6 o anterior) | Descarga progresiva. |
| Dispositivos portátiles | Chrome (Android 7 o posterior) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Android (navegador predeterminado) | Descarga progresiva. |
| Dispositivos portátiles | Safari (iOS) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Chrome (iOS) | Flujo continuo de vídeo HLS. |
| Dispositivos portátiles | Blackberry | Flujo continuo de vídeo HLS. |
