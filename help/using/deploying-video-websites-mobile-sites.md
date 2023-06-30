---
title: Distribución de vídeo en los sitios web y sitios móviles
description: Obtenga información sobre cómo implementar vídeo en sus sitios web y sitios móviles desde Adobe Dynamic Media Classic.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 34%

---

# Distribución de vídeo en los sitios web y sitios móviles{#deploying-video-to-your-websites-and-mobile-sites}

Los sitios web, los sitios móviles y las aplicaciones de escritorio acceden al contenido del servidor de Adobe Dynamic Media Classic, incluido el vídeo, mediante cadenas URL o código incrustado. Adobe Dynamic Media Classic activa estas cadenas URL durante el proceso de publicación. Para colocar la cadena URL o el código incrustado del vídeo en las páginas web, páginas móviles y aplicaciones de escritorio, cópielo desde Adobe Dynamic Media Classic.

>[!NOTE]
>
>La URL o el código incrustado no se activan hasta que publique el recurso.

## Publicación de vídeo {#publishing-video}

La publicación de un vídeo permite a los servidores de Adobe Dynamic Media Classic enviar vídeos a su sitio web, sitio móvil o aplicación.

Existen dos métodos diferentes que puede utilizar para publicar vídeos:

* **Publicación automática e instantánea de vídeos al cargar** : Como parte del proceso de carga de vídeos, Adobe Dynamic Media Classic puede publicar vídeos automáticamente cuando se cargan y codifican. Esta capacidad para publicar inmediatamente significa que no es necesario publicar los vídeos por separado posteriormente.

* **Publicación manual de vídeos tras la carga** - Si no desea publicar vídeos inmediatamente, puede publicar los vídeos manualmente en cualquier momento.

Después de publicar los vídeos, Adobe Dynamic Media Classic activa las cadenas URL de la página del HTML o del código de la aplicación.

**Para publicar vídeos:**

1. Realice una de las siguientes acciones:

   * Para publicar vídeos de forma automática e instantánea al cargar, en la página Cargar, seleccione **[!UICONTROL Publicar tras la carga]**. Ya ha terminado; no tiene que seguir más pasos.
   * Para publicar vídeos manualmente después de la carga, en el panel Examinar, seleccione los vídeos y, a continuación, en la barra de navegación global, seleccione **Publish**.

## Vinculación de una URL de vídeo a un sitio móvil o sitio web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Una vez que haya publicado un vídeo, puede obtener su URL para utilizarla en un sitio web, un sitio de dispositivos móviles o una aplicación de escritorio. Utilice las URL de vídeo cuando desee mostrar vídeo en una ventana emergente o modal por encima de la página web.

Cuando un cliente selecciona el vínculo, se detectan automáticamente su dispositivo, ancho de banda y tamaño de pantalla. Se mostrará el vídeo apropiado para la reproducción en el visor predefinido para el ordenador o en el reproductor de vídeo nativo del dispositivo smartphone o tablet.

Consulte también [Incrustar el visor de vídeo en una página web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Para vincular una URL de vídeo a sitios web o de dispositivos móviles:**

1. En el panel Examen de recursos, en la variable **[!UICONTROL Mostrar]** , seleccione la opción **[!UICONTROL Vídeo]** o **[!UICONTROL Conjunto de vídeos adaptable]**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptables cuyo código incrustado desee vincular.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado de la derecha, en Transmisión HTTP, seleccione **[!UICONTROL Copiar URL]** a la derecha del visor que desee. Como práctica recomendada, copie la dirección URL asociada al `Universal_HTML5_Video` visor.
   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada al `Universal_HTML5_Video` visor.

   * Seleccionar **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada al `Universal_HTML5_Video` visor.

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]**, o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada al `Universal_HTML5_Video` visor.

1. Coloque el vínculo a la URL del vídeo HTML5 en el sitio web y el sitio de dispositivos móviles.

## Incrustar el visor de vídeo en una página web {#embedding-the-video-viewer-on-a-web-page}

Utilice la función de código incrustado si desea reproducir el vídeo incrustado en la página web. Copie el código incrustado en el portapapeles para pegarlo en sus páginas web. No se permite la edición del código en el cuadro de diálogo Código incrustado.

Consulte también [Vinculación de una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Para incrustar el visor de vídeo en una página web:**

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Vídeo]** o **[!UICONTROL Conjunto de vídeos adaptable]**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptables cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado de la derecha, en Transmisión HTTP, seleccione **[!UICONTROL Código incrustado]** a la derecha del visor que desee. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el `Universal_HTML5_Video` visor.
   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura de vídeo, seleccione **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el `Universal_HTML5_Video` visor.

   * Seleccionar **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el `Universal_HTML5_Video` visor.

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]**, o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el `Universal_HTML5_Video` visor.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. select **[!UICONTROL Cerrar]**.
1. Pegue el código incrustado en las páginas web.

