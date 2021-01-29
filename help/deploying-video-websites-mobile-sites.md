---
title: Distribución de vídeos en sitios web y sitios móviles
description: Aprenda a implementar vídeo en sus sitios web y sitios móviles.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 68%

---


# Distribución de vídeos en sitios web y sitios móviles{#deploying-video-to-your-websites-and-mobile-sites}

Los sitios web, los sitios móviles y las aplicaciones de escritorio acceden al contenido del servidor de Dynamic Media Classic, incluido el vídeo, mediante cadenas URL o código incrustado. Dynamic Media Classic activa estas cadenas URL durante el proceso de publicación. Para colocar la cadena URL o el código incrustado del vídeo en las páginas web, las páginas móviles y las aplicaciones de escritorio, debe copiar esta cadena desde Dynamic Media Classic.

>[!NOTE]
>
>La URL o el código incrustado no se activan hasta que publique el recurso.

## Publicación de vídeo  {#publishing-video}

La publicación de un vídeo permite a los servidores Dynamic Media Classic entregar vídeo en el sitio web, el sitio móvil o la aplicación.

Existen dos métodos que puede utilizar para publicar vídeos:

* **Publicación automática e instantánea de vídeos durante la carga**

   Como parte del proceso de carga de vídeo, Dynamic Media Classic puede publicar vídeos automáticamente al cargarlos y codificarlos. Esta capacidad para publicar inmediatamente significa que no es necesario publicar los vídeos por separado posteriormente.

* **Publicación manual de vídeos tras la carga**

   Si no desea publicar vídeos inmediatamente, puede publicar los vídeos manualmente en cualquier momento.

Después de publicar los vídeos, Dynamic Media Classic activa las cadenas URL de su página HTML o código de aplicación.

**Para publicar vídeos**

1. Realice una de las siguientes acciones:

   * Para publicar vídeos de forma automática e instantánea durante la carga, haga clic en **Publicar tras la carga** en la pantalla de carga. Ya ha terminado; no tiene que seguir más pasos.
   * Para publicar vídeos de forma manual tras carga, en el panel Examinar, seleccione los vídeos y a continuación, en la barra de navegación global, haga clic en **Publicar**.

## Vinculación de una URL de vídeo a sitios web o de dispositivos móviles {#linking-a-video-url-to-a-mobile-site-or-a-website}

Una vez que haya publicado un vídeo, puede obtener su URL para utilizarla en un sitio web, un sitio de dispositivos móviles o una aplicación de escritorio. Utilice las URL de vídeo cuando desee mostrar vídeo en una ventana emergente o modal por encima de la página web.

Cuando un cliente haga clic en el vínculo, se detectará automáticamente el dispositivo, el ancho de banda y el tamaño de la pantalla. Se mostrará el vídeo apropiado para la reproducción en el visor predefinido para el ordenador o en el reproductor de vídeo nativo del dispositivo smartphone o tablet.

