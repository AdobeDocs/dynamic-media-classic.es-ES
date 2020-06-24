---
title: Adición de subtítulos a vídeos
seo-title: Adición de subtítulos a vídeos
description: nulo
seo-description: Aprenda a añadir subtítulos al vídeo
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
translation-type: tm+mt
source-git-commit: 74238f90f45f0fb9a4566915a20a1d41dfb69fe1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 70%

---


# Adición de subtítulos a vídeos{#adding-captions-to-video}

Para ampliar el alcance de los vídeos a mercados globales, agregue subtítulos a vídeos únicos o a conjuntos de vídeos adaptables. Con los rótulos, evita tener que doblar el audio o la necesidad de utilizar hablantes nativos para volver a grabar el audio en idiomas diferentes. El vídeo se reproduce en el idioma en el que se ha grabado. Los subtítulos en lengua extranjera aparecen para que las personas de distintos idiomas puedan entender la parte de audio.

Los subtítulos también permiten una mayor accesibilidad gracias al uso de rótulos cerrados para personas con discapacidad auditiva.

>[!NOTE]
>
>El reproductor de vídeo que se utiliza debe admitir la visualización de rótulos.

Consulte [Adición y edición de ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) para configurar el efecto de subtítulo y editar el propio menú de subtítulo, incluido el texto del menú para cualquiera de los visores siguientes:

* `Universal_HTML5_Video` visor.
* `Universal_HTML5_MixedMedia_dark` visor.
* `Universal_HTML5_MixedMedia_light` visor.

Consulte también [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic tiene la capacidad de convertir archivos de subtítulos al formato JSON (JavaScript Object Notation). Esta conversión significa que puede incrustar el texto de JSON en una página web como una transcripción completa pero oculta del vídeo. Los motores de búsqueda pueden buscar e indexar el contenido para que los vídeos se detecten más fácilmente y para proporcionar a los clientes detalles adicionales sobre el contenido de vídeo.

See [Serving static (non-image) contents](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**Para agregar subtítulos a vídeos**

1. Con una aplicación de terceros fuera de Scene7 Publishing System, cree un archivo de subtítulos de vídeo según el tipo de visor que utilice.

   | Tipo de visor | Archivo de subtítulos |
   |--- |--- |
   | HTML5 | Si utiliza un visor de vídeo HTML5, asegúrese de que el archivo de subtítulos que cree sigue el estándar de WebVTT (Web Video Text Tracks). La extensión de nombre de archivo de subtítulos es .vtt. Puede obtener más información sobre el estándar de subtítulos WebVTT.<br><br>[Consulte WebVTT](https://dev.w3.org/html5/webvtt/): Formato de seguimiento de texto de vídeo web. <br><br>Hay herramientas y servicios gratuitos y de pago que puede utilizar para crear archivos de subtítulos fuera de Scene7 Publishing System. Por ejemplo, para crear un archivo de subtítulos de vídeo sencillo sin estilo, puede utilizar la siguiente herramienta gratuita de edición y creación de subtítulos en línea: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Para obtener los mejores resultados, utilice la herramienta de Internet Explorer 9 o posterior, Google Chrome o Safari. <br><br>En la herramienta, pegue la URL del archivo de vídeo en el campo <b>Escribir dirección URL del archivo de vídeo</b> y haga clic en <b>Cargar</b>. <br><br>Por ejemplo, si está utilizando una URL de Dynamic Media Classic para el archivo de vídeo, en SPS, haga clic con el doble en un recurso de vídeo individual (no en un conjunto de vídeos adaptable ni en un vídeo principal) para abrirlo en la Vista de detalles. En el panel derecho de la vista de detalles, amplíe URL y código incrustado. A continuación, en el grupo Móvil, a la derecha de Móvil (progresivo), haga clic en Copiar URL. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. Internet Explorer, Chrome o Safari pueden reproducir el vídeo de forma predeterminada. Siga las instrucciones en pantalla del sitio para crear y guardar el archivo WebVTT. Cuando haya terminado, copie el contenido del archivo de subtítulos, péguelo en un editor de texto sin formato y guárdelo con una extensión de nombre de archivo .vtt. <br><br><b>Nota:</b> Para obtener compatibilidad global con subtítulos de vídeo en idiomas distintos del inglés, el estándar WebVTT requiere que cree llamadas y archivos .vtt independientes para cada idioma que desee admitir. <br><br>Lo normal es que desee nombrar al archivo de subtítulos VTT con el mismo nombre que el archivo de vídeo y le añada la palabra captions. Esto puede ayudarle a automatizar la generación de URL de vídeo mediante el sistema de administración de contenido web. |

1. En Scene7 Publishing System, cargue el archivo WebVTT, DFXP o SMPTE XML.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el archivo de vídeo que desee asociar al archivo de subtítulos que ha cargado.
1. En el panel de exploración de recursos, seleccione un único recurso de vídeo y, a continuación, haga clic en **Vista previa** > **Lista del visor** debajo de la imagen en miniatura del recurso.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * Para obtener un visor de vídeo emergente, haga clic en **Copiar URL** a la derecha del nombre.

      Añada la URL copiada del vídeo con la siguiente sintaxis para asociarla con la URL copiada en el archivo de subtítulos:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. Inmediatamente después de la extensión de nombre de archivo .vtt en la ruta, tiene la opción de activar o desactivar el botón de subtítulos opcionales en la barra del reproductor de vídeo si lo define en `1` o `0` respectivamente.

   * Para obtener un visor de vídeo incorporado, haga clic en **Código Incrustado** a la derecha del nombre.

      En el cuadro de diálogo Código incrustado, haga clic en **Copiar al portapapeles**.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. Inmediatamente después de la extensión de nombre de archivo .vtt en la ruta de URL, tiene la opción de activar o desactivar el botón de subtítulos opcionales en la barra del reproductor de vídeo si lo define en `1` o `0` respectivamente.

