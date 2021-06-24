---
title: Adición de marcadores de capítulo a vídeos
description: Aprenda a añadir marcadores de capítulo a un vídeo.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Visualizadores,Vídeo
role: Business Practitioner
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 217e5bf81cc2108e4bf283f585dfd83d319ff7c9
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 83%

---

# Adición de marcadores de capítulo a vídeos{#adding-chapter-markers-to-video}

Para facilitar la visualización y navegación en vídeos de larga duración, agregue marcadores de capítulo a vídeos individuales o a conjuntos de vídeos adaptables. Cuando un usuario reproduce el vídeo, puede hacer clic en los marcadores de capítulo en la línea de tiempo de vídeo (también conocido como selección manual de vídeo) para navegar con facilidad hasta su punto de interés o para pasar inmediatamente a contenido nuevo, demostraciones, tutoriales, y así sucesivamente.

>[!NOTE]
>
>El reproductor de vídeo que se utilice debe admitir los marcadores de capítulo.

Consulte [Adición y edición de ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) para configurar los puntos de señal de navegación por capítulos y el texto emergente de títulos de capítulos para el visor `Universal_HTML5_Video` (HTML5).

Consulte también [Adición y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

Puede crear una lista de capítulos del vídeo más o menos del mismo modo en que se crean los subtítulos. Es decir, se crea un archivo WebVTT. Tenga en cuenta, no obstante, que este archivo debe ser independiente de cualquier otro archivo WebVTT de subtítulo que utilice; no puede combinar subtítulos y capítulos en un archivo WebVTT.

Puede utilizar la siguiente muestra como ejemplo del formato que se utiliza para crear un archivo WebVTT con navegación por capítulos:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

En el ejemplo anterior, `Chapter 1` es el identificador de referencia y es opcional. El tiempo de referencia de `00:00:000 --> 01:04:364` especifica la hora de inicio y la hora de finalización del capítulo, en formato 00:00:000. Los tres últimos dígitos son milisegundos y pueden dejarse como 000, si se prefiere. El título del capítulo de `The bicycle store behind it all` es la descripción real del contenido del capítulo. El identificador de señal, el tiempo de señal de inicio y el título del capítulo aparecen en una ventana emergente en el reproductor de vídeo cuando un usuario desliza el puntero sobre un punto de señal visual en la línea de tiempo de vídeo.

Como está utilizando un visor de vídeo HTML5, asegúrese de que el archivo de capítulos que cree siga el estándar de WebVTT (Web Video Text Tracks). La extensión de nombre de archivo de capítulos es .vtt. Puede obtener más información sobre el estándar de subtítulos WebVTT.

Consulte [WebVTT: El formato de seguimiento de texto de vídeo web](https://dev.w3.org/html5/webvtt/).

**Para agregar marcadores de capítulo a vídeos**

1. Con un editor de texto simple fuera de Dynamic Media Classic, cree su archivo de capítulo de vídeo.

   >[!NOTE]
   >
   >Para obtener compatibilidad global con capítulos de vídeo en idiomas distintos al inglés, el estándar WebVTT requiere crear llamadas y archivos .vtt independientes para cada idioma.

1. Guarde el archivo .vtt con una codificación UTF8 para evitar problemas de representación de caracteres en el texto del título del capítulo.

   Lo normal es que desee nombrar al archivo de capítulos VTT con el mismo nombre que el archivo de vídeo y le añada la palabra `chapters`. Esto puede ayudarle a automatizar la generación de URL de vídeo mediante el sistema de administración de contenido web.

1. En Dynamic Media Classic, cargue el archivo de capítulo WebVTT.

   Consulte [Carga de archivos](uploading-files.md#uploading_files).

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el archivo de vídeo que desee asociar al archivo de capítulos que haya cargado.
1. En el panel de exploración de recursos, seleccione un único recurso de vídeo y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** debajo de la imagen en miniatura del recurso.
1. En la tabla Lista de visores, busque el visor HTML5 con el nombre **Universal_HTML5_Video** y, a continuación, realice una de las siguientes acciones:

   * Para obtener un visor de vídeo emergente, haga clic en **[!UICONTROL Copiar URL]** a la derecha del nombre.

      Añada la URL copiada del vídeo con la siguiente sintaxis para asociarla con la URL copiada en el archivo de subtítulos:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para obtener un visor de vídeo incorporado, haga clic en **[!UICONTROL Código Incrustado]** a la derecha del nombre.

      En el cuadro de diálogo Código incrustado, haga clic en **[!UICONTROL Copiar al portapapeles]**.

      Para el visor HTML5 `Universal_HTML5_Video`, añada el código incrustado copiado con lo siguiente:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
