---
title: '"Inicio rápido: Vídeo"'
seo-title: '"Inicio rápido: Vídeo"'
description: nulo
seo-description: Introducción e Inicio rápido a vídeo para ayudarle a empezar a utilizarlo rápidamente.
uuid: bf 0 ecf 87-a 1 f 2-4 e 83-8041-df 5192 dd 26 a 1
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/video
discoiquuid: 6 cef 541 b-e 9 df -48 eb -9 a 16-ca 3 e 1 f 07238 e
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Inicio rápido: Vídeo{#quick-start-video}

Adobe Dynamic Media Classic Video es una solución integral que facilita la publicación de vídeos adaptables de alta calidad para transmitir en varias pantallas, incluido el escritorio, iOS, Android, Blackberry y Windows Phone. Los conjuntos de vídeos adaptables agrupan versiones del mismo vídeo codificadas con una velocidad de bits y un formato diferentes, por ejemplo, 400 kbps, 800 kbps y 1.000 kbps. El ordenador de escritorio o dispositivo móvil detecta el ancho de banda disponible.

Por ejemplo, en un dispositivo móvil iOS, detecta un ancho de banda de, por ejemplo, 3G, 4G o Wi-Fi. A continuación, selecciona de forma automática el vídeo codificado correcto de las diversas velocidades de bits que incluye el conjunto de vídeos adaptable. El vídeo se transmite a equipos de escritorio, dispositivos móviles o tablets.

Además, la calidad de vídeo se cambia dinámicamente de forma automática si las condiciones de la red cambian en el equipo de escritorio o en el dispositivo móvil. Además, si un cliente entra en modo de pantalla completa en un equipo de escritorio, el conjunto de vídeos adaptable responde usando una mejor resolución y, por lo tanto, mejorando la experiencia de visualización del cliente. El uso de conjuntos de vídeos adaptables proporciona la mejor reproducción posible para los clientes que reproducen vídeo de Dynamic Media Classic en varias pantallas y dispositivos.

La lógica que un reproductor de vídeo utiliza para determinar qué vídeo codificado se debe reproducir o seleccionar durante la reproducción se basa en el siguiente algoritmo:

1. El reproductor de vídeo carga el fragmento de vídeo inicial en función de la velocidad de bits más cercana al valor establecido para la «velocidad de bits inicial» en el propio reproductor.
1. El reproductor de vídeo cambia según los cambios en la velocidad de ancho de banda mediante los siguientes criterios:

   1. Player elige el flujo de ancho de banda más alto inferior o igual al ancho de banda estimado.
   1. Player solo considera el 80% del ancho de banda disponible. Sin embargo, si está cambiando, es más invervativo a solo un 70% para evitar la sobreestimación y tener que volver inmediatamente.

Consulte la lógica del algoritmo en [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) para obtener información técnica sobre él.

Para gestionar un solo vídeo y conjuntos de vídeos adaptables, Dynamic Media Classic admite lo siguiente:

* Carga de vídeos de varios formatos de vídeo y audio compatibles y codificación de vídeo al formato MP4 H.264 para su reproducción en varias pantallas. Puede utilizar ajustes preestablecidos de vídeo adaptables Classic Media Classic predefinidos, ajustes preestablecidos de codificación de vídeo único o personalizar su propia codificación para controlar la calidad y el tamaño del vídeo.

   Cuando se genera un conjunto de vídeos adaptables, incluye vídeos MP 4.

   `**Note:**` Los vídeos principales/originales y cualquier otro vídeo de formato de origen *no* se agregan a un conjunto de vídeos adaptable.

* Subtitulación de vídeo en los visores Universal_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ dark y Universal_ HTML 5_ mixedmedia_ light y navegación por capítulos de vídeo en los visores Universal_ HTML 5_ Video, Universal_ HTML 5_ mixedmedia_ dark y Universal_ HTML 5_ mixedmedia_ light.

   Consulte [Adición de subtítulos a vídeos](adding-captions-video.md).

   Consulte [Adición de marcadores de capítulo a vídeos](adding-chapter-markers-video.md).

* Organice, explore o busque vídeos con total compatibilidad de metadatos para gestionar eficazmente sus recursos de vídeo. 
* Publique conjuntos de vídeos adaptables en la web, así como en equipos de escritorio y dispositivos móviles, incluidos iPhone, iPad, Android™, BlackBerry y Windows Phone.

   El flujo de vídeo adaptable se admite en numerosas plataformas de iOS.

   Consulte la compatibilidad más reciente en la Guía de referencia de visores [de Adobe](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

   Dynamic Media Classic admite la reproducción de vídeo móvil para vídeo MP 4 H .264. Puede consultar los dispositivos BlackBerry compatibles con este formato de vídeo en este sitio web:

   Consulte [Formatos de vídeo compatibles con Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Puede consultar los dispositivos Windows compatibles con este formato de vídeo:

   Consulte [Formatos de vídeo compatibles en Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Reproducir el vídeo utilizando los ajustes preestablecidos de visor de Dynamic Media Classic, incluidos los siguientes:

   * Visores de vídeos únicos.
   * Visores de medios mixtos que combinan contenido de vídeo y de imagen.

* Configuración de reproductores de vídeo para cumplir las necesidades de marca.
* Integración de vídeo en el sitio web, el sitio móvil o la aplicación móvil con una URL o código incrustado.

**Inicio rápido**

La descripción de flujo de trabajo paso a paso siguiente está diseñada para ayudarle en el uso inicial de conjuntos de vídeos adaptables en Dynamic Media Classic. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Carga y codificación de vídeo**

Cargue y genere conjuntos de vídeos adaptables con una de los dos situaciones siguientes:

* **Cargar vídeos** precodificados: si sus vídeos ya se han codificado fuera de Dynamic Media Classic, haga clic **en Cargar** en la barra de navegación global para buscar y cargar archivos de vídeo MP 4 directamente en Scene 7 Publishing System. A continuación, haga clic en **Generar** &gt; **Conjuntos de vídeos adaptables**. Busque los archivos de vídeo. Arrastre los archivos de vídeo deseados, suéltelos en la tabla Conjunto de vídeos adaptable y, a continuación, guarde el conjunto.
* **Cargar vídeos** de origen maestros: si los vídeos no están codificados, haga clic **en Cargar** en la barra de navegación global para cargar archivos principales de origen de vídeo (que no sean MP 4) y que Scene 7 Publishing System los codifique en archivos MP 4. En el cuadro de diálogo Opciones de trabajo de carga, en Opciones de eVideo, seleccione **Vídeo adaptable**.

   Esta opción preferida permite crear un conjunto de vídeos adaptables que aplica automáticamente el ajuste preestablecido de codificación correcto al vídeo, 16:9 o 4:3, para que coincida con las dimensiones del vídeo que haya cargado. Al enviar el trabajo de carga, se crea automáticamente un conjunto de vídeos adaptable que incluye tres codificaciones de vídeo con la proporción de aspecto correcta.

   En el cuadro de diálogo Opc. de trabajo, en Opciones de Evideo, amplíe **Ajustes preestablecidos de codificación única** y seleccione los ajustes preestablecidos de codificación de vídeo individuales que desee de **Escritorio**, **Móvil (iPhone, iPad, Android)** y **Tablet (iPad, Android)** para crear archivos MP4.

* O bien, puede volver a procesar un vídeo maestro mediante la función de reprocesamiento. Los vídeos recién codificados se añaden al Conjunto de vídeos adaptable existente.

Consulte [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Opcional**

Dynamic Media Classic ofrece numerosos ajustes preestablecidos de codificación de vídeo predefinidos. Estos ajustes preestablecidos reflejan la configuración de codificación de vídeo más común y se han optimizado para la reproducción en las pantallas de destino.

Sin embargo, si es necesario personalizar más el proyecto, los administradores pueden crear ajustes preestablecidos de vídeo para personalizar el tamaño y la reproducción de vídeos para los usuarios finales. Los administradores pueden agregar y administrar ajustes preestablecidos de vídeo desde la página Ajustes preestablecidos de vídeo disponible en Ajustes &gt; Ajustes de aplicación &gt; Ajustes preestablecidos de vídeo &gt; Ajustes preestablecidos de codificación única. La página Ajustes preestablecidos de vídeo contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de vídeo.

Consulte [Uso de ajustes preestablecidos de codificación de vídeo](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Previsualización de vídeos en un visor de vídeos**

Para ver cómo se reproduce un vídeo para los usuarios finales en un equipo de escritorio, en el sitio web o en un dispositivo móvil, seleccione el vídeo en el panel Examinar y, a continuación, haga clic en **Vista previa**.

Consulte [Previsualización de vídeos en un visor de vídeos](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Puede reproducir el vídeo en la pantalla Vista previa. También puede elegir visores de vídeos diferentes para ver qué aspecto tiene el vídeo en otros reproductores. La práctica recomendada es utilizar el reproductor de vídeo HTML5 para la reproducción multipantalla en escritorios, tablets y dispositivos móviles.

**Opcional**

Personalización de ajustes preestablecidos de visor: Dynamic Media Classic ofrece ajustes preestablecidos de visor predefinidos para la publicación de vídeo. Estos ajustes preestablecidos determinan la apariencia del visor y cómo funcionan los controles de reproducción. Para personalizar el visor de vídeo, los administradores pueden agregar y gestionar ajustes preestablecidos de visor desde la página Ajustes preestablecidos de visor. Para abrir esta página, en la esquina superior derecha de Scene7 Publishing System, haga clic en Ajustes &gt; Ajustes preestablecidos de visor. La página Ajustes preestablecidos de visor contiene opciones para agregar, editar, eliminar y activar ajustes preestablecidos de visor.

Consulte [Uso de ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Distribución de vídeos en sitios web y sitios móviles**

Para incorporar el vídeo en el sitio web, puede realizar cualquiera de las acciones siguientes:

* Mostrar el vídeo en su propia ventana emergente o modal; en ese caso, se utiliza la función de Copiar URL.

   Para obtener la URL de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Click Preview, and then click Copy URL to the right of `Universal_HTML5_Viewer`.

   Después de hacer clic en Copiar URL, la dirección URL se copia al portapapeles. Coloque este código en el HTML de su sitio web, sitio móvil o aplicación. 

   ***nota**: Las URL solo se activan después de publicar el vídeo o el conjunto de vídeos adaptables.*

* Mostrar el vídeo incrustado en la página web; en ese caso, deberá utilizar la función de Código incrustado.

   Para obtener el código incrustado de un vídeo, en la vista de cuadrícula o de lista, selecciónelo en el panel Examinar. Haga clic en Vista previa &gt; Lista del visor. En la columna Acciones de la tabla, haga clic en Código incrustado a la derecha de `Universal_HTML5_Video`. No se permite editar el código.

   Haga clic en Cerrar y pegue el código incrustado en las páginas web.

   ***nota**: El código incrustado solo se activa después de publicar el vídeo o el conjunto de vídeos adaptables.*

Consulte [Distribución de vídeo en sitios web y sitios móviles](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best_practices_for_video_encoding)

