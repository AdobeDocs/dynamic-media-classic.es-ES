---
title: Agregar subtítulos a vídeo
description: Aprenda a añadir subtítulos a los vídeos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: a607488b6a1dd51ef7cc8c885db5a87f4f792aaa
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 27%

---

# Agregar subtítulos a vídeo {#add-captions-to-video}

Para ampliar el alcance de los vídeos a mercados globales, agregue subtítulos a vídeos únicos o a conjuntos de vídeos adaptables. Con los rótulos, evita tener que doblar el audio o la necesidad de utilizar hablantes nativos para volver a grabar el audio en idiomas diferentes. El vídeo se reproduce en el idioma en el que se ha grabado. Los subtítulos en lengua extranjera aparecen para que las personas de distintos idiomas puedan entender la parte de audio.

Los subtítulos también permiten una mayor accesibilidad gracias al uso de rótulos cerrados para personas con discapacidad auditiva.

>[!NOTE]
>
>El reproductor de vídeo que se utiliza debe admitir la visualización de rótulos.

Para configurar el efecto de rótulo y editar el propio menú de rótulo, incluido el texto del menú para cualquiera de los siguientes visores:

* `Universal_HTML5_Video` visualizador
* `Universal_HTML5_MixedMedia_dark` visualizador
* `Universal_HTML5_MixedMedia_light` visualizador

Consulte [Añadir o editar un ajuste preestablecido de visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte también [Agregar y editar ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic puede convertir archivos de rótulo al formato JSON (JavaScript Object Notation). Esta conversión significa que puede incrustar el texto de JSON en una página web como una transcripción completa pero oculta del vídeo. Los motores de búsqueda pueden rastrear e indexar el contenido para que los vídeos sean más fáciles de descubrir y dar a los clientes más detalles sobre el contenido del vídeo.

Consulte [Proporcionar contenido estático (que no sea de imagen)](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) en el *Ayuda de API de servicio de imágenes de Adobe* para obtener más información sobre el uso de la función JSON en una dirección URL.

**Para agregar subtítulos al vídeo:**

1. Con una aplicación de terceros fuera de Adobe Dynamic Media Classic, cree el archivo de rótulo de vídeo en función del tipo de visor que esté utilizando.

   | Tipo de visor | Archivo de subtítulos |
   |--- |--- |
   | HTML5 | Si utiliza un visor de vídeo HTML5, asegúrese de que el archivo de subtítulos que cree sigue el estándar de WebVTT (Web Video Text Tracks). La extensión de nombre de archivo de subtítulos es .vtt. Puede obtener más información sobre el estándar de subtítulos WebVTT.<br><br>[Consulte WebVTT](https://w3c.github.io/webvtt/): el formato de seguimiento de texto de vídeo web. <br><br>Hay muchos sitios web que ofrecen herramientas y servicios gratuitos y basados en tarifas que puede utilizar para crear archivos de subtítulos WebVTT fuera de Adobe Dynamic Media Classic. <br><br>Siga las instrucciones en pantalla de un sitio para crear y guardar el archivo WebVTT. Cuando haya terminado, copie el contenido del archivo de rótulo y péguelo en un editor de texto sin formato y guárdelo con la extensión de nombre de archivo VTT. <br><br><b>Nota:</b> Para que los subtítulos de vídeo sean compatibles de forma global en idiomas distintos del inglés, el estándar WebVTT requiere que cree archivos .vtt independientes y que realice llamadas a cada idioma que desee admitir. <br><br>Por lo general, desea asignar al archivo VTT de rótulo el mismo nombre que al archivo de vídeo y anexarlo con rótulos. Esto puede ayudarle a automatizar la generación de URL de vídeo mediante el sistema de administración de contenido web. |

1. En Adobe Dynamic Media Classic, cargue el archivo de subtítulos XML WebVTT, DFXP o SMPTE.

   Consulte [Cargar archivos](uploading-files.md#uploading_files).

1. En el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el archivo de vídeo que se asociará al archivo de rótulo que ha cargado.
1. En el panel Examinar recursos, seleccione un único recurso de vídeo y, debajo de la imagen en miniatura del recurso, seleccione **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.
1. En la tabla Lista de visualizadores, busque el visualizador HTML 5 denominado **Universal_HTML 5_Video**, **Universal_HTML 5_MixedMedia_oscuro**, o **Universal_HTML 5_MixedMedia_light**, a continuación, realice una de las siguientes acciones:

   * Para una experiencia de visor de vídeo emergente, seleccione **[!UICONTROL Copiar URL]** situado en el extremo derecho del nombre.

     Anexe la URL copiada del vídeo con la siguiente sintaxis para que pueda asociarla con la URL copiada al archivo de rótulo:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Tenga en cuenta `,1` al final de la ruta de URL del pie de ilustración. Inmediatamente después de la extensión de nombre de archivo VTT en la ruta, puede, opcionalmente, habilitar o deshabilitar el botón de subtítulos opcionales en la barra del reproductor de vídeo estableciendo en `1` o `0`, respectivamente.

   * Para una experiencia de visor de vídeo integrada, seleccione **[!UICONTROL Código incrustado]** situado en el extremo derecho del nombre.

     En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al portapapeles]**.

     Para el HTML 5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, o `Universal_HTML5_MixedMedia_light` Para los visualizadores de, añada el código incrustado copiado con lo siguiente:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Tenga en cuenta `,1` al final de la ruta URL. Inmediatamente después de la extensión de nombre de archivo VTT en la ruta URL, puede, opcionalmente, habilitar o deshabilitar el botón de rótulo en la barra del reproductor de vídeo estableciendo en `1` o `0`, respectivamente.
