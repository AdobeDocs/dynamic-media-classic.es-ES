---
title: 'Agregar subtítulos a vídeo '
description: Aprenda a añadir subtítulos a vídeo en Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# Agregar subtítulos a vídeo {#adding-captions-to-video}

Para ampliar el alcance de los vídeos a mercados globales, agregue subtítulos a vídeos únicos o a conjuntos de vídeos adaptables. Con los rótulos, evita tener que doblar el audio o la necesidad de utilizar hablantes nativos para volver a grabar el audio en idiomas diferentes. El vídeo se reproduce en el idioma en el que se ha grabado. Los subtítulos en lengua extranjera aparecen para que las personas de distintos idiomas puedan entender la parte de audio.

Los subtítulos también permiten una mayor accesibilidad gracias al uso de rótulos cerrados para personas con discapacidad auditiva.

>[!NOTE]
>
>El reproductor de vídeo que se utiliza debe admitir la visualización de rótulos.

Para configurar el efecto Rótulo y editar el propio menú Rótulo, incluido el texto del menú para cualquiera de los siguientes visores:

* `Universal_HTML5_Video` visor
* `Universal_HTML5_MixedMedia_dark` visor
* `Universal_HTML5_MixedMedia_light` visor

Consulte [Añadir o editar un ajuste preestablecido de visor de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte también [Agregar y editar ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic puede convertir archivos de rótulos al formato JSON (JavaScript Object Notation). Esta conversión significa que puede incrustar el texto de JSON en una página web como una transcripción completa pero oculta del vídeo. Los motores de búsqueda pueden rastrear e indexar el contenido para que los vídeos se puedan descubrir más fácilmente y dar a los clientes más detalles sobre el contenido del vídeo.

Consulte [Proporcionar contenido estático (no de imagen)](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) en la *Ayuda de la API del servicio de imágenes de Adobe* para obtener más información sobre el uso de la función JSON en una URL.

**Para agregar subtítulos a vídeos:**

1. Con una aplicación de terceros fuera de Adobe Dynamic Media Classic, cree su archivo de subtítulos de vídeo en función del tipo de visor que esté utilizando.

   | Tipo de visor | Archivo de subtítulos |
   |--- |--- |
   | HTML5 | Si utiliza un visor de vídeo HTML5, asegúrese de que el archivo de subtítulos que cree sigue el estándar de WebVTT (Web Video Text Tracks). La extensión de nombre de archivo de subtítulos es .vtt. Puede obtener más información sobre el estándar de subtítulos WebVTT.<br><br>[Consulte WebVTT](https://w3c.github.io/webvtt/): Formato de seguimiento de texto de vídeo web. <br><br>Existen herramientas y servicios gratuitos y de pago que puede utilizar para crear archivos de subtítulos fuera de Adobe Dynamic Media Classic. Por ejemplo, para crear un archivo de subtítulos de vídeo sencillo sin estilo, puede utilizar la siguiente herramienta gratuita de edición y creación de subtítulos en línea: <br><br>[Creador de subtítulos WebVTT](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Para obtener mejores resultados, utilice la herramienta en Internet Explorer 9 o superior, Google Chrome o Safari. <br><br>En la herramienta , en el campo  <b>Introducir URL del </b> archivo de vídeo , pegue la URL del archivo de vídeo y, a continuación, seleccione  <b>Cargar</b>. <br><br>Por ejemplo, si utiliza una URL de Dynamic Media Classic de Adobe para el archivo de vídeo, haga doble clic en un recurso de vídeo individual (no en un conjunto de vídeos adaptables ni en un vídeo maestro) para abrirlo en la Vista de detalles. En el panel derecho de la vista de detalles, amplíe URL y código incrustado. A continuación, en el grupo Móvil, a la derecha de Móvil (progresivo), seleccione <b>Copiar URL</b>. Este proceso le da la dirección URL del propio archivo de vídeo, que puede pegar en el campo <b>Enter URL of video file</b>. Internet Explorer, Chrome o Safari pueden reproducir el vídeo de forma predeterminada. Siga las instrucciones en pantalla del sitio para crear y guardar el archivo WebVTT. Cuando haya terminado, copie el contenido del archivo de rótulo y péguelo en un editor de texto sin formato y guárdelo con una extensión de nombre de archivo VTT. <br><br><b>Nota:</b> Para que los subtítulos de vídeo sean compatibles con todo el mundo en idiomas distintos del inglés, el estándar WebVTT requiere que cree archivos .vtt y llamadas independientes para cada idioma que desee admitir. <br><br>Lo normal es que desee nombrar al archivo de subtítulos VTT con el mismo nombre que el archivo de vídeo y le añada la palabra captions. Esto puede ayudarle a automatizar la generación de URL de vídeo mediante el sistema de administración de contenido web. |

1. En Adobe Dynamic Media Classic, cargue su archivo de subtítulos WebVTT, DFXP o SMPTE XML.

   Consulte [Cargar archivos](uploading-files.md#uploading_files).

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el archivo de vídeo que desee asociar al archivo de subtítulos que ha cargado.
1. En el panel Examinar recursos, seleccione un único recurso de vídeo y, a continuación, debajo de la imagen en miniatura del recurso, seleccione **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.
1. En la tabla Lista de visores, busque el visor HTML5 denominado **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** o **Universal_HTML5_MixedMedia_light** y, a continuación, realice una de las siguientes acciones:

   * Para una experiencia con el visor de vídeo emergente, seleccione **[!UICONTROL Copiar URL]** en el extremo derecho del nombre.

      Añada la URL copiada del vídeo con la siguiente sintaxis para poder asociarla con la URL copiada al archivo de rótulo:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Observe el `,1` al final de la ruta URL del rótulo. Inmediatamente después de la extensión de nombre de archivo VTT en la ruta, puede activar o desactivar el botón de subtítulos en la barra del reproductor de vídeo configurando en `1` o `0`, respectivamente.

   * Para una experiencia con el visor de vídeo incrustado, seleccione **[!UICONTROL Código incrustado]** a la derecha del nombre.

      En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al portapapeles]**.

      Para los visores HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` o `Universal_HTML5_MixedMedia_light`, añada el código incrustado copiado con lo siguiente:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Observe el `,1` al final de la ruta de URL. Inmediatamente después de la extensión de nombre de archivo VTT en la ruta URL, puede activar o desactivar el botón de rótulo en la barra del reproductor de vídeo estableciendo en `1` o `0`, respectivamente.
