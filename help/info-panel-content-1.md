---
title: Gestión del contenido del panel de información en conjuntos de imágenes
seo-title: Gestión del contenido del panel de información en conjuntos de imágenes
description: nulo
seo-description: Descubra cómo administrar el contenido del panel de información en conjuntos de imágenes.
uuid: ed 7 b 4344-f 180-41 fc-a 95 a -62 a 9767 dc 056
contentOwner: rbrough
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
content-type: referencia
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sets
discoiquuid: ba 5 d 1 fb 1-af 54-471 c-a 471-853 ace 7 f 72 fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Gestión del contenido del panel de información en conjuntos de imágenes{#managing-info-panel-content-in-image-sets}

Además de utilizar el texto del mapa de imagen para sus rollover en los conjuntos de imágenes, puede utilizar un panel de información para agregar grandes cantidades de texto rollover, incluyendo los vínculos. También puede gestionar el panel de información mediante el uso de almacenamiento en caché programado y actualizaciones de contenido planificadas.

Puede gestionar la configuración y los datos de su panel de información mediante las siguientes características de Scene7 Publishing System:

* El panel de configuración del panel de información le permite especificar la plantilla que desea usar para mostrar el texto del panel de información, una respuesta predeterminada para los errores y el número de horas del almacenamiento de la información en caché. Además, puede especificar si desea publicar automáticamente el conjunto de imágenes.
* El panel Entrada de datos del panel de información le permite especificar un archivo CSV que contenga el texto que desea que aparezca en el texto rollover del panel de información, así como programar los tiempos de actualización de la información.
* El cuadro de diálogo Importación de metadatos le permite importar un archivo TXT delimitado por tabuladores con la información del texto rollover. Puede utilizar esta opción de TXT o el panel Entrada de datos del panel de información con la opción de archivo CSV para su texto rollover.

## Configuración de una plantilla de respuesta para conjuntos de imágenes {#set-up-a-response-template-for-image-sets}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar el texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: el número de columnas y filas, el tamaño del tipo de letra, la fuente, etc. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

**Para configurar una plantilla de respuesta**

1. Haga doble clic en el conjunto de imágenes para abrirlo en la vista de detalles.
1. Click **InfoPanel Setup** to unfold the panel.
1. En la lista desplegable Plantilla de respuesta, realice una de las siguientes acciones:

   * Seleccione Predeterminado para utilizar la respuesta predeterminada. El XML para el diseño de la plantilla aparece atenuado en el cuadro de texto Plantilla del usuario.
   * Para crear su propia plantilla de respuesta, seleccione Personalizar. En el cuadro de texto Plantilla del usuario, escriba la definición XML de la plantilla. Como base para su propia respuesta, puede utilizar la plantilla predeterminada que ya está definida en el cuadro de texto.

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Dynamic Media Classic encuentra un error al recuperar la información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de conjunto de imágenes, pero ningún identificador rollover, aparecerá este mensaje para el usuario.
1. En el campo de texto Tiempo de respuesta, escriba el número de horas que desea esperar antes de almacenar los datos en caché.

   * Establezca un número más bajo si los datos se actualizan frecuentemente a lo largo del día.
   * Establezca un número más alto si los datos son relativamente estables y no requieren actualizarse con frecuencia a lo largo del día. El valor predeterminado es de diez horas.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   Son compatibles los archivos delimitados por tabuladores con codificación UTF-16 y los archivos CSV con codificación ASCII. En el caso de los archivos CSV, los caracteres no ASCII deben estar codificados en HTML.

1. In the InfoPanel Setup panel, click **Publish**.

## Importación del contenido de origen para el panel de información en conjuntos de imágenes {#import-source-content-for-the-info-panel-in-image-sets}

Puede utilizar un archivo CSV (valores delimitados por comas) con codificación ASCII (los caracteres no ASCII deben tener codificación HTML) o un archivo delimitado por tabuladores para el texto de origen del panel de información de un conjunto de imágenes. Los archivos delimitados por tabuladores deben usar la codificación UTF-16 (Unicode). Puede importar los distintos tipos de archivos mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Los datos delimitados por tabuladores y comas deben contener tantas columnas como sea necesario para la plantilla rollover.
* El primer elemento o columna de datos debe ser el identificador de rollover (asociado con el valor rollover_key de las URL de mapas de imagen).
* Asegúrese de que cada elemento delimitado por comas o tabuladores tras el identificador es el elemento que desea sustituir en la plantilla de respuesta (la primera columna se sustituye en $1$, la segunda columna en $2$, y así sucesivamente).

### Importar contenido CSV en conjuntos de imágenes desde una ubicación alojada externamente {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Haga doble clic en el conjunto de imágenes para abrirlo en la vista de detalles.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. En el campo de texto Ubicación del archivo CSV alojado de forma externa (HTTP), introduzca la URL del archivo CSV.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro Tiempos de actualización. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

