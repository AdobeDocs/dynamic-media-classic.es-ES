---
title: '"Inicio rápido: Vídeo"'
description: Introducción y Inicio rápido a Adobe Dynamic Media Classic Video para ayudarle en el uso inicial.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 65%

---


# Inicio rápido: Vídeo{#quick-start-video}

Adobe Dynamic Media Classic Video es una solución integral que facilita la publicación de vídeo adaptable de alta calidad para transmitir en varias pantallas, incluidos equipos de escritorio, iOS, Android, Blackberry y dispositivos móviles Windows. Los conjuntos de vídeos adaptables agrupan versiones del mismo vídeo codificadas con una velocidad de bits y un formato diferentes, por ejemplo, 400 kbps, 800 kbps y 1.000 kbps. El ordenador de escritorio o dispositivo móvil detecta el ancho de banda disponible.

Por ejemplo, en un dispositivo móvil iOS, detecta un ancho de banda de, por ejemplo, 3G, 4G o Wi-Fi. A continuación, selecciona de forma automática el vídeo codificado correcto de las diversas velocidades de bits que incluye el conjunto de vídeos adaptable. El vídeo se transmite a equipos de escritorio, dispositivos móviles o tablets.

Además, la calidad de vídeo se cambia dinámicamente de forma automática si las condiciones de la red cambian en el equipo de escritorio o en el dispositivo móvil. Además, si un cliente entra en modo de pantalla completa en un equipo de escritorio, el conjunto de vídeos adaptable responde usando una mejor resolución y, por lo tanto, mejorando la experiencia de visualización del cliente. El uso de conjuntos de vídeos adaptables le ofrece la mejor reproducción posible para los clientes que reproducen vídeos de Dynamic Media Classic en varios dispositivos y pantallas.

La lógica que un reproductor de vídeo utiliza para determinar qué vídeo codificado se debe reproducir o seleccionar durante la reproducción se basa en el siguiente algoritmo:

1. El reproductor de vídeo carga el fragmento de vídeo inicial en función de la velocidad de bits más cercana al valor definido para la &quot;velocidad de bits inicial&quot; en el propio reproductor.
1. El reproductor de vídeo cambia en función de los cambios en la velocidad de ancho de banda mediante los siguientes criterios:

   1. El reproductor elige el flujo de ancho de banda más alto por debajo o por debajo del ancho de banda estimado.
   1. El reproductor considera solamente el 80% del ancho de banda disponible. Sin embargo, si se está apagando, es más conversador con sólo el 70% para evitar sobreestimar y tener que volver inmediatamente.

