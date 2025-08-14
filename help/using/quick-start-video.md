---
title: 'Inicio rápido: Vídeo en Adobe Dynamic Media Classic'
description: Introducción y Inicio rápido del vídeo de Adobe Dynamic Media Classic para ayudarle a ponerse en marcha rápidamente.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 24%

---

# Inicio rápido: Vídeo en Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video es una solución integral que facilita la publicación de vídeos adaptables de alta calidad para su transmisión por streaming en varias pantallas, incluidos dispositivos de escritorio, iOS, Android™, BlackBerry® y Windows® para dispositivos móviles. Los conjuntos de vídeos adaptables agrupan versiones del mismo vídeo codificadas con una velocidad de bits y un formato diferentes, por ejemplo, 400 kbps, 800 kbps y 1.000 kbps. El ordenador de escritorio o dispositivo móvil detecta el ancho de banda disponible.

Por ejemplo, en un dispositivo móvil iOS, detecta un ancho de banda de, por ejemplo, 3G, 4G o Wi-Fi. A continuación, selecciona de forma automática el vídeo codificado correcto de las diversas velocidades de bits que incluye el conjunto de vídeos adaptable. El vídeo se transmite a equipos de escritorio, dispositivos móviles o tablets.

Además, la calidad de vídeo se cambia dinámicamente de forma automática si las condiciones de la red cambian en el equipo de escritorio o en el dispositivo móvil. Además, si un cliente entra en modo de pantalla completa en un equipo de escritorio, el conjunto de vídeos adaptable responde con una mejor resolución, lo que mejora la experiencia de visualización del cliente. El uso de conjuntos de vídeos adaptables proporciona la mejor reproducción posible. Es mejor para los clientes que reproducen Adobe Dynamic Media Classic Video en varias pantallas y dispositivos.

La lógica que un reproductor de vídeo utiliza para determinar qué vídeo codificado se debe reproducir o seleccionar durante la reproducción se basa en el siguiente algoritmo:

1. El reproductor de vídeo carga el fragmento de vídeo inicial en función de la velocidad de bits más cercana al valor establecido para &quot;velocidad de bits inicial&quot; en el propio reproductor.
1. El reproductor de vídeo cambia según los cambios en la velocidad del ancho de banda según los siguientes criterios:

   1. El reproductor elige el flujo de ancho de banda más alto por debajo o igual al ancho de banda estimado.
   1. El reproductor considera solo el 80% del ancho de banda disponible. Sin embargo, si está subiendo, es más conservador en solo el 70% para evitar la sobreestimación y volver inmediatamente.

