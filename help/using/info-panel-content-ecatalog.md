---
title: Administración del contenido del panel de información en catálogos electrónicos
description: Obtenga información sobre cómo administrar el contenido del panel de información en catálogos electrónicos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T19:51:12.585Z'
TQID: 'https://experienceleague.adobe.com/KZEo-DNrfZJt66xzSAHpLX6A8j1evxOBtwSxQfk44Wc'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: a6556d91057da7b0cd02523a48f97e2eadcebb88
workflow-type: tm+mt
source-wordcount: 889
ht-degree: 26%

---

# Administración del contenido del panel de información en catálogos electrónicos{#managing-info-panel-content-in-ecatalogs}

Además de utilizar el texto del mapa de imagen para sus rollover en los catálogos electrónicos, puede utilizar un panel de información para agregar grandes cantidades de texto rollover, incluyendo los vínculos. También puede administrar el Panel de información mediante el almacenamiento en caché temporizado y la programación de actualizaciones de contenido.

Puede administrar la configuración y los datos del panel de información mediante las siguientes funciones de Adobe Dynamic Media Classic:

* El panel Configuración de InfoPanel le permite especificar la plantilla utilizada para mostrar el texto del Panel de información, una respuesta predeterminada para los errores y el número de horas que la información se almacena en caché. Además, puede especificar si los catálogos electrónicos se publican automáticamente.
* El panel Información Panel Fuente de datos permite especificar un archivo CSV. Este archivo contiene el texto que desea que aparezca en el texto de rollover del panel de información. También puede programar tiempos para actualizar la información.
* El cuadro de diálogo Importar metadatos (al que se accede desde la vista Páginas de mapa) permite importar un archivo TXT delimitado por tabuladores que contiene la información de texto de rollover. Puede utilizar esta opción TXT o el panel Fuente de datos con la opción de archivo CSV para el texto de rollover.
* La vista Páginas de mapas proporciona una opción para obtener una vista previa del XML que aparece para mapas de imágenes específicos.

## Configuración de una plantilla de respuesta para catálogos electrónicos {#set-up-a-response-template-for-ecatalogs}

Puede seleccionar una de las tres plantillas de respuesta preestablecidas para mostrar texto en un panel de información. Estas plantillas de respuesta preestablecidas determinan cómo se presenta la información en el panel de información: cuántas columnas y filas, tipo de letra, tamaño, fuente y otros ajustes. Puede seleccionar una plantilla de respuesta preestablecida o crear una propia.

>[!NOTE]
>
>También puede configurar una plantilla de respuesta en Ajustes preestablecidos de visor. Para usar la plantilla de respuesta en el ajuste preestablecido de visor, agregue `fmt=1` al final de la URL de servidor de información en el ajuste preestablecido de visor.
>
>Consulte [Configurar ajustes preestablecidos del visor de catálogos electrónicos](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Haga doble clic en el catálogo electrónico para que se abra en la Vista de detalles.
1. Seleccione el panel **[!UICONTROL Configuración de InfoPanel]**.
1. Seleccione una plantilla de respuesta:

   * Seleccione un ajuste preestablecido en el menú de la plantilla de respuesta. El XML para el diseño de la plantilla aparece en el cuadro de plantilla de usuario.
   * Para crear tu propia plantilla de respuesta, selecciona **[!UICONTROL Personalizado]**. Escriba la definición de la plantilla XML en el cuadro de plantilla de usuario. Puede utilizar las plantillas preestablecidas como punto de partida para las suyas propias.

1. (Opcional) En el cuadro Respuesta predeterminada, escriba el texto que desea que aparezca si Adobe Dynamic Media Classic encuentra un error al recuperar información para un mapa de imagen. Por ejemplo, si el sistema recibe un nombre de empresa y de catálogo electrónico pero no un identificador de rollover, este mensaje aparece para el usuario.
1. En el cuadro de respuesta TTL, escriba el número de horas que desea esperar antes de almacenar los datos en caché:

   * Establezca un número menor si los datos se actualizan con frecuencia durante el día.
   * Configure un número mayor si los datos son relativamente estables y no requieren actualizaciones frecuentes durante el día. El valor predeterminado es de diez horas.

1. Seleccione **[!UICONTROL Publicar]**.

## Importar contenido de origen para el panel de información en catálogos electrónicos {#import-source-content-for-the-info-panel-in-ecatalogs}

Puede utilizar archivos de valores separados por comas (CSV) o archivos delimitados por tabuladores (TXT) para el texto de origen del panel de información de un catálogo electrónico. Los archivos delimitados por tabuladores deben usar la codificación UTF16 (Unicode). Puede importar los distintos tipos de archivo mediante diferentes métodos.

Cuando dé formato al contenido de origen, tenga en cuenta las siguientes pautas:

* Asegúrese de que los archivos de datos delimitados por comas y tabuladores contienen tantas columnas como sean necesarias para la plantilla de rollover.
* Asegúrese de que el primer elemento o columna de datos sea el identificador de rollover (asociado al valor rollover_key de las direcciones URL del mapa de imagen).
* Asegúrese de que cada elemento delimitado por tabulaciones o comas después del identificador sea el elemento que desee sustituir en la plantilla de respuesta. Por lo tanto, la primera columna se sustituye en $1$, la segunda columna en $2$, etc.

### Importación de contenido CSV en catálogos electrónicos desde una ubicación alojada de forma externa {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Haga doble clic en el catálogo electrónico para que se abra en la Vista de detalles.
1. Seleccione el panel **[!UICONTROL Fuente de datos de InfoPanel]**.
1. Introduzca la dirección URL para el archivo CSV en el cuadro Ubicación del archivo CSV alojado de forma externa. Puede pegar la URL en este campo o escribirla directamente.
1. (Opcional) Especifique una hora para actualizar el contenido mediante el menú Programar actualización y seleccione **[!UICONTROL Agregar]**. Puede seleccionar varios tiempos de actualización. Cada tiempo de actualización aparece en el cuadro de tiempos de actualización. (Para quitar una hora, selecciónela y seleccione **[!UICONTROL Eliminar]**).
1. (Opcional) Seleccione **[!UICONTROL Ejecutar actualización ahora]** para que pueda actualizar inmediatamente el contenido.

### Importación de un archivo CSV o delimitado por tabuladores {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Haga doble clic en el catálogo electrónico para que se abra en la Vista de detalles.
1. Seleccione el panel **[!UICONTROL Configuración de InfoPanel]**.
1. Seleccione **[!UICONTROL Cargar contenido de S7Info]**.
1. Seleccione **[!UICONTROL Examinar]**, seleccione el archivo TXT, CSV o SSV delimitado por tabuladores que desee usar y seleccione **[!UICONTROL Abrir]**.
1. Seleccione **[!UICONTROL Cargar]**.

Adobe Dynamic Media Classic le envía un mensaje de correo electrónico para informarle de si la carga se ha realizado correctamente.

## Vista previa de texto de tecla rollover para un mapa de imagen {#preview-rollover-key-text-for-an-image-map}

Con la pantalla Páginas de mapa, puede ver el texto del panel de información de los mapas de imágenes en una página específica del catálogo electrónico.

1. Seleccione el botón de sustitución del catálogo **[!UICONTROL Editar]**.
1. Seleccione **[!UICONTROL Páginas de mapa]**.
1. En la parte superior de la tabla, en el lado derecho de la pantalla, elija **[!UICONTROL Panel de información]** en el menú Mostrar.

   El texto de tecla rollover aparece junto a cada mapa de imagen que contiene texto del panel de información.