Consulte la lógica del algoritmo en [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obtener información técnica sobre él.

Para administrar un solo vídeo y conjuntos de vídeos adaptables, Dynamic Media Classic admite lo siguiente:

* Carga de vídeos de varios formatos de vídeo y audio compatibles y codificación de vídeo al formato MP4 H.264 para su reproducción en varias pantallas. Puede utilizar los ajustes preestablecidos de vídeo adaptable predefinidos de Dynamic Media Classic, ajustes preestablecidos de codificación de vídeo único o personalizar su propia codificación para controlar la calidad y el tamaño del vídeo.

   Cuando se genera un conjunto de vídeos adaptables, incluye vídeos MP4.

   `**Note:**` Los vídeos principales/originales y cualquier otro vídeo de formato de origen  ** no se admiten en un conjunto de vídeos adaptable.

* Subtítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light y navegación por capítulos de vídeo en los visores Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark y Universal_HTML5_MixedMedia_light.

   Consulte [Adición de subtítulos a vídeos](adding-captions-video.md).

   Consulte [Adición de marcadores de capítulo a vídeos](adding-chapter-markers-video.md).

* Organice, explore o busque vídeos con total compatibilidad de metadatos para gestionar eficazmente sus recursos de vídeo. 
* Publique conjuntos de vídeos adaptables en la web, así como en equipos de escritorio y dispositivos móviles, incluidos iPhone, iPad, Android™, BlackBerry y Windows Phone.

   El flujo de vídeo adaptable se admite en numerosas plataformas de iOS.

   Consulte la compatibilidad más reciente en la [Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/home.html).

   Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP4 H.264. Puede consultar los dispositivos BlackBerry compatibles con este formato de vídeo en este sitio web:

   Consulte [Formatos de vídeo admitidos en Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Puede consultar los dispositivos Windows compatibles con este formato de vídeo:

   Consulte [Formatos de vídeo admitidos en Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Reproducción del vídeo con los ajustes preestablecidos de visor de Dynamic Media Classic, incluidos los siguientes:

   * Visores de vídeos únicos.
   * Visores de medios mixtos que combinan contenido de vídeo y de imagen.

* Configuración de reproductores de vídeo para cumplir las necesidades de marca.
* Integración de vídeo en el sitio web, el sitio móvil o la aplicación móvil con una URL o código incrustado.

**Inicio rápido**

La siguiente descripción paso a paso del flujo de trabajo se ha diseñado para ayudarle en el uso inicial de conjuntos de vídeos adaptables en Dynamic Media Classic. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Carga y codificación de vídeo**

Cargue y genere conjuntos de vídeos adaptables con una de los dos situaciones siguientes:

* **Cargar**
vídeos precodificadosSi los vídeos ya estaban codificados fuera de Dynamic Media Classic, haga clic en 
**** Cargue en la barra de navegación global para buscar y cargar archivos de vídeo MP4 directamente en Dynamic Media Classic. A continuación, haga clic en **Generar > Conjuntos de vídeos adaptables**. Busque los archivos de vídeo. Arrastre los archivos de vídeo deseados, suéltelos en la tabla Conjunto de vídeos adaptable y, a continuación, guarde el conjunto.
* **Cargar**
vídeos de origen maestrosSi los vídeos no están codificados, haga clic en 
**** Cargue en la barra de navegación global para cargar archivos de origen de vídeo maestros (que no sean MP4) y hacer que Dynamic Media Classic los codifique en archivos MP4 por usted. En el cuadro de diálogo Opciones de trabajo de carga, en Opciones de eVideo, seleccione **Vídeo adaptable**.

   Esta opción preferida permite crear un conjunto de vídeos adaptables que aplica automáticamente el ajuste preestablecido de codificación correcto al vídeo, 16:9 o 4:3, para que coincida con las dimensiones del vídeo que haya cargado. Al enviar el trabajo de carga, se crea automáticamente un conjunto de vídeos adaptable que incluye tres codificaciones de vídeo con la proporción de aspecto correcta.

   En el cuadro de diálogo Opc. de trabajo, en Opciones de Evideo, amplíe **Ajustes preestablecidos de codificación única** y seleccione los ajustes preestablecidos de codificación de vídeo individuales que desee de **Escritorio**, **Móvil (iPhone, iPad, Android)** y **Tablet (iPad, Android)** para crear archivos MP4.

* O bien, puede volver a procesar un vídeo maestro mediante la función de reprocesamiento. Los vídeos recién codificados se añaden al Conjunto de vídeos adaptable existente.

Consulte [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

Dynamic Media Classic oferta varios ajustes preestablecidos de codificación de vídeo predefinidos. Estos ajustes preestablecidos reflejan la configuración de codificación de vídeo más común y se han optimizado para la reproducción en las pantallas de destino.

Sin embargo, si es necesario personalizar más el proyecto, los administradores pueden crear ajustes preestablecidos de vídeo para personalizar el tamaño y la reproducción de vídeos para los usuarios finales. Los administradores pueden agregar y administrar ajustes preestablecidos de vídeo desde la página Ajustes preestablecidos de vídeo disponible en Ajustes > Ajustes de aplicación > Ajustes preestablecidos de vídeo > Ajustes preestablecidos de codificación única. La página Ajustes preestablecidos de vídeo contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de vídeo.

Consulte [Uso de ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Previsualización de vídeos en un visor de vídeos**

Para ver cómo se reproduce un vídeo para los usuarios finales en un equipo de escritorio, en el sitio web o en un dispositivo móvil, seleccione el vídeo en el panel Examinar y, a continuación, haga clic en **Vista previa**.

Consulte [Previsualización de vídeos en un visor de vídeos](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Puede reproducir el vídeo en la pantalla Vista previa. También puede elegir visores de vídeos diferentes para ver qué aspecto tiene el vídeo en otros reproductores. La práctica recomendada es utilizar el reproductor de vídeo HTML5 para la reproducción multipantalla en escritorios, tablets y dispositivos móviles.

**Opcional**

Personalización de ajustes preestablecidos de visor: Dynamic Media Classic oferta ajustes preestablecidos de visor predefinidos para la publicación de vídeo. Estos ajustes preestablecidos determinan la apariencia del visor y cómo funcionan los controles de reproducción. Para personalizar el visor de vídeo, los administradores pueden agregar y gestionar ajustes preestablecidos de visor desde la página Ajustes preestablecidos de visor. Para abrir esta página, en la esquina superior derecha de Dynamic Media Classic, haga clic en Ajustes > Ajustes preestablecidos de visor. La página Ajustes preestablecidos de visor contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de visor.

Consulte [Uso de ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Distribución de vídeos en sitios web y sitios móviles**

Para incorporar el vídeo en el sitio web, puede realizar cualquiera de las acciones siguientes:

* Mostrar el vídeo en su propia ventana emergente o modal; en ese caso, se utiliza la función de Copiar URL.

   Para obtener la URL de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Haga clic en Previsualización y, a continuación, en Copiar URL a la derecha de `Universal_HTML5_Viewer`.

   Después de hacer clic en Copiar URL, la dirección URL se copia al portapapeles. Coloque este código en el HTML de su sitio web, sitio móvil o aplicación. 

   >[!NOTE]
   >
   >Las direcciones URL solo se activan tras publicar el vídeo o el conjunto de vídeos adaptables.

* Mostrar el vídeo incrustado en la página web; en ese caso, deberá utilizar la función de Código incrustado.

   Para obtener el código incrustado de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Haga clic en Vista previa > Lista del visor. En la columna Acciones de la tabla, haga clic en Código incrustado a la derecha de `Universal_HTML5_Video`. No se permite editar el código.

   Haga clic en Cerrar y pegue el código incrustado en las páginas web.

   >[!NOTE]
   >
   >Incrustar código solo se activa después de publicar el vídeo o el conjunto de vídeos adaptables.

Consulte [Distribución de vídeo en sitios web y sitios móviles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

