---
title: Carga y codificación de vídeos
description: Obtenga información sobre cómo cargar y codificar vídeos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '3989'
ht-degree: 40%

---

# Carga y codificación de vídeos{#uploading-and-encoding-videos}

Para crear conjuntos de vídeo adaptable o de vídeo único para su envío a la web o a dispositivos móviles, primero debe cargar los archivos de vídeo principales en Adobe Dynamic Media Classic. Adobe Dynamic Media Classic codifica los vídeos en formato MP4 y publica vídeo en los siguientes formatos de archivo:

* **MP4**: Adobe Dynamic Media Classic recomienda MP4 como formato de archivo de vídeo preferido. Utilice archivos MP4 para lo siguiente:

   * Flujo dinámico HTTP en equipos de escritorio.
   * HTTP Live Streaming (protocolo de flujo de Apple).
   * Envío de vídeo progresivo a dispositivos móviles Android™, BlackBerry® y Windows®

  Adobe Dynamic Media Classic ofrece dos flujos de trabajo para cargar archivos de vídeo:

* **Vídeos precodificados**: Los archivos MP4 se cargan directamente en Adobe Dynamic Media Classic. Con este flujo de trabajo, los archivos no se codifican al cargarlos. Los archivos se codifican previamente como preparación para la publicación en el escritorio y los dispositivos móviles.