Consulte también [ Incrustación del visor de vídeo en páginas web](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**Para vincular una URL de vídeo a sitios web o de dispositivos móviles**

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **Vídeo** o **Conjunto de vídeos adaptables**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptables cuyo código incrustado desee vincular.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula** o **Vista de lista**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, en Flujo HTTP, haga clic en **Copiar URL** a la derecha del visor que desee. Se recomienda copiar la URL asociada al visor `Universal_HTML5_Video`.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**. Se recomienda copiar la URL asociada al visor `Universal_HTML5_Video`.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**. Se recomienda copiar la URL asociada al visor `Universal_HTML5_Video`.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** > **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**. Se recomienda copiar la URL asociada al visor `Universal_HTML5_Video`.

1. Coloque el vínculo a la URL del vídeo HTML5 en el sitio web y el sitio de dispositivos móviles.

## Incrustación del visor de vídeo en páginas web  {#embedding-the-video-viewer-on-a-web-page}

Utilice la función de código incrustado si desea reproducir el vídeo incrustado en la página web. El código incrustado se copia en el portapapeles para pegarlo en las páginas web. No se permite la edición del código en el cuadro de diálogo Código incrustado.

Consulte también [Vinculación de una URL de vídeo a sitios web o de dispositivos móviles](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Para incrustar el visor de vídeo en una página web**

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **Vídeo** o **Conjunto de vídeos adaptables**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el vídeo o el conjunto de vídeos adaptables cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula** o **Vista de lista**. En el panel de exploración de recursos, haga doble clic en la miniatura de vídeo de un solo recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, en Flujo HTTP, haga clic en **Código incrustado** a la derecha del visor que desee. Como práctica recomendada, haga clic en **Código incrustado** que está asociado con el visor `Universal_HTML5_Video`.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** debajo de la imagen de la miniatura de vídeo.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**. Como práctica recomendada, haga clic en **Código incrustado** que está asociado con el visor `Universal_HTML5_Video`.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**. Como práctica recomendada, haga clic en **Código incrustado** que está asociado con el visor `Universal_HTML5_Video`.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** > **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**. Como práctica recomendada, haga clic en **Código incrustado** que está asociado con el visor `Universal_HTML5_Video`.

1. En el cuadro de diálogo Código incrustado, haga clic en **Copiar al portapapeles**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Haga clic en **Cerrar**.
1. Pegue el código incrustado en las páginas web.

### Implementación de código incrustado para utilizar vídeo HTML5 con recursos de vídeo MP4 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Si no utiliza el reproductor de vídeo Dynamic Media Classic HTML5, sino que desea utilizar la etiqueta nativa HTML5 `<video>` con recursos de vídeo MP4, puede utilizar la siguiente muestra de código incrustado:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Reemplace `"S7 video thumbnail URL"` por la URL de la miniatura del vídeo. Esta es la imagen en miniatura del vídeo que un usuario ve antes de reproducir el vídeo.

   Consulte [Obtención de las URL de miniaturas de vídeo](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Reemplace `"S7 OGG video asset URL (no player)"` por la URL progresiva del vídeo para vídeo OGG.

   Consulte [Vinculación de una URL de vídeo a sitios web o de dispositivos móviles](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Reemplace `"S7 MP4 mobile progressive video asset URL (no player)"` por la URL móvil progresiva del vídeo.

   Consulte [Vinculación de una URL de vídeo a sitios web o de dispositivos móviles](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Implementación de vídeo con un reproductor de vídeo de terceros  {#deploying-video-using-a-third-party-video-player}

Si utiliza un reproductor de vídeo de terceros o un reproductor de vídeo integrado personalizado en lugar de un visor de vídeo Dynamic Media Classic, puede obtener la URL de vídeo directa que funciona para el flujo de vídeo de varias velocidades de bits HLS o la descarga progresiva.

**Para implementar vídeo con un reproductor de vídeo de terceros**

1. En Dynamic Media Classic, en la barra de navegación global, haga clic en **Configuración** > **Ajustes de aplicación** > **Configuración general**.
1. Según el tipo de URL que desee utilizar, realice una de las tareas siguientes:
* Para generar una URL directa de vídeo de flujo HLS (varias velocidades de bits)

   En la página **Configuración general de la aplicación**, en el grupo **Servidores**, en el campo de texto **Nombre del servidor publicado**, cree la dirección URL directa con la siguiente sintaxis: `server/is/content/company/folder/filename.m3u8`
Por ejemplo, supongamos que el nombre del servidor Publicado es `https://s7d9.scene7.com/.` Con la sintaxis del paso 2, la dirección URL directa podría tener el siguiente aspecto:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* Para generar una URL directa de vídeo de flujo HLS (velocidad de bits única)

   En la página **Configuración general de la aplicación**, en el grupo **Servidores**, en el campo de texto **Nombre del servidor de flujo HLS**, cree la dirección URL directa con la siguiente sintaxis:
   `server/company/folder/filename.ext.m3u8`
Por ejemplo, supongamos que el nombre del servidor de flujo HLS es  `https://s7mbrstream.scene7.com/hls-vod/`. Utilizando la sintaxis en el paso 2, la dirección URL directa puede tener el siguiente aspecto:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* Para generar una URL directa de vídeo progresivo

   En la página **Configuración general de la aplicación**, en el grupo **Servidores**, campo de texto **Nombre del servidor de vídeo progresivo**, cree la URL de eVideo directa utilizando la siguiente sintaxis:  `server/company/folder/filename`
Por ejemplo, supongamos que el nombre del servidor de vídeo progresivo es  `https://s7d9.scene7.com/is/content/`. Utilizando la sintaxis en el paso 2, la dirección URL directa puede tener el siguiente aspecto:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Uso de las miniaturas de vídeo {#working-with-video-thumbnails}

Dynamic Media Classic genera miniaturas para vídeos codificados y vídeos precodificados. Puede utilizar las miniaturas de vídeo como cualquier otro recurso de imagen. Además, puede obtener direcciones URL para las miniaturas de vídeo que Dynamic Media Classic genera e implementar estas URL fuera de Dynamic Media Classic. Por ejemplo, puede implementar las miniaturas en resultados de búsquedas, listados de vídeos relacionados y listas de reproducción de vídeos en un sitio web.

Las miniaturas se generan en función del primer fotograma heterogéneo (no en un fotograma todo negro o todo blanco, etc. ) del vídeo.

### Obtención de las URL de miniaturas de vídeo {#obtaining-video-thumbnail-urls}

Dynamic Media Classic genera automáticamente miniaturas de vídeo durante el proceso de carga. Las miniaturas aparecen en el panel Examinar en la vista de lista y en la vista de cuadrícula.

Para generar direcciones URL para miniaturas de vídeo, realice una operación de publicación.

Consulte [Publicación de vídeo](deploying-video-websites-mobile-sites.md#publishing_video).

Tras la publicación, puede obtener las URL de las miniaturas de vídeo en la vista de detalles del panel URL y código incrustado. Haga clic en **Copiar URL** a la derecha de la miniatura de vídeo para copiar su dirección URL.

### Modificación de fotogramas de póster en visores de vídeos  {#modifying-poster-frames-in-video-viewers}

El *fotograma de póster* es el fotograma inicial que aparece en los visores de vídeo antes de que el vídeo empiece a reproducirse. Dynamic Media Classic utiliza miniaturas de vídeo como fotogramas de póster.

Puede aplicar modificadores de imagen al fotograma de póster. Por ejemplo, puede recortar el fotograma de póster o hacerlo transparente. Para modificar el fotograma de póster, abra la pantalla de configuración del visor de vídeo e introduzca modificadores en la sección Modificadores de imagen de póster. 

Consulte [Adición o edición de un ajuste preestablecido de visor de vídeo](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Consulte [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

También puede modificar las miniaturas de los vídeos agregando modificadores a las URL de las miniaturas de vídeo.

>[!MORELIKETHIS]
>
>* [Publicar archivos ](publishing-files.md#publishing_files)

