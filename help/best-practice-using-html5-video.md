---
title: '"Práctica recomendada: Uso del visor de vídeo HTML5"'
seo-title: '"Práctica recomendada: Uso del visor de vídeo HTML5"'
description: nulo
seo-description: Obtenga información sobre las prácticas recomendadas para utilizar el visor de vídeo HTML 5.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64 b
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/video
discoiquuid: 4 b 11 cab 7-88 cf -42 dd -8554-2 eea 530753 bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Práctica recomendada: Uso del visor de vídeo HTML5{#best-practice-using-the-html-video-viewer}

Los ajustes preestablecidos del visor de vídeo HTML 5 de Dynamic Media Classic son reproductores de vídeo sólidos. En el lado de diseño del reproductor, puede crear toda la funcionalidad del reproductor de vídeo utilizando herramientas de desarrollo web estándar. Por ejemplo, se pueden diseñar los botones, controles y el fondo de imagen de póster personalizado utilizando HTML5 y CSS para ayudarle a captar clientes con un aspecto personalizado.

En la parte de reproducción del visor, se detecta de forma automática la funcionalidad de vídeo del navegador. A continuación, proporciona el vídeo usando HLS (flujo continuo de vídeo adaptable). O bien, si el método de entrega no está presente, se utilizará en su lugar HTML 5 progresivo.

Al combinar en un solo reproductor la capacidad para diseñar los componentes reproducción mediante HTML5 y CSS, tener la reproducción incorporada y usar flujo adaptable y progresivo en función de la capacidad del navegador, se amplía el alcance del contenido de medios enriquecidos para los usuarios móviles y escritorio y se garantiza una experiencia optimizada de vídeo.

Consulte también [Acerca de los visores](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) HTML 5 en la Guía de referencia de visores de Adobe.

## Reproducción de vídeo en equipos de escritorio y dispositivos móviles mediante el visor de vídeos clásico de Media Media Classic {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Para el flujo continuo de vídeo adaptable móvil y de escritorio, los vídeos utilizados para el cambio de velocidad de bits se basan en todos los vídeos MP 4 del conjunto de vídeos adaptable.

La reproducción de vídeo se produce mediante HLS o vídeo progresivo. HLS (HTTP Live Streaming) es un estándar Apple para el flujo de vídeo adaptable que ajusta automáticamente la reproducción en función de la capacidad de ancho de banda de la red. También permite al cliente «buscar» en cualquier punto del vídeo sin necesidad de esperar a que se descargue el resto del vídeo (consulte también [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/)). El vídeo progresivo se entrega descargando y almacenando el vídeo localmente en la pantalla de escritorio o dispositivo móvil del usuario.

En la siguiente tabla se describe el dispositivo, el navegador y el método de reproducción de vídeos en equipos de escritorio y dispositivos móviles con el visor de vídeo clásico de Media Media Classic.

| Dispositivo | Explorador | Modo de reproducción de vídeo |
|--- |--- |--- |
| Deskop | Internet Explorer 9 y 10 | Descarga progresiva. |
| Ordenador | Internet Explorer 11 + | Flujo continuo de vídeo HLS. |
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
