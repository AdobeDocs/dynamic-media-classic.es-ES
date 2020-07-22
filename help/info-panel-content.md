---
title: Administración del contenido del panel de información en catálogos electrónicos
seo-title: Administración del contenido del panel de información en catálogos electrónicos
description: nulo
seo-description: Aprenda a administrar el contenido del panel de información en los catálogos electrónicos.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 81%

---


# Administración del contenido del panel de información en catálogos electrónicos{#managing-info-panel-content-in-ecatalogs}

Además de utilizar el texto del mapa de imagen para sus rollover en los catálogos electrónicos, puede utilizar un panel de información para agregar grandes cantidades de texto rollover, incluyendo los vínculos. También puede gestionar el panel de información mediante el uso de almacenamiento en caché programado y actualizaciones de contenido planificadas.

Puede administrar la configuración y los datos del panel de información mediante las siguientes funciones de Dynamic Media Classic:

* El panel de configuración del panel de información le permite especificar la plantilla que desea usar para mostrar el texto del panel de información, una respuesta predeterminada para los errores y el número de horas del almacenamiento de la información en caché. Además, puede especificar si desea publicar automáticamente los catálogos electrónicos.
* La alimentación de datos del panel de información le permite especificar un archivo CSV que contenga el texto que desea que aparezca en el texto rollover del panel de información, así como programar los tiempos de actualización de la información.
* El cuadro de diálogo Importar metadatos (al que se accede a través de la vista Páginas de mapa) permite importar un archivo TXT delimitado por tabuladores con la información del texto rollover. Puede utilizar esta opción de TXT o el panel de alimentación de datos con la opción de archivo CSV para su texto rollover.
* La vista Páginas de mapa proporciona una opción para previsualizar el XML que aparece para los mapas de imagen específicos.

## Configuración de una plantilla de respuesta para catálogos electrónicos {#set-up-a-response-template-for-ecatalogs}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar el texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: el número de columnas y filas, el tamaño del tipo de letra, la fuente, etc. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

>[!NOTE]
>
>También puede configurar una plantilla de respuesta en Ajustes preestablecidos de visor. To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>Consulte [Configuración de ajustes preestablecidos del visor de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Haga doble clic en su catálogo electrónico para abrirlo en la vista de detalles.
1. Haga clic en el panel de configuración del panel de información para abrirlo.
1. Seleccione una plantilla de respuesta:

   * Seleccione un ajuste preestablecido en el menú de la plantilla de respuesta. El XML para el diseño de la plantilla aparece en el cuadro de plantilla de usuario.
   * Para crear su propia plantilla de respuesta, seleccione Personalizar. Escriba la definición de la plantilla XML en el cuadro de plantilla de usuario. Puede usar una plantilla preestablecida como base para la suya propia. 

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Dynamic Media Classic encuentra un error al recuperar la información de un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de catálogo electrónico, pero ningún identificador rollover, aparecerá este mensaje para el usuario.
1. En el cuadro de respuesta TTL, escriba el número de horas que desea esperar antes de almacenar los datos en caché:

   * Establezca un número más bajo si los datos se actualizan frecuentemente a lo largo del día.
   * Establezca un número más alto si los datos son relativamente estables y no requieren actualizarse con frecuencia a lo largo del día. El valor predeterminado es de diez horas.

1. Click **Publish**.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

Puede utilizar archivos de valores separados por comas (CSV) o archivos delimitados por tabuladores (TXT) para el texto de origen del panel de información de un catálogo electrónico. Los archivos delimitados por tabuladores deben usar la codificación UTF16 (Unicode). Puede importar los distintos tipos de archivos mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Asegúrese de que los archivos de datos delimitados por comas y tabuladores contienen tantas columnas como sean necesarias para la plantilla de rollover.
* Asegúrese de que el primer elemento o columna de datos es el identificador de rollover (asociado con el valor rollover_key de las URL de mapas de imagen).
* Asegúrese de que cada elemento delimitado por comas o tabuladores tras el identificador es el elemento que desea sustituir en la plantilla de respuesta (la primera columna se sustituye en $1$, la segunda columna en $2$, y así sucesivamente).

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Haga doble clic en el catálogo electrónico para abrirlo en la vista de detalles.
1. Haga clic en el panel de alimentación de datos del panel de información para abrirlo.
1. Introduzca la dirección URL para el archivo CSV en el cuadro Ubicación del archivo CSV alojado de forma externa. Puede pegar la URL en este campo o escribirla directamente.
1. (Opcional) Especifique un tiempo para la actualización del contenido mediante los menús Actualiz. de la progr. y haga clic en Agregar. Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro de tiempos de actualización. (Para eliminar un tiempo, selecciónelo y haga clic en Eliminar).
1. (Opcional) Haga clic en el botón de ejecución de la actualización para actualizar los contenidos inmediatamente.

### Importación de un archivo CSV o delimitado por tabuladores {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Haga doble clic en el catálogo electrónico para abrirlo en la vista de detalles.
1. Haga clic en el panel de configuración del panel de información para abrirlo.
1. **Haga clic en Cargar contenido** de S7Info.
1. Click **Browse**, select the tab-delimited TXT file, CSV or SSV file you want to use, and click **Open**.
1. Haga clic en **Cargar**.

Dynamic Media Classic le envía un mensaje de correo electrónico en el que se indica si la carga se ha realizado correctamente o no.

## Vista previa de texto de tecla rollover para un mapa de imagen {#preview-rollover-key-text-for-an-image-map}

Mediante la pantalla Páginas de mapa, puede ver de forma fácil y rápida el texto del panel de información para los mapas de imágenes en una página específica de su catálogo electrónico.

1. Haga clic en el botón de rollover Editar del catálogo.
1. Haga clic en Páginas de mapa.
1. En la parte superior de la tabla, en la parte derecha de la pantalla, elija Panel de información desde el menú Mostrar.

   El texto de clave de sustitución aparece al lado de cada Mapa de imágenes que contenga texto de Panel de información.