* **Vídeos de origen principales**: cargue archivos de vídeo de origen principales y, al cargarlos, codifique estos archivos en archivos MP4. Los vídeos codificados se etiquetan como &quot;Vídeo&quot; en el panel Examinar. Adobe Dynamic Media Classic admite la codificación de archivos de vídeo en muchos formatos.

   * Asegúrese de que los archivos de vídeo de origen principales que desea codificar sean compatibles.

     Consulte [Tipos de archivos de vídeo compatibles para la codificación](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Elija un ajuste preestablecido de codificación de vídeo.

     Consulte [Ajustes preestablecidos de vídeo para la codificación de archivos de vídeo](application-setup.md#video-presets-for-encoding-video-files)

     Consulte [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic también genera miniaturas de vídeo. Puede obtener más información sobre las miniaturas de vídeo, la obtención de sus URL y la modificación de fotogramas de póster.

Consulte [Trabajo con miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para cargar y codificar vídeos:**

Realice una de las siguientes acciones.

*Si los vídeos ya están codificados*

1. En la barra de navegación global, seleccione **[!UICONTROL Cargar]**.
1. En la página Cargar, seleccione **[!UICONTROL Desde el escritorio]** pestaña.
1. En la página Cargar, en el **[!UICONTROL Seleccionar archivos para cargar]** panel, seleccionar **[!UICONTROL Examinar]**, vaya a un archivo de vídeo MP4 y, a continuación, seleccione **[!UICONTROL Abrir]**.
1. En el elegido **[!UICONTROL Destino de carpeta]** , seleccione una carpeta para el archivo cargado.
1. En la página Cargar, asegúrese de que **[!UICONTROL Publicar tras la carga]** está marcada.
1. Seleccionar **[!UICONTROL Cargar envío]**.

*Si desea codificar los vídeos con Adobe Dynamic Media Classic*

1. En la barra de navegación global, seleccione **[!UICONTROL Cargar]**.
1. En la página Cargar, seleccione **[!UICONTROL Desde el escritorio]** pestaña.
1. En el **[!UICONTROL Seleccionar archivos para cargar]** panel, seleccionar **[!UICONTROL Examinar]**, vaya a un archivo de vídeo de origen principal y, a continuación, seleccione **[!UICONTROL Abrir]**.
1. En el elegido **[!UICONTROL Destino de carpeta]** , seleccione una carpeta para el archivo cargado.
1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Opciones de trabajo]**,
1. En el cuadro de diálogo Opciones del trabajo de carga, expanda **[!UICONTROL Opciones de vídeo]**, a continuación, realice una de las siguientes acciones:

   * La práctica recomendada es seleccionar **[!UICONTROL Codificación de vídeo adaptable]**. Consulte [Vídeo adaptable (predeterminado)](application-setup.md#adaptive-video-default).
   * Opcional. Si desea utilizar una configuración de codificación individual, expanda **[!UICONTROL Ajustes preestablecidos de codificación única]**y, a continuación, seleccione las opciones de codificación que desee para Escritorio, Móvil y Tablet.
Consulte [Ajustes preestablecidos de codificación de vídeo para equipos de escritorio](application-setup.md#desktop-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para dispositivos móviles](application-setup.md#mobile-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para tablets](application-setup.md#tablet-video-encoding-presets).
1. En el cuadro de diálogo Opciones del trabajo de carga, seleccione **[!UICONTROL Guardar]**.
1. En la página Cargar, asegúrese de que **[!UICONTROL Publicar tras la carga]** está marcada.
1. En la página Cargar, en la esquina inferior derecha, seleccione **[!UICONTROL Cargar envío]**.

*Si desea volver a codificar un archivo de vídeo que haya cargado anteriormente*

1. En Adobe Dynamic Media Classic, en el panel Examinar, vaya al vídeo y selecciónelo.
1. Ir a **[!UICONTROL Archivo]** > **[!UICONTROL Reprocesar]**.
1. En el cuadro de diálogo Volver a procesar recursos, expanda **[!UICONTROL Opciones de vídeo]**, a continuación, realice una de las siguientes acciones:
   * La práctica recomendada es utilizar el siguiente método. Seleccionar **Vídeo adaptable**.
Consulte [Vídeo adaptable (predeterminado)](application-setup.md#adaptive-video-default).
   * Opcional. Si desea utilizar una configuración de codificación individual, expanda **[!UICONTROL Ajustes preestablecidos de codificación única]**y, a continuación, seleccione las opciones de codificación que desee para Escritorio, Móvil y Tablet.
Consulte [Ajustes preestablecidos de codificación de vídeo para equipos de escritorio](application-setup.md#desktop-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para dispositivos móviles](application-setup.md#mobile-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para tablets](application-setup.md#tablet-video-encoding-presets).
1. En el cuadro de diálogo Volver a procesar recursos, seleccione **[!UICONTROL Enviar]**.

Cuando se utiliza un ajuste preestablecido de codificación de vídeo adaptable o varios ajustes preestablecidos de codificación única, el resultado es un conjunto de vídeos adaptable que se crea automáticamente con varias codificaciones de vídeo. También puede crear manualmente un conjunto de vídeos adaptables seleccionando los vídeos individuales.

Cuando se genera un conjunto de vídeos adaptables automáticamente o manualmente, solo se crean tipos de archivo MP4 y M4V.

## Tipos de archivo de vídeo compatibles para la codificación {#supported-video-file-types-for-encoding}

En la siguiente tabla se muestran los tipos de archivo de vídeo (con los códecs de vídeo permitidos) que puede codificar al formato MP4 u OGV al cargar los archivos. En la tabla se muestran los formatos de archivo y códecs:

* **Formatos de archivo de vídeo**: similar a un archivo ZIP, un formato de archivo de vídeo determina cómo se incluyen los archivos en el archivo de vídeo. Un archivo de vídeo suele contener varias pistas, una pista de vídeo (sin audio) y una o más pistas de audio (sin vídeo), que están interrelacionadas y sincronizadas. El formato de archivo de vídeo determina cómo se organizan estas distintas pistas de datos y metadatos.

* **Códecs de vídeo**: Un códec de vídeo describe el algoritmo por el que se codifica un vídeo. Un reproductor de vídeo descodifica el vídeo según su códec y, a continuación, reproduce una serie de imágenes, o fotogramas, en la pantalla. Los códecs minimizan la cantidad de información que tienen que almacenar los archivos de vídeo para reproducir el vídeo. En lugar de almacenar información sobre cada fotograma individual, sólo se almacena información sobre las diferencias entre uno y otro. Debido a que la mayoría de los vídeos cambian poco de un fotograma a otro, los códecs permiten altas tasas de compresión, lo que da como resultado tamaños de archivo más pequeños.

  | Formato de archivo de vídeo | Códecs de vídeo |
  | --- | --- |
  | 3GP | H.263, H.264 |
  | AVI | DivX, DV |
  | M2P | MPEG-2 PS |
  | M2T | MPEG-2 TS |
  | M2TS | MPEG-2 TS |
  | M2V | MPEG-2 ES |
  | M4V | H.264  |
  | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
  | MP4 | `H.264/MPEG-4` AVC |
  | MPEG | MPEG-2 SS |
  | MPG | MPEG-2 SS |
  | MTS | MPEG-2 |
  | ProRes | APCN, APCS, APCO, APCH, AP4H |
  | TS | DVCPro 50 |
  | VOB | MPEG-2 |
  | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

  >[!NOTE]
  >
  >La pantalla Trabajos le avisa si carga e intenta codificar un archivo de vídeo pero este se rechaza porque contiene un códec o contenedor de archivos no compatible. Para obtener más información, consulte [Comprobar archivos de trabajo](checking-job-files.md).

## Prácticas recomendadas para la codificación de vídeo {#best-practices-for-video-encoding}

A continuación se ofrecen sugerencias recomendadas para codificar archivos de vídeo de origen en Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Archivos de vídeo de origen {#source-video-files}

Al codificar un archivo de vídeo, utilice el archivo de vídeo de origen de la máxima calidad posible. Evite utilizar archivos de vídeo codificados previamente, ya que estos archivos ya están comprimidos y una codificación adicional crearía un vídeo de mala calidad.

En la tabla siguiente se describe el tamaño recomendado, la relación de aspecto y la velocidad de bits mínima que deben tener los archivos de vídeo de origen al codificarlos:

| Tamaño | Proporción de aspecto | Velocidad de bits mínima |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 4500 Kbps para la mayoría de vídeos. |
| 1280 X 720 | 16:9 | 3.000: 6.000 kbps, en función de la cantidad de movimiento del vídeo. |
| 1920 X 1080 | 16:9 | 6.000: 8.000 kbps, en función de la cantidad de movimiento del vídeo. |

### Obtener los metadatos de un archivo {#obtaining-a-file-s-metadata}

Puede obtener los metadatos de un archivo visualizando sus metadatos en Adobe Dynamic Media Classic, utilizando una herramienta de edición de vídeo o utilizando una aplicación diseñada para obtener metadatos. A continuación se indican instrucciones para utilizar MediaInfo, una aplicación de terceros, para obtener los metadatos de un archivo de vídeo:

1. Ir a esta página web: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Seleccione y descargue el instalador para la versión de interfaz gráfica de usuario y siga las instrucciones de instalación.
1. Después de la instalación, haga clic con el botón derecho en el archivo de vídeo (solo Windows®) y seleccione MediaInfo o abra MediaInfo y arrastre el archivo de vídeo a la aplicación. Se ven todos los metadatos asociados al archivo de vídeo, incluida su anchura, su altura y los fotogramas por segundo.

### Proporción de aspecto {#aspect-ratio}

Cuando seleccione o cree un ajuste preestablecido de codificación de vídeo para el archivo de vídeo principal, asegúrese de que el ajuste preestablecido tenga la misma proporción de aspecto que el archivo de vídeo principal. La *proporción de aspecto* es la proporción de anchura y altura del vídeo.

Para determinar la proporción de aspecto de un archivo de vídeo, obtenga los metadatos del archivo y anote la anchura y altura del archivo (consulte [Obtener los metadatos de un archivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). A continuación, utilice esta fórmula para determinar la proporción de aspecto:

Anchura / Altura = Proporción de aspecto

En la tabla siguiente se describe cómo se traducen los resultados de la fórmula en opciones comunes de proporción de aspecto:

| Resultado de la fórmula | Proporción de aspecto |
| --- | --- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Por ejemplo, un vídeo de 1440 de anchura × 1080 de altura tiene una relación de aspecto de 1440/1080 o 1,33. En este caso, elija un ajuste preestablecido de codificación de vídeo con una relación de aspecto de 4:3 para codificar el archivo de vídeo.

### Velocidad de datos {#data-rate}

El *velocidad de datos* (también llamado *velocidad de bits*) es la cantidad de datos codificados para formar un solo segundo de reproducción de vídeo. La velocidad de datos se mide en kilobits por segundo (kbps).

>[!NOTE]
>
>debido a que todos los códecs utilizan la compresión con pérdida, la velocidad de datos es el factor más importante en lo que respecta a la calidad de vídeo. En la compresión con pérdida, cuanto más se comprima un archivo de vídeo, más se degrada la calidad. Por este motivo, si se mantienen las demás características (la resolución, la velocidad de fotogramas y el códec), cuanto menor sea la velocidad de los datos, menor será la calidad del archivo comprimido.

Cuando elija un ajuste preestablecido de codificación de vídeo, recuerde tener en cuenta la velocidad de conexión del usuario final de destino. Elija un ajuste preestablecido con una velocidad de datos del 80 % de esa velocidad. Por ejemplo, si la velocidad de conexión del usuario final de destino es de 1000 Kbps, el mejor ajuste preestablecido es uno con una velocidad de datos de vídeo de 800 Kbps.

En esta tabla se describe la velocidad de datos de las velocidades de conexión habituales.

| Velocidad (kbps) | Tipo de conexión |
| --- | --- |
| 256 | Conexión de marcación. |
| 800 | Conexión móvil habitual. Para esta conexión, utilice una velocidad de datos en el rango de 400 a 800 para experiencias 3G. |
| 2000 | Conexión de escritorio de ancho de banda habitual. Para esta conexión, utilice una velocidad de datos en el rango de 800 a 2000 kbps, con velocidades medias entre 1200 y 1500 kbps. |
| 5000 | Conexión de gran ancho de banda habitual. La codificación en este rango superior no se recomienda, porque la mayoría de los usuarios no pueden recibir el vídeo a esta velocidad. |

### Resolución {#resolution}

*Resolución* describe la altura y anchura de un archivo de vídeo en píxeles. La mayor parte del vídeo de origen se almacena en alta resolución (por ejemplo, 1920 × 1080). Para fines de streaming, el vídeo de origen se comprime con una resolución más pequeña (640 × 480 o menor).

La resolución y la velocidad de datos son dos factores totalmente vinculados que determinan la calidad de vídeo. Para mantener la misma calidad de vídeo, cuanto mayor sea el número de píxeles de un archivo de vídeo (cuanto mayor sea la resolución), mayor será la velocidad de datos. Por ejemplo, considere el número de píxeles por fotograma en una resolución de 320 × 240 y un archivo de vídeo de resolución de 640 × 480:

| Resolución | Píxeles por fotograma |
| --- | --- |
| 320 × 240 | 76.800 |
| 640 × 480 | 307.200 |

El archivo de 640 × 480 tiene cuatro veces más píxeles por fotograma. Para lograr la misma velocidad de datos para estas dos resoluciones de ejemplo, se aplica cuatro veces la compresión al archivo de 640 × 480, lo que puede reducir la calidad del vídeo. Por lo tanto, una velocidad de datos de vídeo de 250 Kbps produce una visualización de alta calidad con una resolución de 320 × 240, pero no con una resolución de 640 × 480.

>[!NOTE]
>
>En general, cuanto mayor sea la velocidad de datos que utilice, mejor aparecerá el vídeo y, cuanto mayor sea la resolución que utilice, mayor será la velocidad de datos que deberá mantener con calidad de visualización (en comparación con resoluciones más bajas).

Debido a que la resolución y la velocidad de datos están vinculadas, al codificar el vídeo dispone de dos opciones:

* Elija una velocidad de datos y, a continuación, codifique con la resolución más alta que mejor se adapte a la velocidad de datos elegida.
* Elegir una resolución y, a continuación, codificar con la velocidad de datos necesaria para lograr un vídeo de gran calidad a la resolución elegida.

Cuando elija (o cree) un ajuste preestablecido de codificación de vídeo para el archivo de vídeo principal, utilice esta tabla para seleccionar la resolución correcta:

| Resolución | Altura (píxeles) | Tamaño de la pantalla |
| --- | --- | --- |
| 240p | 240 | Pantalla muy pequeña |
| 300p | 300 | Pantallas pequeñas normalmente para dispositivos móviles |
| 360p | 360 | Pantalla pequeña |
| 480p | 480 | Pantalla intermedia |
| 720p | 720 | Pantalla grande |
| 1080p | 1080 | Pantalla grande de alta definición |

### FPS (fotogramas por segundo) {#fps-frames-per-second}

En Estados Unidos y Japón, la mayoría de los vídeos se graban a 29,97 fotogramas por segundo (FPS); en Europa, la mayoría de los vídeos se graban a 25 FPS. La película se filma a 24 FPS.

Elija un ajuste preestablecido de codificación de vídeo que coincida con la velocidad de FPS del archivo de vídeo principal. Por ejemplo, si el vídeo principal es de 25 FPS, elija un ajuste preestablecido de codificación con 25 FPS. De forma predeterminada, todas las codificaciones personalizadas utilizan el FPS del archivo de vídeo principal. Por este motivo, no es necesario especificar la configuración de FPS al crear un ajuste preestablecido de codificación de vídeo.

### Dimensiones de codificación de vídeo {#video-encoding-dimensions}

Para obtener resultados óptimos, seleccione unas dimensiones de codificación de forma que el vídeo de origen sea un múltiplo entero de todos los vídeos codificados.

Para calcular esta proporción, divida la anchura del archivo de origen entre la anchura del archivo codificado. Seguidamente, divida la altura del archivo de origen entre la altura del archivo codificado para obtener la proporción de altura.

Si la proporción resultante es un número entero, el vídeo tendrá una escala óptima. Si la proporción resultante no es un número entero, la calidad del vídeo se verá afectada por defectos de píxeles en la pantalla. Este efecto resulta más evidente cuando el vídeo tiene texto.

Por ejemplo, supongamos que el vídeo de origen es 1920 × 1080. En la tabla siguiente, los tres vídeos codificados ofrecen los ajustes de codificación óptimos que deben utilizarse.

| Tipo de vídeo | Anchura × altura | Proporción de anchura | Proporción de altura |
| --- | --- | --- | --- |
| Origen | 1920 × 1080 | 1 | 1 |
| Codificado | 960 × 540 | 2 | 2 |
| Codificado | 640 × 360 | 3 | 3 |
| Codificado | 480 × 270 | 4 | 4 |

### Formato de archivo de vídeo codificado {#encoded-video-file-format}

Adobe Dynamic Media Classic recomienda utilizar ajustes preestablecidos de codificación de vídeo MP4 H.264. Dado que los archivos MP4 usan el códec de vídeo H.264, proporcionan vídeo de alta calidad pero con un tamaño de archivo comprimido.

## Trabajar con ajustes preestablecidos de codificación de vídeo {#working-with-video-encoding-presets}

Los archivos de vídeo principales creados con equipos de producción de vídeo y software de edición de vídeo suelen ser demasiado grandes y no tienen el formato adecuado para su distribución a destinos en línea. Para convertir vídeo digital al formato y especificaciones correctos para la reproducción en distintas pantallas, puede *transcodificar* archivos de vídeo (un proceso que también se denomina *codificación*). Durante el proceso de codificación, el vídeo se comprime en un tamaño de archivo más pequeño y eficaz. Lo hace para una entrega óptima a la web y a los dispositivos móviles.

Consulte [Carga y codificación de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic le ofrece una biblioteca de ajustes preestablecidos de codificación de vídeo predefinidos que reflejan los ajustes de codificación más comunes utilizados en la actualidad. Estos ajustes preestablecidos de codificación se han optimizado para la reproducción en pantallas de destino. Además, los administradores pueden crear sus propios ajustes preestablecidos de codificación de vídeo para personalizar el tamaño y la calidad de reproducción de vídeos para los usuarios finales. Todos los ajustes preestablecidos de codificación de vídeo, ya sea de forma predeterminada de Adobe Dynamic Media Classic o personalizados, emiten vídeo en formato de archivo MP4.

En la pantalla Ajustes preestablecidos de vídeo, los administradores pueden configurar y administrar la codificación de vídeo. Pueden hacer lo siguiente:

* Activar y desactivar ajustes preestablecidos de codificación de vídeo.
* Crear un ajuste preestablecido de codificación de vídeo.
* Editar ajustes preestablecidos de codificación de vídeo.
* Eliminar ajustes preestablecidos de vídeo.

Cualquier vídeo que cargue en Adobe Dynamic Media Classic o que codifique en Adobe Dynamic Media Classic se tratará como &quot;vídeo&quot;. Es decir, con esta clasificación de los recursos, podrá publicar el vídeo para reproducirlo en equipos de escritorio, dispositivos móviles, o ambos. Por ejemplo, puede obtener una vista previa de estos tipos de vídeos en Adobe Dynamic Media Classic. También puede generar direcciones URL (con la función de Copiar URL) y código que puede incrustar (con la función de Código incrustado) para su uso con los reproductores de vídeo, en sitios web, etc.

Consulte [Vista previa de vídeos en un visor de vídeos](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vinculación de una URL de vídeo a un sitio móvil o sitio web](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incrustar el visor de vídeo en una página web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para los recursos de vídeo que se cargan y codifican en Adobe Dynamic Media Classic, el vídeo se entrega en el siguiente formato de archivo:

**MP4 H.264** Utilice archivos MP4 para lo siguiente:

* Flujo dinámico HTTP en equipos de escritorio.
* HLS (flujo en directo HTTP, protocolo de flujo de Apple).
* Envío de vídeo progresivo a dispositivos móviles Android™, BlackBerry® y Windows®.

Cualquier otro formato de vídeo y códec se trata como &quot;Vídeo principal&quot;. Esta clasificación de los recursos implica que el vídeo es un archivo de origen y no se puede utilizar para su reproducción en escritorios ni dispositivos móviles. Por ejemplo, no puede obtener una vista previa de estos tipos de vídeos en Adobe Dynamic Media Classic. No se pueden generar direcciones URL de copia ni códigos incrustados para utilizarlos en reproductores de vídeo, sitios web, etc.

### Filtrar la lista de ajustes preestablecidos de codificación de vídeo {#filtering-the-list-of-video-encoding-presets}

Las páginas Ajustes preestablecidos de vídeo y Ajustes preestablecidos de vídeo adaptable constan de una tabla que enumera el estado activo, el nombre del ajuste preestablecido, el dispositivo de reproducción previsto, el tamaño del vídeo y la velocidad de datos de cada Ajuste preestablecido de vídeo.

Puede restringir la lista seleccionando filtrar por Activo, Inactivo o Ambos o reducir la lista a los que están activos o inactivos.

También puede filtrar en función de una opción de dispositivo de reproducción para reducir la lista a los ajustes preestablecidos de vídeo diseñados para reproducir vídeos en todos los dispositivos, escritorio, móviles o tablets.

**Para filtrar la lista de ajustes preestablecidos de codificación de vídeo:**

1. En Adobe Dynamic Media Classic, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]** > **[!UICONTROL Ajustes preestablecidos de vídeo adaptable]** o **[!UICONTROL Ajustes preestablecidos de codificación única]**.

   Las páginas para Ajustes preestablecidos de vídeo adaptable y Ajustes preestablecidos de codificación única incluyen una tabla que enumera el estado Activo, el nombre del Ajuste preestablecido, el dispositivo de reproducción previsto, las dimensiones de vídeo y la velocidad de datos de cada Ajuste preestablecido de vídeo.

1. En la página de ajustes preestablecidos de codificación única llamada Ajustes preestablecidos de vídeo, en la barra de herramientas de ajustes preestablecidos de vídeo, utilice las dos listas desplegables para restringir la lista de ajustes preestablecidos en la tabla según el estado activo y el dispositivo de reproducción.

   * En el primer campo, con una lista desplegable más estrecha, elija **[!UICONTROL Ambos]** para ver todos los ajustes preestablecidos de vídeo o elija **[!UICONTROL Activo]** o **[!UICONTROL Inactivo]** para reducir la lista a los que están activos o inactivos.
   * En la segunda lista desplegable, más amplia, elija una opción de dispositivo de reproducción para reducir la lista a los ajustes preestablecidos de vídeo diseñados para reproducir vídeos en equipos de escritorio o para reproducir vídeos en dispositivos móviles o tablets.

### Activar o desactivar ajustes preestablecidos de codificación de vídeo {#activating-or-deactivating-video-encoding-presets}

Los ajustes preestablecidos de vídeo activados aparecen en el cuadro de diálogo Opciones de trabajo de carga. El cuadro de diálogo aparece cuando un usuario carga archivos de vídeo durante el proceso de carga. Puede elegir de una lista de todos los ajustes preestablecidos de codificación activados.

1. En Adobe Dynamic Media Classic, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]**.
1. Realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Ajustes preestablecidos de vídeo adaptable]**.
   * Seleccionar **[!UICONTROL Ajustes preestablecidos de codificación única]**.

1. Realice una de las siguientes acciones:

   * Para activar un ajuste preestablecido de vídeo, en la página Ajustes preestablecidos, en la columna Activo, seleccione la casilla junto al nombre de un ajuste preestablecido.
   * Para desactivar un ajuste preestablecido de vídeo, anule la selección del cuadro situado junto al ajuste preestablecido de vídeo que quiera desactivar.

     >[!NOTE]
     >
     >Los ajustes preestablecidos de vídeo inactivos no aparecen en el cuadro de diálogo Opciones de trabajo de carga.

1. En la esquina inferior derecha de la página, seleccione **[!UICONTROL Cerrar]**.

### Agregar o editar un ajuste preestablecido de codificación de vídeo {#adding-or-editing-a-video-encoding-preset}

Puede crear sus propios ajustes preestablecidos de vídeo personalizados de codificación única y añadirlos a la tabla Ajustes preestablecidos de vídeo. También puede cambiar cualquier ajuste preestablecido de vídeo predefinido de codificación única que se haya incluido con Adobe Dynamic Media Classic, siempre que guarde el ajuste preestablecido editado con un nombre nuevo.

Adobe Dynamic Media Classic ha establecido límites máximos en la velocidad de datos de destino, la altura de la resolución y la anchura de la resolución para garantizar una experiencia de reproducción adecuada. Los mensajes de advertencia aparecen si se sobrepasan estos límites, que son los siguientes:

* Para la reproducción en equipo, los límites son: (Anchura/16) &#42; (Altura/16) &lt; 8192.
* Para la reproducción móvil, los límites son: (Anchura/16) &#42; (Altura/16) &lt; 660; velocidad de datos objetivo &lt; 4000.
* Para la reproducción en tablet, los límites son: (Anchura/16) &#42; (Altura/16) &lt; 3600.

**Para añadir o editar un ajuste preestablecido de codificación de vídeo:**

1. En Adobe Dynamic Media Classic, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]**.
1. Seleccionar **[!UICONTROL Ajustes preestablecidos de codificación única]**.
1. En la página Ajustes preestablecidos de vídeo, realice una de las acciones siguientes:

   * En la barra de herramientas Ajustes preestablecidos de vídeo, seleccione **[!UICONTROL Añadir]** para poder agregar un ajuste preestablecido de vídeo.
   * Seleccione un ajuste preestablecido de vídeo. En la barra de herramientas, seleccione **[!UICONTROL Editar]**.

     No puede editar ajustes predefinidos de Adobe Dynamic Media Classic; solo puede crear un ajuste preestablecido a partir de uno existente seleccionando **[!UICONTROL Guardar como]**.

1. En la página Agregar ajuste preestablecido de vídeo o la página Editar ajuste preestablecido de vídeo, establezca las opciones de ajustes preestablecidos de vídeo que desee.

   Consulte [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para ver la configuración recomendada.

   | Opción de ajuste preestablecido de vídeo | Descripción |
   | --- | --- |
   | Nombre de ajuste preestablecido | Asigne un nombre descriptivo al ajuste. Este nombre aparece en el cuadro de diálogo Opciones de trabajo de carga, en el que los usuarios seleccionan las opciones de transcodificación. |
   | Descripción | Describa el ajuste preestablecido de vídeo. Lo que escriba aparecerá como información de objeto. Cuando los usuarios eligen opciones de transcodificación, la información del objeto aparece cuando mueven el puntero sobre el nombre del ajuste preestablecido en el cuadro de diálogo Opciones de carga de trabajo. |
   | Dispositivo de reproducción | Seleccione el dispositivo en el que está previsto que se reproduzca el vídeo. Las opciones son Equipo (equipos de escritorio), Móvil (iPhone, iPad, Android™) o Tablet (solo iPad). Esta configuración determina automáticamente el códec de audio y vídeo adecuado que se utilizará durante la codificación. |
   | Velocidad de datos de destino | Introduzca la velocidad media de la conexión a Internet (en kilobits por segundo) del usuario final de destino. La velocidad se puede introducir manualmente o con el control deslizante. El espectro de velocidad de conexión del usuario muestra las velocidades típicas para ancho de banda, DSL, conexiones móviles y de marcación. Esta configuración determina automáticamente la velocidad de datos de audio y de vídeo combinada, Es decir, la cantidad de datos codificados para configurar un solo segundo de reproducción de vídeo. Cuanto mayor sea la velocidad de datos, mejor será la calidad del vídeo resultante. No obstante, las velocidades de datos demasiado altas producen tamaños de archivo grandes que crean visualizaciones no del todo satisfactorias por parte de los usuarios que tengan un ancho de banda menor. Como práctica recomendada, encuentre el equilibrio entre velocidades de datos altas y bajas. Intente crear una experiencia de reproducción de calidad adecuada sin enajenar a los usuarios con anchos de banda estrechos. |
   | Proporción de aspecto | La relación de aspecto es la relación entre la anchura y la altura del vídeo. Las dos primeras proporciones de aspecto enumeradas a continuación suelen utilizarse para mostrar vídeo horizontalmente:<ul><li> 4:3: Se utiliza en casi todo el contenido de emisiones de TV de definición estándar.</li><li>16:9: Se utiliza para casi todo el contenido de pantalla ancha y películas en televisión de alta definición (HDTV).</li><li>Escalado automático: (predeterminado) ajuste preestablecido de codificación única que funciona con cualquier relación de aspecto para crear vídeos para su envío a dispositivos móviles, tabletas y de escritorio. Los vídeos originales cargados que se hayan codificado con este ajuste preestablecido se definirán con una altura fija. Sin embargo, la anchura se amplía automáticamente para conservar la relación de aspecto del vídeo (relación de anchura y altura).</li><li>Personalizado: se utiliza cuando desea definir un tamaño de vídeo no estándar.</li><li>La proporción de aspecto que elija determina la anchura y la altura de la configuración de Tamaño de resolución; el valor de anchura y altura se adapta automáticamente a la proporción de aspecto adecuada.</li></ul> |
   | Tamaño de la resolución | El tamaño de la resolución, expresado por el número de píxeles de ancho por el número de píxeles de alto, determina el tamaño. Introduzca un valor de anchura y altura en píxeles o arrastre el control deslizante para introducir estos valores. El espectro de resolución muestra los tamaños de resolución típicos. El valor de anchura y el valor de altura se ajustan automáticamente a la relación de aspecto seleccionada. Por ejemplo, si selecciona 4:3 como proporción de aspecto e introduce 400 para anchura, se introduce 300 automáticamente para altura. Si ha seleccionado Escalar automáticamente para la configuración Proporción de aspecto, el valor Anchura para el Tamaño de resolución se establece automáticamente como Automático. Seleccionar **[!UICONTROL Previsualizar]** para que pueda abrir una ventana del explorador y ver las opciones de resolución allí. |
   | Codificar sufijo de archivo | Introduzca un sufijo. Este sufijo se añade al archivo de vídeo codificado resultante. Puede introducir un guión y un guión bajo en el nombre; los espacios en blanco y los caracteres especiales no están permitidos. |
   | Otros ajustes | Adobe Dynamic Media Classic determina automáticamente todos los demás ajustes de codificación según las directrices de codificación de prácticas recomendadas. |

1. Realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Guardar]** si ha añadido o editado un ajuste preestablecido de vídeo.
   * Seleccionar **[!UICONTROL Guardar como]** si ha añadido un ajuste preestablecido de vídeo a partir de un ajuste preestablecido existente.

### Eliminar un ajuste preestablecido de codificación de vídeo {#delete-a-video-encoding-preset}

Los administradores pueden eliminar ajustes preestablecidos de vídeo personalizados. Los ajustes preestablecidos de vídeo que se incluyen con Adobe Dynamic Media Classic no se pueden eliminar.

1. En Adobe Dynamic Media Classic, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de vídeo]**.
1. Seleccionar **[!UICONTROL Ajustes preestablecidos de codificación única]**.
1. En la página Ajustes preestablecidos de vídeo, seleccione un ajuste preestablecido de vídeo de la tabla que ya no desee o necesite.
1. En la barra de herramientas Ajustes preestablecidos de vídeo, seleccione **[!UICONTROL Eliminar]**.
1. En el cuadro de diálogo Eliminar ajuste preestablecido, seleccione **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Inicio rápido: Vídeo en Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Carga y codificación de vídeos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Trabajo con ajustes preestablecidos de visualizador de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [Ajustes preestablecidos de vídeo](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) vídeo de formación
