---
title: Administración del contenido del panel de información en conjuntos de imágenes
description: Obtenga información sobre cómo administrar el contenido del panel de información en los conjuntos de imágenes en Adobe Dynamic Media Classic.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 45%

---

# Administración del contenido del panel de información en conjuntos de imágenes{#managing-info-panel-content-in-image-sets}

Además de utilizar el texto del mapa de imagen para sus rollover en los conjuntos de imágenes, puede utilizar un panel de información para agregar grandes cantidades de texto rollover, incluyendo los vínculos. También puede administrar el panel de información mediante el almacenamiento en caché de tiempo y la programación de actualizaciones de contenido.

Puede administrar la configuración y los datos de InfoPanel mediante las siguientes funciones de Adobe Dynamic Media Classic:

* El panel de configuración del panel de información le permite especificar la plantilla que desea usar para mostrar el texto del panel de información, una respuesta predeterminada para los errores y el número de horas del almacenamiento de la información en caché. Además, puede especificar si desea publicar automáticamente el conjunto de imágenes.
* El panel Fuente de datos de InfoPanel le permite especificar un archivo CSV que contiene el texto que desea que aparezca en el texto de rollover del panel de información y programar tiempos para actualizar la información.
* El cuadro de diálogo Importación de metadatos le permite importar un archivo TXT delimitado por tabuladores con la información del texto rollover. Puede utilizar esta opción TXT o el panel de fuente de datos del panel de información con la opción de archivo CSV para el texto de rollover.

## Configuración de una plantilla de respuesta para conjuntos de imágenes {#set-up-a-response-template-for-image-sets}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar el texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: el número de columnas y filas, el tamaño del tipo de letra, la fuente, etc. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

**Para configurar una plantilla de respuesta para conjuntos de imágenes:**

1. Haga doble clic en el conjunto de imágenes para que se abra en la Vista de detalles.
1. Seleccionar **[!UICONTROL Configuración de InfoPanel]**.
1. En la lista desplegable Plantilla de respuesta, realice una de las siguientes acciones:

   * Para utilizar la respuesta predeterminada, seleccione **[!UICONTROL Predeterminado]**. El XML para el diseño de la plantilla aparece atenuado en el cuadro de texto Plantilla del usuario.
   * Para crear su propia plantilla de respuesta, seleccione **[!UICONTROL Personalizado]**. En el cuadro de texto Plantilla del usuario, escriba la definición XML de la plantilla. Como base para su propia respuesta, puede utilizar la plantilla predeterminada que ya está definida en el cuadro de texto.

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de conjunto de imágenes, pero ningún identificador rollover, aparecerá este mensaje para el usuario.
1. En el campo de texto Tiempo de respuesta, escriba el número de horas que desea esperar antes de almacenar los datos en caché.

   * Establezca un número más bajo si los datos se actualizan frecuentemente a lo largo del día.
   * Establezca un número más alto si los datos son relativamente estables y no requieren actualizarse con frecuencia a lo largo del día. El valor predeterminado es de diez horas.

1. Seleccionar **[!UICONTROL Cargar]** para cargar contenido del panel de información en s7info en función del valor rollover_key.
1. En el cuadro de diálogo Cargar S7Info, busque el archivo que desea utilizar y, a continuación, seleccione **[!UICONTROL Cargar]**.

   Los formatos de archivo compatibles son archivos delimitados por tabuladores con codificación UTF-16 y archivos CSV con codificación ASCII. En el caso de los archivos CSV, los caracteres no ASCII deben estar codificados en HTML.

1. En el panel Configuración de InfoPanel, seleccione **[!UICONTROL Publish]**.

## Importar contenido de origen para el panel de información en conjuntos de imágenes {#import-source-content-for-the-info-panel-in-image-sets}

Puede utilizar un archivo CSV (Valor separado por comas) con codificación ASCII (los caracteres no ASCII deben estar codificados por el HTML) o un archivo delimitado por tabuladores para el texto de origen de un panel de información de un conjunto de imágenes. Los archivos delimitados por tabuladores deben usar la codificación UTF-16 (Unicode). Puede importar los distintos tipos de archivos mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Los datos delimitados por tabulaciones y comas pueden contener tantas columnas como sea necesario para la plantilla de rollover.
* El primer elemento o columna de datos es el identificador de rollover (asociado al valor rollover_key de las direcciones URL de mapa de imagen).
* Asegúrese de que cada elemento delimitado por tabulaciones o comas después del identificador sea el elemento que desee sustituir en la plantilla de respuesta. Por lo tanto, la primera columna se sustituye en $1$, la segunda columna en $2$, y así sucesivamente).

### Importación de contenido CSV en conjuntos de imágenes desde una ubicación alojada de forma externa {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Haga doble clic en el conjunto de imágenes para que se abra en Vista de detalles.
1. Seleccionar **[!UICONTROL Fuente de datos de InfoPanel]**.
1. En el campo de texto Ubicación del archivo CSV alojado de forma externa (HTTP), introduzca la URL del archivo CSV.
1. (Opcional) En el campo Programar actualización, especifique una hora para actualizar el contenido y, a continuación, seleccione **[!UICONTROL Añadir]**.

   Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro Tiempos de actualización. Para quitar una hora programada, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]**.

1. (Opcional) Seleccione **[!UICONTROL Ejecutar actualización]** para actualizar el contenido inmediatamente.