### Implementar código incrustado para utilizar vídeo de HTML 5 con recursos de vídeo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Si no utiliza el reproductor de vídeo Adobe Dynamic Media Classic HTML5, sino el HTML nativo5 `<video>` con recursos de vídeo MP4, puede utilizar el siguiente ejemplo de código incrustado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Reemplazar `"S7 video thumbnail URL"` con la URL de la miniatura del vídeo, que es la imagen en miniatura del vídeo que ve un usuario antes de reproducir el vídeo.

  Consulte [Obtener URL de miniaturas de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Reemplazar `"S7 OGG video asset URL (no player)"` con la URL progresiva del vídeo para el vídeo OGG.

  Consulte [Vinculación de una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Reemplazar `"S7 MP4 mobile progressive video asset URL (no player)"` con la URL móvil progresiva del vídeo.

  Consulte [Vinculación de una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implementación de vídeo mediante un reproductor de vídeo de terceros {#deploying-video-using-a-third-party-video-player}

Si utiliza un reproductor de vídeo de terceros o un reproductor de vídeo personalizado en lugar de un visor de vídeo de Dynamic Media Classic, obtendrá la URL de vídeo directo que funciona para la descarga progresiva o la transmisión de vídeo a varias velocidades de bits HLS.

**Para implementar vídeo con un reproductor de vídeo de terceros:**

1. En Adobe Dynamic Media Classic, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Configuración general]**.
1. Según el tipo de URL que desee utilizar, realice una de las tareas siguientes:

* Para generar una URL de vídeo de flujo HLS directa (varias velocidades de bits)

  En el **[!UICONTROL Configuración general de la aplicación]** , en la **[!UICONTROL Servidores]** , en el **[!UICONTROL Servidor de publicación]** , construya la dirección URL directa. Utilice la siguiente sintaxis: `server/is/content/company/folder/filename.m3u8`

  Por ejemplo, supongamos que el nombre del servidor Publicado es `https://s7d9.scene7.com/.` Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Para generar una URL de vídeo de flujo HLS directa (velocidad de bits única)

  En el **[!UICONTROL Configuración general de la aplicación]** , en la **[!UICONTROL Servidores]** , en el **[!UICONTROL Nombre del servidor de flujo HLS]** , cree la dirección URL directa con la siguiente sintaxis:

  `server/company/folder/filename.ext.m3u8`

  Por ejemplo, supongamos que el nombre del servidor de flujo HLS es `https://s7mbrstream.scene7.com/hls-vod/`. Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Para generar una URL directa de vídeo progresivo

  En la página **[!UICONTROL Configuración general de la aplicación]**, en el grupo **[!UICONTROL Servidores]**, campo de texto **[!UICONTROL Nombre del servidor de vídeo progresivo]**, cree la URL de eVideo directa utilizando la siguiente sintaxis:

  `server/company/folder/filename`

  Por ejemplo, supongamos que el nombre del servidor de vídeo progresivo es `https://s7d9.scene7.com/is/content/`. Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Trabajo con miniaturas de vídeo {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genera miniaturas para vídeos codificados y vídeos precodificados. Puede utilizar las miniaturas de vídeo como cualquier otro recurso de imagen. Además, puede obtener las direcciones URL de las miniaturas de vídeo que genera Adobe Dynamic Media Classic. A continuación, puede implementar estas direcciones URL fuera de Adobe Dynamic Media Classic. Por ejemplo, puede implementar las miniaturas en resultados de búsquedas, listados de vídeos relacionados y listas de reproducción de vídeos en un sitio web.

Las miniaturas se generan en función del primer fotograma heterogéneo (no en un fotograma todo negro o todo blanco, etc. ) del vídeo.

### Obtener URL de miniaturas de vídeo {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genera miniaturas de vídeo automáticamente durante el proceso de carga. Las miniaturas aparecen en el panel Examinar de las vistas Lista y Cuadrícula.

Para generar direcciones URL para miniaturas de vídeo, realice una operación de publicación.

Consulte [Publicar vídeo](deploying-video-websites-mobile-sites.md#publishing_video).

Tras la publicación, puede obtener las URL de las miniaturas de vídeo en la vista de detalles del panel URL y código incrustado. Seleccionar **[!UICONTROL Copiar URL]** a la derecha de la miniatura del vídeo para copiar su URL.

### Modificación de fotogramas de póster en visores de vídeo {#modifying-poster-frames-in-video-viewers}

El *fotograma de póster* es el fotograma inicial que aparece en los visores de vídeo antes de que el vídeo empiece a reproducirse. Adobe Dynamic Media Classic utiliza miniaturas de vídeo como fotogramas de póster.

Puede aplicar modificadores de imagen al fotograma de póster. Por ejemplo, puede recortar el fotograma de póster o hacerlo transparente. Para modificar el fotograma de póster, abra la pantalla de configuración del visor de vídeo e introduzca modificadores en la sección Modificadores de imagen de póster. 

Consulte [Añadir o editar un ajuste preestablecido de visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [Guía del servicio de imágenes](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

También puede modificar las miniaturas de los vídeos agregando modificadores a las URL de las miniaturas de vídeo.

>[!MORELIKETHIS]
>
>* [Publicar archivos](publishing-files.md#publishing_files)