---
title: Añadir marcadores de capítulo al vídeo
description: Aprenda a añadir marcadores de capítulo a un vídeo en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# Añadir marcadores de capítulo al vídeo {#adding-chapter-markers-to-video}

Puede facilitar la visualización y navegación de los vídeos de formato largo añadiendo marcadores de capítulo a vídeos únicos o a conjuntos de vídeos adaptables. Cuando un usuario reproduce el vídeo, puede seleccionar los marcadores de capítulo en la cronología del vídeo (también conocida como selección manual de vídeo). Al hacerlo, pueden desplazarse fácilmente a su punto de interés o ir inmediatamente a nuevo contenido, demostraciones, tutoriales, etc.

>[!NOTE]
>
>El reproductor de vídeo que se utilice debe admitir los marcadores de capítulo.

Consulte [Agregar o editar un ajuste preestablecido de visor de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) si desea configurar los puntos de referencia de navegación por capítulos y el texto emergente del título del capítulo para el visor `Universal_HTML5_Video` (HTML5).

Consulte también [Agregar y editar ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets).

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

En el ejemplo anterior, `Chapter 1` es el identificador de referencia y es opcional. La hora de referencia de `00:00:000 --> 01:04:364` especifica la hora de inicio y finalización del capítulo, en formato 00:00:000. Los tres últimos dígitos son milisegundos y pueden dejarse como 000, si se prefiere. El título de capítulo de `The bicycle store behind it all` es la descripción real del contenido del capítulo. El identificador de referencia, el tiempo de referencia inicial y el título del capítulo aparecen en una ventana emergente del reproductor de vídeo cuando se pasa el puntero sobre un punto de referencia visual en la cronología del vídeo.

Como está utilizando un visor de vídeo HTML5, asegúrese de que el archivo de capítulos que cree siga el estándar de WebVTT (Web Video Text Tracks). La extensión del nombre de archivo del capítulo es `.VTT`. Puede obtener más información sobre el estándar de subtítulos WebVTT.

Ver [WebVTT: el formato de seguimiento de texto de vídeo web](https://w3c.github.io/webvtt/).

**Para agregar marcadores de capítulo a un vídeo:**

1. Cree su archivo de capítulo de vídeo con un editor de texto simple fuera de Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >Para ofrecer compatibilidad global con capítulos de vídeo en idiomas distintos del inglés, el estándar WebVTT requiere que cree `.VTT` archivos y llamadas independientes para cada idioma que desee admitir.

1. Guarde el archivo VTT con codificación UTF8 para evitar problemas con la representación de caracteres en el texto del título del capítulo.

   Por lo general, desea asignar al archivo VTT del capítulo el mismo nombre que al archivo de vídeo y anexarlo con `chapters`. Al hacerlo, puede ayudarle con la automatización de la generación de las direcciones URL de vídeo mediante el sistema de administración de contenido web existente.

1. En Adobe Dynamic Media Classic, cargue el archivo de capítulo WebVTT.

   Ver [Cargar archivos](uploading-files.md#uploading_files).

1. En el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el archivo de vídeo que se asociará al archivo de capítulo que ha cargado.
1. En el panel Examinar recursos, seleccione un solo recurso de vídeo y, debajo de la imagen en miniatura del recurso, seleccione **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.
1. En la tabla Lista de visores, busque el visor HTML5 con el nombre **Universal_HTML5_Video** y, a continuación, realice una de las siguientes acciones:

   * Para obtener una experiencia de visor de vídeo emergente, seleccione **[!UICONTROL Copiar URL]** en el extremo derecho del nombre.

     Anexe la URL copiada del vídeo con la siguiente sintaxis para que pueda asociarla con la URL copiada al archivo de rótulo:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Para disfrutar de una experiencia de visor de vídeo integrada, seleccione **[!UICONTROL Código incrustado]** en el extremo derecho del nombre.

     En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al Portapapeles]**.

     Para el visor de HTML5 `Universal_HTML5_Video`, anexe el código incrustado copiado con lo siguiente:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
