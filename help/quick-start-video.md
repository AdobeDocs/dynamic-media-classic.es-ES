---
title: '"Inicio rápido: Vídeo en Adobe Dynamic Media Classic"'
description: Introducción y Vídeo de inicio rápido de Adobe Dynamic Media Classic para ayudarle a empezar a utilizarlo rápidamente.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1806'
ht-degree: 28%

---

# Inicio rápido: Vídeo en Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video es una solución integral que facilita la publicación de vídeos adaptables de alta calidad para su transmisión en varias pantallas, incluidos equipos de escritorio, iOS, Android™, BlackBerry® y dispositivos móviles Windows®. Los conjuntos de vídeos adaptables agrupan versiones del mismo vídeo codificadas con una velocidad de bits y un formato diferentes, por ejemplo, 400 kbps, 800 kbps y 1.000 kbps. El ordenador de escritorio o dispositivo móvil detecta el ancho de banda disponible.

Por ejemplo, en un dispositivo móvil iOS, detecta un ancho de banda de, por ejemplo, 3G, 4G o Wi-Fi. A continuación, selecciona de forma automática el vídeo codificado correcto de las diversas velocidades de bits que incluye el conjunto de vídeos adaptable. El vídeo se transmite a equipos de escritorio, dispositivos móviles o tablets.

Además, la calidad de vídeo se cambia dinámicamente de forma automática si las condiciones de la red cambian en el equipo de escritorio o en el dispositivo móvil. Además, si un cliente entra en el modo de pantalla completa en un escritorio, el conjunto de vídeos adaptables responde mediante una mejor resolución, lo que mejora la experiencia de visualización del cliente. El uso de conjuntos de vídeos adaptables le ofrece la mejor reproducción posible para los clientes que reproduzcan vídeo de Adobe Dynamic Media Classic en varias pantallas y dispositivos.

La lógica que un reproductor de vídeo utiliza para determinar qué vídeo codificado se debe reproducir o seleccionar durante la reproducción se basa en el siguiente algoritmo:

1. El reproductor de vídeo carga el fragmento de vídeo inicial en función de la velocidad de bits más cercana al valor establecido para la &quot;velocidad de bits inicial&quot; en el propio reproductor.
1. El reproductor de vídeo cambia en función de los cambios en la velocidad de ancho de banda mediante los siguientes criterios:

   1. El reproductor elige el flujo de ancho de banda más alto por debajo o igual al ancho de banda estimado.
   1. El reproductor considera sólo el 80% del ancho de banda disponible. Sin embargo, si está cambiando, es más conservador, con solo el 70%, evitar sobreestimar y tener que volver inmediatamente.

