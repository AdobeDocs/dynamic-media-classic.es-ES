---
title: Distribución de vídeo en los sitios web y sitios móviles
description: Obtenga información sobre cómo implementar vídeo en sus sitios web y sitios móviles desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 23%

---

# Distribución de vídeo en los sitios web y sitios móviles{#deploying-video-to-your-websites-and-mobile-sites}

Los sitios web, los sitios móviles y las aplicaciones de escritorio acceden al contenido del servidor de Adobe Dynamic Media Classic, incluido el vídeo, mediante cadenas URL o código incrustado. Adobe Dynamic Media Classic activa estas cadenas URL durante el proceso de publicación. Para colocar la cadena URL o el código incrustado del vídeo en las páginas web, páginas móviles y aplicaciones de escritorio, cópielo desde Adobe Dynamic Media Classic.

>[!NOTE]
>
>La URL o el código de incrustación no estarán activos hasta que publique el recurso.

## Publicación de vídeo {#publishing-video}

La publicación de un vídeo permite a los servidores de Adobe Dynamic Media Classic enviar vídeos a su sitio web, sitio móvil o aplicación.

Existen dos métodos diferentes que puede utilizar para publicar vídeos:

* **Vídeos de Publish de forma automática e instantánea al cargar**: Como parte del proceso de carga de vídeos, Adobe Dynamic Media Classic puede publicar vídeos automáticamente cuando se cargan y codifican. Esta capacidad de publicación instantánea significa que no hay necesidad de publicar vídeos por separado después del hecho.

* **Vídeo de Publish manualmente después de la carga**: Si no desea publicar vídeos inmediatamente, puede publicarlos manualmente en cualquier momento.

Después de publicar los vídeos, Adobe Dynamic Media Classic activa las cadenas URL de la página del HTML o del código de la aplicación.

**Para publicar el vídeo:**

1. Realice una de las siguientes acciones:

   * Para publicar vídeos de forma automática e instantánea al cargar, en la página Cargar, selecciona **[!UICONTROL Publish después de cargar]**. Ya ha terminado; no tiene que seguir más pasos.
   * Para publicar vídeos manualmente después de la carga, en el panel Examinar, selecciona los vídeos y, a continuación, en la barra de navegación global, selecciona **Publish**.

## Vinculación de una URL de vídeo a un sitio móvil o sitio web {#linking-a-video-url-to-a-mobile-site-or-a-website}

Al publicar un vídeo, puede obtener su URL asociada para utilizarlo en su sitio web, sitio móvil o aplicación de escritorio. Utilice la dirección URL del vídeo cuando desee mostrar el vídeo en una ventana emergente o modal en la parte superior de la página web.

Cuando un cliente selecciona el vínculo, se detectan automáticamente su dispositivo, ancho de banda y tamaño de pantalla. Se mostrará el vídeo apropiado para la reproducción en el visor predefinido para el ordenador o en el reproductor de vídeo nativo del dispositivo smartphone o tablet.

