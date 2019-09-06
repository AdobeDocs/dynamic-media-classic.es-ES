---
title: Carga y codificación de vídeo
seo-title: Carga y codificación de vídeo
description: Aprenda a cargar y codificar vídeos.
seo-description: Aprenda a cargar y codificar vídeos.
uuid: 9 a 7 d 6513-b 10 c -40 b 0-aebb -18 a 795 c 2 b 8 d 1
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: a 0941823-850 c -4373-9 e 37-f 32032 de 3805
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Carga y codificación de vídeo{#uploading-and-encoding-videos}

Para crear vídeo único o conjuntos de vídeos adaptables para publicarlos en la web o dispositivos móviles, primero cargue los archivos de vídeo maestros en Scene7 Publishing System. Dynamic Media Classic codifica vídeos en formato MP 4 y publica vídeo en los siguientes formatos de archivo:

**MP 4** Dynamic Media Classic recomienda MP 4 como el formato de archivo de vídeo preferido. Utilice archivos MP4 para lo siguiente:

* Flujo dinámico HTTP en equipos de escritorio.
* HTTP Live Streaming (protocolo de flujo de Apple).
* Publicación de vídeo progresivo en dispositivos móviles Android, BlackBerry y Windows Phone

Dynamic Media Classic ofrece dos flujos de trabajo para cargar archivos de vídeo:

**Vídeos precodificados** Cargue archivos MP 4 directamente en Dynamic Media Classic. Con este flujo de trabajo, los archivos no se codifican al cargarlos. Los archivos se codifican previamente como preparación para la publicación en el escritorio y los dispositivos móviles.

**Vídeos de origen maestros** Cargue archivos de origen maestros de origen y, al cargarlos, codifíquelos a archivos MP 4. Los vídeos codificados tienen la etiqueta “Vídeo” en el panel Examinar. Dynamic Media Classic admite la codificación de archivos de vídeo en varios formatos.

* Asegúrese de que los archivos de vídeo de origen maestros que desea codificar sean compatibles. 

   Consulte [Tipos de archivos de vídeo compatibles para la codificación](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

* Elija un ajuste preestablecido de codificación de vídeo.

   Consulte [Ajustes preestablecidos de vídeo para la codificación de archivos de vídeo](application-setup.md#video-presets-for-encoding-video-files)

   Consulte [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding).

Dynamic Media Classic también genera miniaturas de vídeo. Puede obtener más información sobre las miniaturas de vídeo, la obtención de sus URL y la modificación de fotogramas de póster.

Consulte [Uso de las miniaturas de vídeo](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Para cargar y codificar vídeos**

Realice una de las siguientes acciones:

*Si los vídeos ya están codificados*

1. En la barra de navegación global, haga clic en **Cargar**.
1. En la pantalla **Cargar**, haga clic en la ficha Desde el escritorio.
1. On the Upload page, in the Select Files for Upload panel, click **Browse**, navigate to an MP4 video file, and then click **Open**.
1. En el panel Elija el destino de la carpeta, elija una carpeta para cargar el archivo.
1. En la página de carga, asegúrese de que esté activado **Publicar tras la carga**.
1. Haga clic en **Cargar envío**.

*Si desea codificar los vídeos mediante Scene7 Publishing System*

1. En la barra de navegación global, haga clic en **Cargar**.
1. En la pantalla **Cargar**, haga clic en la ficha Desde el escritorio.
1. En el panel Seleccionar archivos para cargar, haga clic en **Examinar**, busque un archivo de vídeo de origen maestro y haga clic en **Abrir**.
1. En el panel Elija el destino de la carpeta, elija una carpeta para cargar el archivo.
1. En la esquina inferior derecha de la página, haga clic en **Opc. de trabajo**.
1. En el cuadro de diálogo Opciones de trabajo de carga, amplíe Opciones de eVideo.
   * Realice una de las siguientes acciones:
      * La práctica recomendada es utilizar el método siguiente.
Seleccione **Codificación de vídeo adaptable**.
Consulte [Vídeo adaptable (predeterminado)](application-setup.md#adaptive-video-default).
   * (Opcional) Si desea utilizar ajustes de codificación individuales, haga lo siguiente.
Amplíe **Ajustes preestablecidos de codificación única** y seleccione las opciones de codificación que desee para Escritorio, Móvil y Tablet.
Consulte [Ajustes preestablecidos de codificación de vídeo para equipos de escritorio](application-setup.md#desktop-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para dispositivos móviles](application-setup.md#mobile-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para tablets](application-setup.md#tablet-video-encoding-presets).
1. En el cuadro de diálogo Opciones de trabajo de carga, haga clic en **Guardar**.
1. En la página de carga, asegúrese de que esté activado **Publicar tras la carga**.
1. En la página de carga, en la esquina inferior derecha, haga clic en **Cargar envío**.

Si desea volver a codificar a un archivo de vídeo cargado anteriormente

1. En Dynamic Media Classic, en el panel Examinar, vaya al vídeo y selecciónelo.
1. Haga clic en **Archivo** &gt; **Procesar de nuevo**.
1. En el cuadro de diálogo Volver a procesar los recursos, expanda Opciones de eVideo.
1. Realice una de las siguientes acciones:
   * La práctica recomendada es utilizar el método siguiente.
Seleccione **Vídeo adaptable**.
Consulte [Vídeo adaptable (predeterminado)](application-setup.md#adaptive-video-default).
   * (Opcional) Si desea utilizar ajustes de codificación individuales, haga lo siguiente.
Amplíe **Ajustes preestablecidos de codificación única** y seleccione las opciones de codificación que desee para Escritorio, Móvil y Tablet.
Consulte [Ajustes preestablecidos de codificación de vídeo para equipos de escritorio](application-setup.md#desktop-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para dispositivos móviles](application-setup.md#mobile-video-encoding-presets), [Ajustes preestablecidos de codificación de vídeo para tablets](application-setup.md#tablet-video-encoding-presets).
1. En el cuadro de diálogo Volver a procesar los recursos, haga clic en **Enviar**.

Cuando se utiliza un ajuste preestablecido de codificación de vídeo adaptable o varios ajustes preestablecidos de codificación individuales, el resultado es un conjunto de vídeos adaptables que se crea automáticamente con varias codificaciones de vídeo. También puede crear manualmente un conjunto de vídeos adaptables seleccionando los vídeos individuales.

Cuando se genera un conjunto de vídeos adaptables automáticamente o manualmente, solo se crean tipos de archivo MP4 y M4V.

## Tipos de archivo de vídeo compatibles para la codificación {#supported-video-file-types-for-encoding}

En la siguiente tabla se muestran los tipos de archivo de vídeo (con los códecs de vídeo permitidos) que puede codificar al formato MP4 u OGV al cargar los archivos. En la tabla se muestran los formatos de archivo y códecs:

**Formatos de archivo de vídeo** similar a un archivo ZIP, un formato de archivo de vídeo determina cómo se encuentran los archivos en el archivo de vídeo. Un archivo de vídeo suele contener varias pistas, una pista de vídeo (sin audio) y una o más pistas de audio (sin vídeo), que están interrelacionadas y sincronizadas. El formato de archivo de vídeo determina cómo se organizan estas distintas pistas de datos y metadatos.

**Códecs de vídeo** Un códec de vídeo describe el algoritmo por el que se codifica un vídeo. Un reproductor de vídeo descodifica el vídeo según su códec y, a continuación, reproduce una serie de imágenes, o fotogramas, en la pantalla. Los códecs minimizan la cantidad de información que tienen que almacenar los archivos de vídeo para reproducir el vídeo. En lugar de la información sobre cada fotograma individual, solo se almacena la información sobre las diferencias entre un fotograma y el siguiente. Puesto que la mayoría de vídeos cambian poco de un fotograma al siguiente, los códecs permiten velocidades de compresión altas, cuyo resultado son tamaños de archivo menores.

| Formato de archivo de vídeo | Códecs de vídeo |
|:--- |:--- |
| 3GP | H.263, H.264 |
| AVI | DivX, DV |
| M2P | MPEG-2 PS |
| M2T | MPEG-2 TS |
| M2TS | MPEG-2 TS |
| M2V | MPEG-2 ES |
| M4V | H.264  |
| MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
| MP4 | H.264/MPEG-4 AVC |
| MPEG | MPEG-2 SS |
| MPG | MPEG-2 SS |
| MTS | MPEG-2 |
| ProRes | APCN, APCS, APCO, APCH, AP4H |
| TS | DVCPro 50 |
| VOB | MPEG-2 |
| WMV/ASF | VC-1, Windows Media Video 7, Windows Media Video 8 |

>[!NOTE]
>
>La pantalla Trabajos le avisa si carga e intenta codificar un archivo de vídeo pero este se rechaza porque contiene un códec o contenedor de archivos no compatible. Para obtener más información, consulte [Comprobación de archivos de trabajo](checking-job-files.md).

## Prácticas recomendadas para la codificación de vídeo {#best-practices-for-video-encoding}

A continuación se detallan prácticas recomendadas para codificar archivos de vídeo de origen en Scene7 Publishing System.

Para obtener más consejos sobre la codificación de vídeo, consulte los siguientes recursos:

* Article: *Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution: * [www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en).
* Vídeo: * Conceptos básicos de codificación de vídeo: * [www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en).

### Archivos de vídeo de origen {#source-video-files}

Al codificar un archivo de vídeo, utilice el archivo de vídeo de origen de la máxima calidad posible. Evite utilizar archivos de vídeo codificados previamente, ya que estos archivos ya están comprimidos y una codificación adicional crearía un vídeo de mala calidad.

La siguiente tabla describe el tamaño recomendado, la proporción de aspecto y la velocidad de bits mínima que deben tener los archivos de vídeo de origen cuando se codifiquen:

| Tamaño | Proporción de aspecto | Velocidad de bits mínima |
|--- |--- |--- |
| 1024 X 768 | 4:3 | 4500 Kbps para la mayoría de vídeos. |
| 1280 X 720 | 16:9 | 3000 - 6000 kbps, dependiendo de la cantidad de movimiento del vídeo. |
| 1920 X 1080 | 16:9 | 6000 - 8000 kbps, dependiendo de la cantidad de movimiento del vídeo. |

### Obtención de los metadatos de un archivo {#obtaining-a-file-s-metadata}

Puede obtener los metadatos de un archivo consultando sus metadatos en Dynamic Media Classic, utilizando una herramienta de edición de vídeo o utilizando una aplicación diseñada para obtener metadatos. A continuación se muestran instrucciones para el uso de MediaInfo, una aplicación de terceros, para obtener los metadatos de un archivo de vídeo:

1. Go to this web page: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Seleccione y descargue el instalador para la versión de interfaz gráfica de usuario y siga las instrucciones de instalación.
1. Después de la instalación, haga clic con el botón derecho en el archivo de vídeo (solo Windows) y seleccione MediaInfo o abra MediaInfo y arrastre el archivo de vídeo a la aplicación. Se ven todos los metadatos asociados al archivo de vídeo, incluida su anchura, su altura y los fotogramas por segundo.

### Proporción de aspecto {#aspect-ratio}

Al elegir o crear un ajuste preestablecido de codificación de vídeo para el archivo de vídeo principal, asegúrese de que dicho ajuste tenga la misma proporción de aspecto que el archivo de vídeo principal. La *proporción de aspecto* es la proporción de anchura y altura del vídeo.

Para determinar la proporción de aspecto de un archivo de vídeo, obtenga los metadatos del archivo y tenga en cuenta la anchura y la altura del archivo (consulte [Obtención de los metadatos de un archivo](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). A continuación, utilice esta fórmula para determinar la proporción de aspecto:

anchura/altura = proporción de aspecto

En la tabla siguiente se describe cómo se traducen los resultados de la fórmula en opciones comunes de proporción de aspecto:

| Resultado de la fórmula | Proporción de aspecto |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Por ejemplo, un vídeo con una anchura de 1440 y una altura de 1080 tiene una proporción de aspecto de 1440/1080 o 1,33. En este caso, debe elegir un ajuste preestablecido de codificación de vídeo con una proporción de aspecto 4:3 para codificar el archivo de vídeo.

### Velocidad de datos {#data-rate}

The *data rate* (also called the* bit rate*) is the amount of data that is encoded to make up a single second of video playback. La velocidad de datos se mide en kilobits por segundo (kbps).

>[!NOTE]
>
>debido a que todos los códecs utilizan la compresión con pérdida, la velocidad de datos es el factor más importante en lo que respecta a la calidad de vídeo. En la compresión con pérdida, cuanto más se comprima un archivo de vídeo, más se degrada la calidad. Por este motivo, si se mantienen las demás características (la resolución, la velocidad de fotogramas y el códec), cuanto menor sea la velocidad de los datos, menor será la calidad del archivo comprimido.

Al elegir un ajuste preestablecido de codificación de vídeo, tenga en cuenta la velocidad de conexión del usuario final al que va destinado. Elija un ajuste que tenga una velocidad de datos del 80 por ciento de dicha velocidad. Por ejemplo, si la velocidad de conexión del usuario final al que va destinado es de 1000 kbps, el mejor ajuste preestablecido es aquel que tiene una velocidad de datos de vídeo de 800 kbps.

En esta tabla se describe la velocidad de datos de las velocidades de conexión habituales.

| Velocidad (kbps) | Tipo de conexión |
|--- |--- |
| 256 | Conexión de marcación. |
| 800 | Conexión móvil habitual. Para esta conexión, utilice una velocidad de datos en el rango de 400 a 800 para experiencias 3G. |
| 2000 | Conexión de escritorio de ancho de banda habitual. Para esta conexión, defina una velocidad de datos en el rango de 800 a 2000 kbps, con la mayoría de objetivos promedios entre 1200 y 1500 kbps. |
| 5000 | Conexión de gran ancho de banda habitual. La codificación en este rango superior no se recomienda, porque la mayoría de los usuarios no pueden recibir el vídeo a esta velocidad. |

### Resolución {#resolution}

Con *resolución* se describe la altura y la anchura de un vídeo en píxeles. La mayoría de vídeos de origen se almacenan con una resolución alta (por ejemplo, 1920 x 1080). Para el flujo continuo, el vídeo de origen se comprime con una resolución menor (640 x 480 o inferior).

La resolución y la velocidad de datos son dos factores totalmente vinculados que determinan la calidad de vídeo. Para mantener la misma calidad de vídeo, cuanto mayor sea el número de píxeles de un archivo de vídeo (cuanto mayor sea la resolución), mayor será la velocidad de datos. Por ejemplo, observe el número de píxeles por fotograma en un archivo de vídeo con una resolución de 320 x 240 y de 640 x 480:

| Resolución | Píxeles por fotograma |
|--- |--- |
| 320 x 240 | 76.800 |
| 640 x 480 | 307.200 |

El archivo con resolución 640 x 480 tiene cuatro veces más píxeles por fotograma. Para lograr la misma velocidad de datos para estas dos resoluciones de ejemplo, tiene que aplicar cuatro veces la compresión al archivo de 640 x 480, lo que puede reducir la calidad del vídeo. Por lo tanto, una velocidad de datos de vídeo de 250 Kbps produce una visualización de alta calidad con una resolución de 320 x 240, pero no con una resolución de 640 x 480.

>[!NOTE]
>
>Por lo general, cuanto mayor sea la velocidad de datos que utilice, mejor será el aspecto del vídeo; por otra parte, cuanto mayor sea la resolución que use, mayor velocidad de datos necesitará para mantener la calidad de visualización (en comparación con resoluciones inferiores).

Debido a que la resolución y la velocidad de datos están vinculadas, al codificar el vídeo dispone de dos opciones:

* Elegir una velocidad de datos y, a continuación, codificar a la máxima resolución que permita una visualización aceptable con la velocidad de datos elegida.
* Elegir una resolución y, a continuación, codificar con la velocidad de datos necesaria para lograr un vídeo de gran calidad a la resolución elegida.

Cuando elija (o cree) un ajuste preestablecido de codificación de vídeo para el archivo de vídeo principal, utilice esta tabla para conseguir la resolución correcta:

| Resolución | Altura (píxeles) | Tamaño de la pantalla |
|--- |--- |--- |
| 240p | 240 | Pantalla muy pequeña |
| 300p | 300 | Pantalla pequeña habitual de los dispositivos móviles |
| 360p | 360 | Pantalla pequeña |
| 480p | 480 | Pantalla intermedia |
| 720p | 720 | Pantalla grande |
| 1080p | 1080 | Pantalla grande de alta definición |

### Fotogramas por segundo (fps) {#fps-frames-per-second}

En Estados Unidos y Japón, la mayoría de los vídeos se graban a 29,97 fotogramas por segundo (fps); en Europa, la mayoría se graba a 25 fps. Las películas se graban a 24 fps.

Elija un ajuste preestablecido de codificación de vídeo que coincida con la velocidad de fps del archivo de vídeo principal. Por ejemplo, si el vídeo principal tiene una resolución de 25 fps, elija un ajuste preestablecido de codificación de 25 fps. De manera predeterminada, toda la codificación personalizada utiliza el valor de fps del archivo de vídeo principal. Por este motivo, no es necesario que especifique explícitamente el ajuste de fps al crear un ajuste preestablecido de codificación de vídeo.

### Dimensiones de codificación de vídeo {#video-encoding-dimensions}

Para obtener resultados óptimos, seleccione unas dimensiones de codificación de forma que el vídeo de origen sea un múltiplo entero de todos los vídeos codificados.

Para calcular esta proporción, divida la anchura del archivo de origen entre la anchura del archivo codificado. Seguidamente, divida la altura del archivo de origen entre la altura del archivo codificado para obtener la proporción de altura.

Si la proporción resultante es un número entero, el vídeo tendrá una escala óptima. Si la proporción resultante no es un número entero, la calidad del vídeo se verá afectada por defectos de píxeles en la pantalla. Este efecto resulta más evidente cuando el vídeo tiene texto.

Como ejemplo, suponga que el vídeo de origen es de 1920 x 1080. En la tabla siguiente, los tres vídeos codificados ofrecen los ajustes de codificación óptimos que deben utilizarse.

| Tipo de vídeo | Anchura x altura | Proporción de anchura | Proporción de altura |
|--- |--- |--- |--- |
| Origen | 1920 x 1080 | 1 | 1 |
| Codificado | 960 x 540 | 2 | 2 |
| Codificado | 640 x 360 | 3 | 3 |
| Codificado | 480 x 270 | 4 | 4 |

### Formato de archivo de vídeo codificado {#encoded-video-file-format}

Adobe Dynamic Media Classic recomienda utilizar ajustes preestablecidos de codificación de vídeo MP 4 H .264. Dado que los archivos MP4 usan el códec de vídeo H.264, proporcionan vídeo de alta calidad pero con un tamaño de archivo comprimido.

## Uso de ajustes preestablecidos de codificación de vídeo {#working-with-video-encoding-presets}

Los archivos de vídeo principales creados con un equipo de producción de vídeo y software de edición de vídeo suelen ser demasiado grandes y no tienen el formato correcto para la publicación en destinos en línea. Para convertir vídeo digital al formato y especificaciones correctos para la reproducción en distintas pantallas, puede *transcodificar* archivos de vídeo (un proceso que también se denomina *codificación*). Durante el proceso de codificación, el vídeo se comprime a un tamaño de archivo eficaz más pequeño, óptimo para la publicación en la web y en dispositivos móviles.

Consulte [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading-and-encoding-videos).

Dynamic Media Classic proporciona una biblioteca de ajustes preestablecidos de codificación de vídeo predefinidos que reflejan los ajustes de codificación más comunes. Estos ajustes preestablecidos de codificación se han optimizado para la reproducción en pantallas de destino. Además, los administradores pueden crear sus propios ajustes preestablecidos de codificación de vídeo para personalizar el tamaño y la calidad de reproducción de vídeos para los usuarios finales. Todos los ajustes preestablecidos de codificación de vídeo, ya sean listos para usar desde Dynamic Media Classic o personalizados, generan vídeo en formato de archivo MP 4.

En la pantalla Ajustes preestablecidos de vídeo, los administradores pueden configurar y administrar la codificación de vídeo. Pueden hacer lo siguiente:

* Activar y desactivar ajustes preestablecidos de codificación de vídeo.
* Crear un ajuste preestablecido de codificación de vídeo.
* Editar ajustes preestablecidos de codificación de vídeo.
* Eliminar ajustes preestablecidos de vídeo.

Cualquier vídeo cargado o codificado en Scene7 Publishing System se trata como “vídeo”. Es decir, con esta clasificación de los recursos, podrá publicar el vídeo para reproducirlo en equipos de escritorio, dispositivos móviles, o ambos. Por ejemplo, puede obtener una vista previa de estos tipos de vídeos en Scene7 Publishing System. También puede generar direcciones URL (con la función de Copiar URL) y código que puede incrustar (con la función de Código incrustado) para su uso con los reproductores de vídeo, en sitios web, etc.

Consulte [Previsualización de vídeos en un visor de vídeos](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Consulte [Vinculación de una URL de vídeo a sitios web o de dispositivos móviles](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Consulte [Incrustación del visor de vídeo en páginas web](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Para los recursos de vídeo que cargue y codifique en Scene 7 Publishing System, el vídeo se enviará en el siguiente formato de archivo:

**MP 4 H .264** Utilice archivos MP 4 para lo siguiente:

* Flujo dinámico HTTP en equipos de escritorio.
* HLS (HTTP Live Streaming, protocolo de flujo de Apple).
* Publicación de vídeo progresivo en dispositivos móviles Android, BlackBerry y Windows Phone.

Cualquier otro códec y formato de vídeo se tratará como «Vídeo principal». Esta clasificación de los recursos implica que el vídeo es un archivo de origen y no se puede utilizar para su reproducción en escritorios ni dispositivos móviles. Por ejemplo, no puede obtener una vista previa de estos tipos de vídeos en Scene7 Publishing System. Tampoco puede generar las opciones Copiar URL ni Código incrustado para su uso en los reproductores de vídeo, en los sitios web, etc.

### Filtrado de la lista de ajustes preestablecidos de codificación de vídeo {#filtering-the-list-of-video-encoding-presets}

La página Ajustes preestablecidos de vídeo y la página Ajustes preestablecidos de vídeos adaptables constan de una tabla que enumera el estado activo, el nombre del ajuste preestablecido, el dispositivo de reproducción, el tamaño del vídeo y la velocidad de datos de destino de cada ajuste preestablecido de vídeo.

Puede restringir la lista seleccionando filtrar por Activo, Inactivo o Ambos o reducir la lista a los que están activos o inactivos.

También puede filtrar en función de una opción de dispositivo de reproducción para reducir la lista a los ajustes preestablecidos de vídeo diseñados para reproducir vídeos en todos los dispositivos, escritorio, móviles o tablets.

**Para filtrar la lista de ajustes preestablecidos de codificación de vídeo**

1. In Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Video Presets** &gt; **Adaptive Video Presets** or **Single Encoding Presets**.

   Las páginas para los ajustes preestablecidos de vídeos adaptables y ajustes preestablecidos de codificación única incluyen una tabla que enumera el estado activo, el nombre de ajuste preestablecido, el dispositivo de reproducción, tamaño del vídeo, y la velocidad de datos de destino de cada ajuste preestablecido de vídeo.

1. En la página de ajustes preestablecidos de codificación única llamada Ajustes preestablecidos de vídeo, en la barra de herramientas de ajustes preestablecidos de vídeo, utilice las dos listas desplegables para restringir la lista de ajustes preestablecidos en la tabla según el estado activo y el dispositivo de reproducción.

   * En el primer campo, con una lista desplegable más estrecha, elija **Ambos** para ver todos los ajustes preestablecidos de vídeo o elija **Activo** o **Inactivo** para reducir la lista a los que están activos o inactivos.
   * En la segunda lista desplegable, más amplia, elija una opción de dispositivo de reproducción para reducir la lista a los ajustes preestablecidos de vídeo diseñados para reproducir vídeos en equipos de escritorio o para reproducir vídeos en dispositivos móviles o tablets.

### Activación o desactivación de ajustes preestablecidos de codificación de vídeo {#activating-or-deactivating-video-encoding-presets}

Los ajustes preestablecidos de vídeo activados aparecen en el cuadro de diálogo Opciones de trabajo de carga. Se trata del cuadro de diálogo que aparece cuando un usuario carga archivos de vídeo durante el proceso de carga. Puede elegir de una lista de todos los ajustes preestablecidos de codificación activados.

**Para activar o desactivar ajustes preestablecidos de codificación de vídeo**

1. En Dynamic Media Classic, haga clic **en Ajustes** &gt; Ajustes **de aplicación** &gt; Ajustes preestablecidos **de vídeo**.
1. Realice una de las siguientes acciones:

   * Haga clic en **Ajustes preestablecidos de vídeo adaptables**.
   * Haga clic en **Ajustes preestablecidos de codificación única**.

1. Realice una de las siguientes acciones:

   * Para activar un ajuste preestablecido de vídeo, en la columna Activo de la página de ajustes preestablecidos, seleccione la casilla junto a un nombre de ajuste preestablecido.
   * Para desactivar un ajuste preestablecido de vídeo, desactive la casilla junto a los que desea hacer inactivos.

      ***note**: Inactive Video Presets do not appear in the Upload Job Options dialog box. *

1. En la esquina inferior derecha de la página, haga clic en **Cerrar**.

### Adición o edición de un ajuste preestablecido de codificación de vídeo {#adding-or-editing-a-video-encoding-preset}

Puede crear sus propios ajustes preestablecidos de codificación única personalizados y añadirlos a la tabla Ajustes preestablecidos de vídeo. También puede realizar cambios en cualquier ajuste preestablecido de codificación única predefinido que venga con Dynamic Media Classic, siempre y cuando guarde el ajuste preestablecido modificado con un nombre nuevo.

Dynamic Media Classic tiene límites máximos para la velocidad de datos de destino, la altura de resolución y la anchura de resolución para garantizar una reproducción adecuada. Aparecerán mensajes de advertencia si se exceden los límites siguientes:

* Para la reproducción en ordenadores, los límites son: (anchura/16) * (altura/16) &lt; 8192. 
* Para la reproducción en móviles, los límites son: (anchura/16) * (altura/16) &lt; 660; velocidad de datos de destino &lt; 4000. 
* Para la reproducción en tablet, los límites son: (anchura/16) * (altura/16) &lt; 3600.

**Para añadir o editar un ajuste preestablecido de codificación de vídeo**

1. En Dynamic Media Classic, haga clic **en Ajustes** &gt; Ajustes **de aplicación** &gt; Ajustes preestablecidos **de vídeo**.
1. Haga clic en **Ajustes preestablecidos de codificación única** para abrir la página Ajustes preestablecidos de vídeo.
1. En la página Ajustes preestablecidos de vídeo, realice una de las acciones siguientes:

   * En la barra de herramientas de Ajustes preestablecidos de vídeo, haga clic en **Agregar** para agregar un nuevo ajuste preestablecido de vídeo.
   * Seleccione un ajuste preestablecido de vídeo. En la barra de herramientas, haga clic en **Editar**.

      You cannot edit Dynamic Media Classic predefined presets; you can only create a preset from an existing one by choosing **Save As**.

1. En la página Agregar ajuste preestablecido de vídeo o la página Editar ajuste preestablecido de vídeo, establezca las opciones de ajustes preestablecidos de vídeo que desee.

   Consulte [Prácticas recomendadas para la codificación de vídeo](uploading-encoding-videos.md#best-practices-for-video-encoding) para ver la configuración recomendada.

   | Opción de ajuste preestablecido de vídeo | Descripción |
   |--- |--- |
   | Nombre de ajuste preestablecido | Asigne un nombre descriptivo al ajuste. Este nombre aparece en el cuadro de diálogo Opciones de trabajo de carga, en el que los usuarios seleccionan las opciones de transcodificación. |
   | Descripción | Describa el ajuste preestablecido de vídeo. Lo que introduzca aparecerá como información de objeto al mover el puntero sobre el nombre del ajuste preestablecido en el cuadro de diálogo Opciones de trabajo de carga en el que los usuarios seleccionan las opciones de transcodificación. |
   | Dispositivo de reproducción | Seleccione el dispositivo en el que está previsto que se reproduzca el vídeo. Las opciones son Equipo (escritorios), Móvil (iphone, ipad, Android); o Tablet (solo ipad). Esta configuración determina automáticamente el códec de audio y vídeo adecuado utilizado durante la codificación. |
   | Velocidad de datos de destino | Introduzca la velocidad media de la conexión a Internet (en kilobits por segundo) del usuario final de destino. La velocidad se puede introducir manualmente o con el control deslizante. El espectro de velocidad de conexión del usuario muestra las velocidades típicas para ancho de banda, DSL, conexiones móviles y de marcación. Esta configuración determina automáticamente la velocidad de datos de audio y de vídeo combinada, Es decir, la cantidad de datos codificados para configurar un solo segundo de reproducción de vídeo. Cuanto mayor sea la velocidad de datos, mejor será la calidad del vídeo resultante. No obstante, las velocidades de datos demasiado altas producen tamaños de archivo grandes que crean visualizaciones no del todo satisfactorias por parte de los usuarios que tengan un ancho de banda menor. Como práctica recomendada, encuentre el equilibrio entre velocidades de datos altas y bajas. Intente crear una reproducción con una calidad adecuada sin perjudicar a los usuarios que tienen anchos de banda bajos. |
   | Proporción de aspecto | La proporción de aspecto es la relación de anchura y altura del vídeo. Las dos primeras proporciones de aspecto enumeradas a continuación suelen utilizarse para mostrar vídeo horizontalmente:<ul><li> 4:3, utilizado para casi todos los contenidos emitidos en la televisión estándar.</li><li>16:9, utilizado para casi todas las películas y contenido de TV de alta definición para pantalla panorámica.</li><li>Escala automática: (predeterminado) un ajuste preestablecido de codificación que funciona con cualquier proporción de aspecto para crear vídeos para su distribución en teléfonos móviles, tablets y equipos de escritorio. Los vídeos originales cargados que se hayan codificado con este ajuste preestablecido se definirán con una altura fija. Sin embargo, la anchura se escala automáticamente para mantener la proporción de aspecto del vídeo (proporción de anchura a altura).</li><li>Personalizado: se utiliza para definir un tamaño de vídeo no estándar.</li><li>La relación de aspecto que elija determinará la configuración de anchura y altura del tamaño de la resolución; los valores de anchura y altura se escalarán automáticamente a la relación de aspecto adecuada.</li></ul> |
   | Tamaño de la resolución | El tamaño de la resolución, expresado mediante el número de anchura de píxeles por el número de altura de píxeles, determina la dimensión. Introduzca los valores de anchura y altura en píxeles o sírvase del control deslizante. El espectro de resolución muestra los tamaños de resolución típicos. Los valores de anchura y altura se adherirán automáticamente a la relación de aspecto seleccionada. Por ejemplo, si selecciona 4:3 como proporción de aspecto e introduce 400 para la anchura, 300 se introduce automáticamente para la altura. Si ha seleccionado Escala automática para el ajuste Proporción de aspecto, el valor de Anchura para el tamaño de la resolución se establece automáticamente en Automático. Haga clic en Vista previa para abrir una ventana del explorador y ver las opciones de resolución allí. |
   | Codificar sufijo de archivo | Introduzca un sufijo. Este sufijo se añade al archivo de vídeo codificado resultante. Puede introducir un guión y un guión bajo en el nombre; los espacios en blanco y los caracteres especiales no están permitidos. |
   | Otros ajustes | Dynamic Media Classic determina todos los demás ajustes de codificación automáticamente según las directrices de codificación recomendadas. |

1. Realice una de las siguientes acciones:

   * Haga clic en **Guardar** si ha agregado o editado un ajuste preestablecido de vídeo.
   * Haga clic en **Guardar como** si ha agregado un ajuste preestablecido de vídeo a partir de uno existente.

### Eliminación de un ajuste preestablecido de codificación de vídeo. {#deleting-a-video-encoding-preset}

Los administradores pueden eliminar ajustes preestablecidos de vídeo personalizados. Los ajustes preestablecidos de vídeo que vienen con Dynamic Media Classic no se pueden eliminar.

**Para eliminar un ajuste preestablecido de codificación de vídeo**

1. En Dynamic Media Classic, haga clic **en Ajustes** &gt; Ajustes **de aplicación** &gt; Ajustes preestablecidos **de vídeo**.
1. Haga clic en **Ajustes preestablecidos de codificación única** para abrir la página Ajustes preestablecidos de vídeo.
1. En la página Ajustes preestablecidos de vídeo, seleccione un ajuste preestablecido de vídeo de la tabla que ya no desee o necesite.
1. En la barra de herramientas de ajustes preestablecidos de vídeo, haga clic en **Eliminar**.
1. En el cuadro de diálogo Eliminar ajuste preestablecido, haga clic en **Eliminar**.

>[!MORELIKETHIS]
>
>* [Inicio rápido: Vídeo](quick-start-video.md#quick-start-video)
>* [Carga y codificación de vídeo](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Uso de ajustes preestablecidos de visor de vídeo](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
