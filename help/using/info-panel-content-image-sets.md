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
autotag-review: '2026-05-13T20:01:44.270Z'
TQID: 'https://experienceleague.adobe.com/kYn0xood-R05EoIVrWA7w89rJm3qpqzdxPbmz563WJ0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 596e4337002ebd67dd9f915a5ae63ae2a6e18437
workflow-type: tm+mt
source-wordcount: 796
ht-degree: 28%

---

# Administración del contenido del panel de información en conjuntos de imágenes{#managing-info-panel-content-in-image-sets}

Además de utilizar texto de mapa de imagen para los rollovers en conjuntos de imágenes, puede utilizar un panel de información para añadir grandes cantidades de texto de rollover, incluidos vínculos. También puede administrar el Panel de información mediante el almacenamiento en caché de tiempo y la programación de actualizaciones de contenido.

Puede administrar la configuración y los datos de InfoPanel mediante las siguientes funciones de Adobe Dynamic Media Classic:

* El panel Configuración del panel de información le permite especificar la plantilla utilizada para mostrar el texto del panel de información, una respuesta predeterminada para los errores y el número de horas que la información se almacena en caché. Además, puede especificar si desea publicar automáticamente el conjunto de imágenes.
* El panel Información Panel Fuente de datos permite especificar un archivo CSV. Este archivo contiene el texto que desea que aparezca en el texto de rollover del panel de información. También puede programar tiempos para actualizar la información.
* El cuadro de diálogo Importar metadatos le permite importar un archivo TXT delimitado por tabuladores que contiene la información de texto de rollover. Puede utilizar esta opción TXT o el panel de fuente de datos del panel de información con la opción de archivo CSV para el texto de rollover.

## Configuración de una plantilla de respuesta para conjuntos de imágenes {#set-up-a-response-template-for-image-sets}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar el texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: el número de columnas y filas, el tamaño del tipo de letra, la fuente, etc. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

**Para configurar una plantilla de respuesta para conjuntos de imágenes:**

1. Haga doble clic en el conjunto de imágenes para que se abra en la Vista de detalles.
1. Seleccione **[!UICONTROL Configuración de InfoPanel]**.
1. En la lista desplegable Plantilla de respuesta, realice una de las siguientes acciones:

   * Para usar la respuesta predeterminada, seleccione **[!UICONTROL Predeterminado]**. El XML para el diseño de la plantilla aparece atenuado en el cuadro de texto Plantilla del usuario.
   * Para crear tu propia plantilla de respuesta, selecciona **[!UICONTROL Personalizado]**. En el cuadro de texto Plantilla del usuario, escriba la definición XML de la plantilla. Puede utilizar la plantilla predeterminada que ya está definida en el cuadro de texto como base para su propia respuesta.

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y un nombre de conjunto de imágenes pero carece de un identificador de rollover, este mensaje aparece para el usuario.
1. En el campo de texto Tiempo de respuesta, escriba el número de horas que desea esperar antes de almacenar los datos en caché.

   * Establezca un número más bajo si los datos se actualizan frecuentemente a lo largo del día.
   * Establezca un número más alto si los datos son relativamente estables y no requieren actualizarse con frecuencia a lo largo del día. El valor predeterminado es de diez horas.

1. Seleccione **[!UICONTROL Upload]** para cargar el contenido del panel de información a s7info, según el valor rollover_key.
1. En el cuadro de diálogo Cargar S7Info, busque el archivo que desee usar y, a continuación, seleccione **[!UICONTROL Cargar]**.

   Los formatos de archivo compatibles son archivos delimitados por tabuladores con codificación UTF-16 y archivos CSV con codificación ASCII. En el caso de los archivos CSV, los caracteres no ASCII deben estar codificados en HTML.

1. En el panel Configuración de InfoPanel, seleccione **[!UICONTROL Publicar]**.

## Importar contenido de origen para el panel de información en conjuntos de imágenes {#import-source-content-for-the-info-panel-in-image-sets}

Puede utilizar un archivo CSV (Valor separado por comas) con codificación ASCII (los caracteres no ASCII deben estar codificados en HTML) o un archivo delimitado por tabuladores para el texto de origen de un panel de información de un conjunto de imágenes. Los archivos delimitados por tabuladores deben usar la codificación UTF-16 (Unicode). Puede importar los distintos tipos de archivo mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Los datos delimitados por tabulaciones y comas pueden contener tantas columnas como sea necesario para la plantilla de rollover.
* El primer elemento o columna de datos es el identificador de rollover (asociado al valor rollover_key de las direcciones URL del mapa de imagen).
* Asegúrese de que cada elemento delimitado por tabulaciones o comas después del identificador sea el elemento que desee sustituir en la plantilla de respuesta. Por lo tanto, la primera columna se sustituye en $1$, la segunda columna en $2$, etc.

### Importación de contenido CSV en conjuntos de imágenes desde una ubicación alojada de forma externa {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Haga doble clic en el conjunto de imágenes para que se abra en Vista de detalles.
1. Seleccione **[!UICONTROL Fuente de datos de InfoPanel]**.
1. En el campo de texto Ubicación del archivo CSV alojado de forma externa (HTTP), introduzca la URL del archivo CSV.
1. (Opcional) En el campo Programar actualización, especifique una hora para actualizar el contenido y, a continuación, seleccione **[!UICONTROL Agregar]**.

   Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro Tiempos de actualización. Para quitar una hora programada, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]**.

1. (Opcional) Seleccione **[!UICONTROL Ejecutar actualización]** para que pueda actualizar inmediatamente el contenido.