Vea también [Incrustar el visor de vídeo en una página web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Para vincular una dirección URL de vídeo a un sitio móvil o sitio web:**

1. En el panel Examinar recursos, en la lista desplegable **[!UICONTROL Mostrar]**, seleccione **[!UICONTROL Vídeo]** o **[!UICONTROL Conjunto de vídeos adaptable]**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptables cuyo código incrustado desee vincular.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado que se encuentra a la derecha, en Transmisión HTTP, seleccione **[!UICONTROL Copiar URL]** a la derecha del visor que desee. Como práctica recomendada, copie la dirección URL asociada con el visor `Universal_HTML5_Video`.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada con el visor `Universal_HTML5_Video`.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada con el visor `Universal_HTML5_Video`.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**. Como práctica recomendada, copie la dirección URL asociada con el visor `Universal_HTML5_Video`.

1. Coloque el vínculo a la URL del vídeo HTML5 en el sitio web y el sitio de dispositivos móviles.

## Incrustar el visor de vídeo en una página web {#embedding-the-video-viewer-on-a-web-page}

Utilice la función Código incrustado cuando desee reproducir el vídeo incrustado en la página web. El código incrustado se copia en el portapapeles para pegarlo en las páginas Web. No se permite la edición del código en el cuadro de diálogo Código incrustado.

Ver también [Vincular una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Para incrustar el visor de vídeo en una página Web:**

1. En el panel Examinar recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Vídeo]** o **[!UICONTROL Conjunto de vídeos adaptable]**.
1. en el panel Biblioteca de recursos, en el lado izquierdo, navegue hasta la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptable cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel Direcciones URL y código incrustado que se encuentra a la derecha, en Transmisión HTTP, seleccione **[!UICONTROL Código incrustado]** a la derecha del visor que desee. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el visor `Universal_HTML5_Video`.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura de vídeo, seleccione **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el visor `Universal_HTML5_Video`.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el visor `Universal_HTML5_Video`.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**. Como práctica recomendada, seleccione **[!UICONTROL Código incrustado]** que está asociado con el visor `Universal_HTML5_Video`.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al Portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. seleccione **[!UICONTROL Cerrar]**.
1. Pegue el código incrustado en las páginas web.

### Implementar código incrustado para utilizar vídeo de HTML5 con recursos de vídeo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Es posible que no desee utilizar el reproductor de vídeo Adobe Dynamic Media Classic HTML5. En su lugar, si desea utilizar la etiqueta nativa HTML5 `<video>` con recursos de vídeo MP4, puede utilizar el siguiente ejemplo de código incrustado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Reemplace `"S7 video thumbnail URL"` por la URL de la miniatura del vídeo, que es la imagen en miniatura que el usuario ve antes de reproducir el vídeo.

  Ver [Obtener URL de miniaturas de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Reemplace `"S7 OGG video asset URL (no player)"` por la URL progresiva del vídeo para el vídeo OGG.

  Ver [Vincular una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Reemplace `"S7 MP4 mobile progressive video asset URL (no player)"` por la URL móvil progresiva del vídeo.

  Ver [Vincular una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implementación de vídeo mediante un reproductor de vídeo de terceros {#deploying-video-using-a-third-party-video-player}

Si utiliza reproductores de vídeo de terceros o un reproductor de vídeo personalizado en lugar de un visor de vídeo de Dynamic Media Classic, obtendrá la URL de vídeo directo que funciona para la descarga progresiva o la transmisión de vídeo a varias velocidades de bits HLS.

**Para implementar vídeo mediante un reproductor de vídeo de terceros:**

1. En Adobe Dynamic Media Classic, en la barra de navegación global, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración general]**.
1. Según el tipo de URL que desee utilizar, realice una de las tareas siguientes:

* Para generar una URL de vídeo de flujo HLS directa (varias velocidades de bits)

  En la página **[!UICONTROL Configuración general de la aplicación]**, en el grupo **[!UICONTROL Servidores]**, en el campo de texto **[!UICONTROL Nombre del servidor publicado]**, cree la dirección URL directa. Utilice la siguiente sintaxis: `server/is/content/company/folder/filename.m3u8`

  Por ejemplo, supongamos que el nombre del servidor publicado es `https://s7d9.scene7.com/.`. Utilizando la sintaxis del paso 2, la dirección URL directa podría tener el aspecto siguiente:
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Para generar una URL de vídeo de flujo HLS directa (velocidad de bits única)

  En la página **[!UICONTROL Configuración general de la aplicación]**, en el grupo **[!UICONTROL Servidores]**, en el campo de texto **[!UICONTROL Nombre del servidor de flujo HLS]**, cree la dirección URL directa con la siguiente sintaxis:

  `server/company/folder/filename.ext.m3u8`

  Por ejemplo, supongamos que el nombre del servidor de flujo HLS es `https://s7mbrstream.scene7.com/hls-vod/`. Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Para generar una URL directa de vídeo progresivo

  En la página **[!UICONTROL Configuración general de la aplicación]**, en el grupo **[!UICONTROL Servidores]**, campo de texto **[!UICONTROL Nombre del servidor de vídeo progresivo]**, cree la URL de eVideo directa utilizando la siguiente sintaxis:

  `server/company/folder/filename`

  Por ejemplo, suponga que el nombre del servidor de vídeo progresivo es `https://s7d9.scene7.com/is/content/`. Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Trabajo con miniaturas de vídeo {#working-with-video-thumbnails}

Adobe Dynamic Media Classic genera miniaturas para vídeos codificados y vídeos precodificados. Puede utilizar las miniaturas de vídeo como cualquier otro recurso de imagen. Además, puede obtener las direcciones URL de las miniaturas de vídeo que genera Adobe Dynamic Media Classic. A continuación, puede implementar estas direcciones URL fuera de Adobe Dynamic Media Classic. Por ejemplo, puede implementar las miniaturas en resultados de búsquedas, listados de vídeos relacionados y listas de reproducción de vídeos en un sitio web.

Las miniaturas se generan en función del primer fotograma heterogéneo (no en un fotograma todo negro o todo blanco, etc. ) del vídeo.

### Obtener URL de miniaturas de vídeo {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic genera miniaturas de vídeo automáticamente durante el proceso de carga. Las miniaturas aparecen en el panel Examinar de las vistas Lista y Cuadrícula.

Para generar direcciones URL para miniaturas de vídeo, realice una operación de publicación.

Ver [vídeo de Publish](deploying-video-websites-mobile-sites.md#publishing_video).

Tras la publicación, puede obtener las URL de las miniaturas de vídeo en la vista de detalles del panel URL y código incrustado. Seleccione **[!UICONTROL Copiar URL]** a la derecha de la miniatura de vídeo para poder copiar su URL asociada.

### Modificación de fotogramas de póster en visores de vídeo {#modifying-poster-frames-in-video-viewers}

El *fotograma de póster* es el fotograma inicial que aparece en los visores de vídeo antes de que el vídeo empiece a reproducirse. Adobe Dynamic Media Classic utiliza miniaturas de vídeo como fotogramas de póster.

Puede aplicar modificadores de imagen al fotograma de póster. Por ejemplo, puede recortar el fotograma de póster o hacerlo transparente. Para modificar el fotograma de póster, abra la pantalla de configuración del visor de vídeo e introduzca modificadores en la sección Modificadores de imagen de póster. 

Consulte [Agregar o editar un ajuste preestablecido de visualizador de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [Guía de servicio de imágenes](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api).

También puede modificar las miniaturas de los vídeos agregando modificadores a las URL de las miniaturas de vídeo.

>[!MORELIKETHIS]
>
>* [archivos de Publish](publishing-files.md#publishing_files)