Consulte la lógica del algoritmo en [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obtener información técnica al respecto.

Para administrar conjuntos de vídeos adaptables y de vídeo único, Adobe Dynamic Media Classic admite lo siguiente:

* Carga de vídeos de varios formatos de vídeo y audio compatibles y codificación de vídeo al formato MP4 H.264 para su reproducción en varias pantallas. Puede utilizar ajustes preestablecidos de vídeo adaptables de Adobe Dynamic Media Classic predefinidos, ajustes preestablecidos de codificación de vídeo único o personalizar su propia codificación para controlar la calidad y el tamaño del vídeo.

Consulte [Activación o desactivación de ajustes preestablecidos de vídeo adaptables](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Consulte también el vídeo de formación [Ajustes preestablecidos de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

Cuando se genera un conjunto de vídeos adaptables, incluye vídeos MP4.

>[!NOTE]
>
>Los vídeos principales/de origen y cualquier otro vídeo de formato de origen se *no* agregan a un conjunto de vídeos adaptables.

* Subtítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light y navegación de capítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light.

   Consulte [Agregar subtítulos a vídeo](adding-captions-video.md).

   Consulte [Agregar marcadores de capítulo a vídeo](adding-chapter-markers-video.md).

* Organice, explore o busque vídeos con total compatibilidad de metadatos para gestionar eficazmente sus recursos de vídeo. 
* Entregue conjuntos de vídeos adaptables a la Web y a los equipos de escritorio, así como a los dispositivos móviles, incluidos iPhone, iPad, Android™, BlackBerry® y el teléfono Windows®.

   La transmisión de vídeo adaptable es compatible con varias plataformas de iOS.

   Consulte la compatibilidad más reciente en la [Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP4 H.264. Puede encontrar dispositivos BlackBerry® compatibles con este formato de vídeo en el siguiente sitio web:

   Consulte [Formatos de vídeo compatibles con BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Puede encontrar los dispositivos Windows® compatibles con este formato de vídeo en el siguiente enlace:

   Consulte [Formatos de vídeo compatibles con Windows® Phone](https://docs.microsoft.com/en-us/).

* Reproduzca el vídeo con los ajustes preestablecidos del visor de Adobe Dynamic Media Classic, que incluyen lo siguiente:

   * Visores de vídeos únicos.
   * Visores de medios mixtos que combinan contenido de vídeo y de imagen.

* Configuración de reproductores de vídeo para cumplir las necesidades de marca.
* Integración de vídeo en el sitio web, el sitio móvil o la aplicación móvil con una URL o código incrustado.

Consulte los siguientes vídeos de formación:
* [Información general del vídeo de MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [Vista previa de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [Carga de vídeo MP4](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Información general sobre la transmisión](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Inicio rápido**

La siguiente descripción paso a paso del flujo de trabajo está diseñada para ayudarle a poner en marcha rápidamente los conjuntos de vídeos adaptables en Adobe Dynamic Media Classic. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

## 1. Cargar y codificar vídeos

Cargue y genere conjuntos de vídeos adaptables con una de los dos situaciones siguientes:

* **Cargar vídeos precodificados** : si los vídeos ya estaban codificados fuera de Adobe Dynamic Media Classic, en la barra de navegación global, seleccione  **** Cargar para examinar y cargar archivos de vídeo MP4 directamente en Adobe Dynamic Media Classic. A continuación, vaya a **[!UICONTROL Build]** > **[!UICONTROL Adaptive Video Sets]**. Busque los archivos de vídeo. Arrastre los archivos de vídeo deseados, suéltelos en la tabla Conjunto de vídeos adaptable y, a continuación, guarde el conjunto.
* **Cargar vídeos de origen maestros** : si los vídeos no están codificados, en la barra de navegación global, seleccione  **** Cargar para cargar archivos de origen de vídeo maestros (que no sean MP4). Adobe Dynamic Media Classic los codifica en archivos MP4 por usted. En el cuadro de diálogo **[!UICONTROL Cargar opciones de trabajo]**, en **[!UICONTROL Opciones de vídeo]**, seleccione **[!UICONTROL Vídeo adaptable]**.

   Esta opción preferida permite crear un conjunto de vídeos adaptables que aplica automáticamente el ajuste preestablecido de codificación correcto al vídeo, 16:9 o 4:3, para que coincida con las dimensiones del vídeo que haya cargado. Al enviar el trabajo de carga, se crea automáticamente un conjunto de vídeos adaptables, que incluye tres ajustes de codificación de vídeo en la proporción de aspecto correcta.

   O bien, en el mismo cuadro de diálogo **[!UICONTROL Opciones de trabajo]**, en **[!UICONTROL Opciones de eVideo]**, expanda **[!UICONTROL Ajustes preestablecidos de codificación única]**. Seleccione los ajustes preestablecidos de codificación de vídeo que desee en **Escritorio**, **Móvil (iPhone, iPad, Android™)** y **Tablet (iPad, Android™)** para crear los archivos MP4.

* O bien, puede volver a procesar un vídeo maestro mediante la función **[!UICONTROL Reprocesar]**. Los vídeos recién codificados se añaden al Conjunto de vídeos adaptable existente.

Consulte [Cargar y codificar vídeos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

Adobe Dynamic Media Classic ofrece numerosos ajustes preestablecidos de codificación de vídeo predefinidos. Estos ajustes predefinidos reflejan los ajustes de codificación de vídeo más comunes utilizados actualmente y están optimizados para la reproducción en páginas de destino.

Sin embargo, si es necesario personalizar más el proyecto, los administradores pueden crear ajustes preestablecidos de vídeo para personalizar el tamaño y la reproducción de vídeos para los usuarios finales. Los administradores pueden agregar y administrar ajustes preestablecidos de vídeo desde la página Ajustes preestablecidos de vídeo disponible en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]** > **[!UICONTROL Ajustes preestablecidos de codificación única]**. La página Ajustes preestablecidos de vídeo contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de vídeo.

Consulte [Trabajo con ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Previsualizar vídeos en un visor de vídeos

Para ver cómo se reproduce un vídeo para los usuarios finales en un escritorio, su sitio web o un dispositivo móvil, seleccione el vídeo en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]**.

Consulte [Vista previa de vídeos en un visor de vídeo](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Puede reproducir el vídeo en la página Vista previa . También puede elegir diferentes visualizadores de vídeo para averiguar cómo aparece el vídeo en diferentes reproductores. La práctica recomendada es utilizar el reproductor de vídeo HTML5 para la reproducción multipantalla en escritorios, tablets y dispositivos móviles.

**Opcional**

Personalización de ajustes preestablecidos de visor : Adobe Dynamic Media Classic ofrece ajustes preestablecidos de visor predefinidos para la entrega de vídeo. Estos ajustes preestablecidos determinan la apariencia del visor y cómo funcionan los controles de reproducción. Para personalizar el visor de vídeo, los administradores pueden agregar y gestionar ajustes preestablecidos de visor desde la página Ajustes preestablecidos de visor. Para abrir esta página, en la esquina superior derecha de Adobe Dynamic Media Classic, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visualizador]**. La página Ajustes preestablecidos de visor contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de visor.

Consulte [Trabajo con ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Consulte también el vídeo de formación [Ajustes preestablecidos de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

## 3. Implemente vídeos en sus sitios web y sitios móviles

Para incorporar el vídeo en el sitio web, puede realizar cualquiera de las acciones siguientes:

* Muestre el vídeo en su propia ventana emergente o modal, en cuyo caso utilice la función **[!UICONTROL Copiar URL]**.

   Para obtener la URL de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Seleccione **[!UICONTROL Preview]** y, a continuación, seleccione **[!UICONTROL Copy URL]** a la derecha de `Universal_HTML5_Viewer`.

   Cuando selecciona **[!UICONTROL Copiar URL]**, la URL se copia en el portapapeles. Coloque este código en el HTML de su sitio web, sitio móvil o aplicación. 

   >[!NOTE]
   >
   >Las direcciones URL solo se activan tras publicar el vídeo o el conjunto de vídeos adaptables.

* Muestre el vídeo incrustado en la página web, en cuyo caso utilice la función **[!UICONTROL Código incrustado]**.

   Para obtener el código incrustado de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Vaya a **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**. En la columna Actions de la tabla, seleccione **[!UICONTROL Embed Code]** a la derecha de `Universal_HTML5_Video`. No se permite editar el código.

   Seleccione **[!UICONTROL Cerrar]** y pegue el código incrustado en las páginas web.

   >[!NOTE]
   >
   >Incrustar código solo se activa después de publicar el vídeo o el conjunto de vídeos adaptables.

Consulte [Implementar vídeo en sitios web y sitios móviles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

