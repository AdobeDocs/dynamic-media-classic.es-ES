---
title: Administrar contenido del panel de información en conjuntos de imágenes
description: Obtenga información sobre cómo administrar el contenido del panel de información en conjuntos de imágenes en Dynamic Media Classic.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: bb387446f294cf1e90d26ae1df4422879ad29db7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 51%

---

# Administrar contenido del panel de información en conjuntos de imágenes{#managing-info-panel-content-in-image-sets}

Además de utilizar el texto del mapa de imagen para sus rollover en los conjuntos de imágenes, puede utilizar un panel de información para agregar grandes cantidades de texto rollover, incluyendo los vínculos. También puede gestionar el panel de información mediante el uso de almacenamiento en caché programado y actualizaciones de contenido planificadas.

Puede administrar la configuración y los datos del panel de información mediante las siguientes funciones en Dynamic Media Classic:

* El panel de configuración del panel de información le permite especificar la plantilla que desea usar para mostrar el texto del panel de información, una respuesta predeterminada para los errores y el número de horas del almacenamiento de la información en caché. Además, puede especificar si desea publicar automáticamente el conjunto de imágenes.
* El panel de fuente de datos del panel de información le permite especificar un archivo CSV que contenga el texto que desea que aparezca en el texto de sustitución del panel de información y programar tiempos para actualizar la información.
* El cuadro de diálogo Importación de metadatos le permite importar un archivo TXT delimitado por tabuladores con la información del texto rollover. Puede utilizar esta opción TXT o el panel de fuente de datos del panel de información con la opción de archivo CSV para el texto de sustitución.

## Configuración de una plantilla de respuesta para conjuntos de imágenes {#set-up-a-response-template-for-image-sets}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar el texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: el número de columnas y filas, el tamaño del tipo de letra, la fuente, etc. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

**Para configurar una plantilla de respuesta para los conjuntos de imágenes:**

1. Haga doble clic en el conjunto de imágenes para que se abra en la vista de detalles.
1. Seleccione **[!UICONTROL InfoPanel Setup]**.
1. En la lista desplegable Plantilla de respuesta, realice una de las siguientes acciones:

   * Para utilizar la respuesta predeterminada, seleccione **[!UICONTROL Default]**. El XML para el diseño de la plantilla aparece atenuado en el cuadro de texto Plantilla del usuario.
   * Para crear su propia plantilla de respuesta, seleccione **[!UICONTROL Personalizado]**. En el cuadro de texto Plantilla del usuario, escriba la definición XML de la plantilla. Como base para su propia respuesta, puede utilizar la plantilla predeterminada que ya está definida en el cuadro de texto.

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de conjunto de imágenes, pero ningún identificador rollover, aparecerá este mensaje para el usuario.
1. En el campo de texto Tiempo de respuesta, escriba el número de horas que desea esperar antes de almacenar los datos en caché.

   * Establezca un número más bajo si los datos se actualizan frecuentemente a lo largo del día.
   * Establezca un número más alto si los datos son relativamente estables y no requieren actualizarse con frecuencia a lo largo del día. El valor predeterminado es de diez horas.

1. Seleccione **[!UICONTROL Upload]** para cargar el contenido del panel de información, en función de los valores rollover_key, a s7info.
1. En el cuadro de diálogo Carga de S7Info, busque el archivo que desea utilizar y, a continuación, seleccione **[!UICONTROL Cargar]**.

   Los formatos de archivo admitidos son archivos delimitados por tabuladores con codificación UTF-16 y archivos CSV con codificación ASCII. En el caso de los archivos CSV, los caracteres no ASCII deben estar codificados en HTML.

1. En el panel Configuración del panel de información, seleccione **[!UICONTROL Publicar]**.

## Importación de contenido de origen para el panel Información en conjuntos de imágenes {#import-source-content-for-the-info-panel-in-image-sets}

Puede utilizar un archivo CSV (valores delimitados por comas) con codificación ASCII (los caracteres no ASCII deben tener codificación HTML) o un archivo delimitado por tabuladores para el texto de origen del panel de información de un conjunto de imágenes. Los archivos delimitados por tabuladores deben usar la codificación UTF-16 (Unicode). Puede importar los distintos tipos de archivos mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Los datos delimitados por tabuladores y comas pueden contener tantas columnas como sean necesarias para la plantilla de sustitución.
* El primer elemento o columna de datos es el identificador de sustitución (asociado con el valor rollover_key de las URL de mapa de imagen).
* Asegúrese de que cada elemento delimitado por tabulaciones o comas después del identificador sea el elemento que desea sustituir en la plantilla de respuesta. Por lo tanto, la primera columna se sustituye por $1$, la segunda columna por $2$, y así sucesivamente).

### Importar contenido CSV en conjuntos de imágenes desde una ubicación alojada de forma externa {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Haga doble clic en el conjunto de imágenes para que se abra en la vista de detalles.
1. Seleccione **[!UICONTROL InfoPanel Datafeed]**.
1. En el campo de texto Ubicación del archivo CSV alojado de forma externa (HTTP), introduzca la URL del archivo CSV.
1. (Opcional) En los campos Programar actualización , especifique una hora para actualizar el contenido y, a continuación, seleccione **[!UICONTROL Agregar]**.

   Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro Tiempos de actualización. Para quitar una hora programada, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]**.

1. (Opcional) Seleccione **[!UICONTROL Ejecutar actualización]** para actualizar el contenido inmediatamente.