Consulte la lógica del algoritmo en [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obtener información técnica al respecto.

Para administrar vídeos únicos y conjuntos de vídeos adaptables, Adobe Dynamic Media Classic admite lo siguiente:

* Carga de vídeo desde varios formatos de vídeo compatibles. Y, cargar formatos de audio y codificar vídeo a formato MP4 H.264 para su reproducción en varias pantallas. Puede utilizar ajustes preestablecidos de Adobe Dynamic Media Classic Adaptive Video, ajustes preestablecidos de codificación de vídeo únicos o personalizar su propia codificación para controlar la calidad y el tamaño del vídeo.

Consulte [Activar o desactivar ajustes preestablecidos de vídeo adaptables](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Consulte también [Ajustes preestablecidos de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de formación.

Cuando se genera un conjunto de vídeos adaptable, incluye vídeos MP4.

>[!NOTE]
>
>Los vídeos principales/de origen y cualquier otro vídeo en formato de origen *no* se han agregado a un conjunto de vídeos adaptable.

* Subtítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light y navegación de capítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light.

  Ver [Agregar subtítulos a un vídeo](adding-captions-video.md).

  Ver [Agregar marcadores de capítulo a un vídeo](adding-chapter-markers-video.md).

* Organice, explore o busque vídeos con total compatibilidad de metadatos para gestionar eficazmente sus recursos de vídeo. 
* Ofrezca conjuntos de vídeos adaptables a la web y a equipos de escritorio y dispositivos móviles, incluidos iPhone, iPad, Android™, BlackBerry® y Windows® phone.

  La transmisión de vídeo adaptable es compatible con varias plataformas de iOS.

  Consulte la compatibilidad más reciente en la [Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/es/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP4 H.264. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Puede encontrar dispositivos Windows® compatibles con este formato de vídeo en los siguientes enlaces:

  [Formatos de vídeo compatibles con Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Reproduzca el vídeo con los ajustes preestablecidos del visualizador de Adobe Dynamic Media Classic, incluidos los siguientes:

   * Visualizadores de vídeo únicos.
   * Visores de medios mixtos que combinan contenido de vídeo y de imagen.

* Configuración de reproductores de vídeo para cumplir las necesidades de marca.
* Integre vídeo en su sitio web, sitio móvil o aplicación móvil con una URL simple o un código incrustado.

Consulte los siguientes vídeos de formación:
* [Descripción general del vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Vista previa de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Carga de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Resumen de transmisión](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Inicio rápido**

La siguiente descripción paso a paso del flujo de trabajo se ha diseñado para ayudarle a ponerse en marcha rápidamente con los conjuntos de vídeos adaptables en Adobe Dynamic Media Classic. Después de cada paso, se hace una referencia cruzada a un encabezado de tema donde puede encontrar más información.

## &#x200B;1. Cargue y codifique vídeos

Cargue y genere conjuntos de vídeos adaptables con una de los dos situaciones siguientes:

* **Cargar vídeos precodificados**: Si tus vídeos ya se han codificado externamente desde Adobe Dynamic Media Classic, en la barra de navegación global, selecciona **[!UICONTROL Cargar]**. Explore y cargue archivos de vídeo MP4 directamente en Adobe Dynamic Media Classic. A continuación, vaya a **[!UICONTROL Compilación]** > **[!UICONTROL Conjuntos de vídeos adaptables]**. Busque los archivos de vídeo. Arrastre y suelte los archivos de vídeo que desee en la tabla Conjunto de vídeos adaptable y, a continuación, guarde el conjunto.
* **Cargar vídeos de origen principal**: Si los vídeos no están codificados, en la barra de navegación global, selecciona **[!UICONTROL Cargar]** para cargar los archivos de origen del vídeo principal (que no sean MP4). Adobe Dynamic Media Classic los codifica en archivos MP4 por usted. En el cuadro de diálogo **[!UICONTROL Cargar opciones del trabajo]**, en **[!UICONTROL Opciones de vídeo electrónico]**, seleccione **[!UICONTROL Vídeo adaptable]**.

  Con esta opción preferida, puede crear conjuntos de vídeos adaptables. El ajuste preestablecido de codificación correcto se aplica automáticamente al vídeo, ya sea 16:9 o 4:3, para que coincida con las dimensiones del vídeo que ha cargado. Al enviar el trabajo de carga, se crea automáticamente un conjunto de vídeos adaptable que incluye tres ajustes de codificación de vídeo en la relación de aspecto correcta.

  O bien, en el mismo cuadro de diálogo **[!UICONTROL Opciones de trabajo]**, en **[!UICONTROL Opciones de vídeo electrónico]**, expanda **[!UICONTROL Ajustes preestablecidos de codificación única]**. Seleccione los ajustes preestablecidos de codificación de vídeo individuales que desee. Puede seleccionar **Escritorio**, **Móvil (iPhone, iPad, Android™)** y **Tablet (iPad, Android™)** para crear los archivos MP4.

* O bien, puede volver a procesar un vídeo principal mediante la función **[!UICONTROL Reprocesando]**. Los vídeos recién codificados se añaden al Conjunto de vídeos adaptable existente.

Ver [Cargar y codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

Adobe Dynamic Media Classic ofrece numerosos ajustes preestablecidos de codificación de vídeo predefinidos. Estos ajustes preestablecidos reflejan los ajustes de codificación de vídeo más comunes utilizados hoy en día y están optimizados para su reproducción en páginas de destino.

Sin embargo, si es necesario personalizar más el proyecto, los administradores pueden crear ajustes preestablecidos de vídeo para personalizar el tamaño y la reproducción de vídeos para los usuarios finales. Los administradores pueden agregar y administrar ajustes preestablecidos de vídeo desde la página Ajustes preestablecidos de vídeo, disponible en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]** > **[!UICONTROL Ajustes preestablecidos de codificación única]**. La página Ajustes preestablecidos de vídeo contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de vídeo.

Consulte [Trabajar con ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## &#x200B;2. Vista previa de vídeos en un visor de vídeos

Para ver cómo se reproduce un vídeo para los usuarios finales en un escritorio, un sitio web o un dispositivo móvil, seleccione el vídeo en el panel Examinar. Luego selecciona **[!UICONTROL Vista previa]**.

Ver [Vista previa de vídeos en un visor de vídeos](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Puede reproducir el vídeo en la página Vista previa. También puede elegir diferentes visores de vídeo para averiguar cómo aparece el vídeo en diferentes reproductores. La práctica recomendada es utilizar el reproductor de vídeo HTML5 para la reproducción multipantalla en escritorios, tablets y dispositivos móviles.

**Opcional**

Personalización de ajustes preestablecidos de visualizador: Adobe Dynamic Media Classic ofrece ajustes preestablecidos de visualizador para la entrega de vídeo. Estos ajustes preestablecidos determinan la apariencia del visor y cómo funcionan los controles de reproducción. Para personalizar el visor de vídeo, los administradores pueden agregar y gestionar ajustes preestablecidos de visor desde la página Ajustes preestablecidos de visor. Para abrir esta página, en la esquina superior derecha de Adobe Dynamic Media Classic, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**. La página Ajustes preestablecidos de visor contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de visor.

Consulte [Trabajar con ajustes preestablecidos del visor de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Consulte también [Ajustes preestablecidos de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de formación.

## &#x200B;3. Implementar vídeos en sus sitios web y sitios móviles

Para incorporar el vídeo en el sitio web, puede realizar cualquiera de las acciones siguientes:

* Muestre el vídeo en su propia ventana emergente o modal, en cuyo caso use la función **[!UICONTROL Copiar URL]**.

  Para obtener la dirección URL de un vídeo, en las vistas Cuadrícula o Lista, selecciónelo en el panel Examinar. Seleccione **[!UICONTROL Vista previa]** y, a continuación, seleccione **[!UICONTROL Copiar URL]** a la derecha de `Universal_HTML5_Viewer`.

  Al seleccionar **[!UICONTROL Copiar URL]**, la URL se copia en el Portapapeles. Coloque este código en el HTML de su sitio web, sitio móvil o aplicación. 

  >[!NOTE]
  >
  >Las direcciones URL solo se activan tras publicar el vídeo o el conjunto de vídeos adaptables.

* Muestre el vídeo incrustado en la página web, en cuyo caso use la característica **[!UICONTROL Código incrustado]**.

  Para obtener el código incrustado de un vídeo, en las vistas de cuadrícula o de lista, seleccione el vídeo en el panel Examinar. Vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**. En la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]** a la derecha de `Universal_HTML5_Video`. No se permite editar el código.

  Seleccione **[!UICONTROL Cerrar]** y pegue el código incrustado en una o varias de sus páginas web.

  >[!NOTE]
  >
  >El código incrustado solo se activa después de publicar el vídeo o el conjunto de vídeos adaptable.

Ver [Implementar vídeo en sus sitios web y sitios móviles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)
