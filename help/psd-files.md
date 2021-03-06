---
title: Trabajo con archivos PSD
description: Aprenda a trabajar con archivos PSD en Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 29%

---

# Trabajo con archivos PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

Los PSD (archivos de documento de Photoshop) se usan con mayor frecuencia en Adobe Dynamic Media Classic para crear plantillas. Al cargar un archivo PSD, puede crear una plantilla de Dynamic Media Classic de Adobe automáticamente desde el archivo (seleccione la opción Crear plantilla en la pantalla Cargar ).

Adobe Dynamic Media Classic crea varias imágenes de un archivo PSD con capas si utiliza el archivo para crear una plantilla; crea una imagen para cada capa.

## Opciones de carga de archivos PSD {#psd-upload-options}

Las opciones para cargar archivos PSD se encuentran en Opciones de Photoshop, en el cuadro de diálogo Opciones de carga de trabajo . Puede recortar un archivo, elegir un perfil de color para el mismo, usarlo para crear una plantilla y seleccionar un anclaje.

Estas opciones están disponibles al cargar archivos PSD:

* **Opciones de recorte** : se encuentra en Opciones de  **[!UICONTROL recorte]**. Seleccione **[!UICONTROL Recortar]** para recortar automáticamente el espacio en blanco de los bordes de un archivo PSD; seleccione **[!UICONTROL Manual]** para recortar los lados del archivo PSD:

   * **[!UICONTROL Recortar]** : seleccione el menú  **[!UICONTROL Recortar sin base]** y elija  **** Transparencia de  **[!UICONTROL color]**.

      Si elige la opción **[!UICONTROL Color]**, seleccione el menú Esquina y elija la esquina del PSD con el color que mejor represente el color del espacio en blanco que desea recortar.

      Arrastre el control deslizante para especificar una tolerancia de 0 a 1. Para un recorte basado en color, especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PSD. Los números más cercanos a 1 permiten una mayor diferencia de color. Para recortar en función de la transparencia, especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

   * **[!UICONTROL Manual]** : introduzca el número de píxeles que desea recortar de cualquier lado o de cada lado de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, si la imagen muestra 150 ppp y se introduce 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, se recortará media pulgada de cada lado de la imagen.

* **Opciones**  de perfil de color: se encuentra en Opciones de perfil de  **[!UICONTROL color]**.

   * **[!UICONTROL Conservación de color predeterminada]**

   * **[!UICONTROL Mantener espacio de color original]** : conserva el espacio de color original de la imagen.

   * **[!UICONTROL Personalizar de]**  >  **[!UICONTROL A]** : abre los menús para que pueda elegir un espacio de color Convertir de y Convertir en. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic. Consulte [Perfiles ICC](/help/icc-profiles.md).

* **Opciones de Photoshop**

   * **[!UICONTROL Mantener capas]** : permite extraer las capas del PSD, si las hay, en recursos individuales. Las capas de recursos permanecen asociadas al PSD. Puede verlos abriendo el archivo PSD en la Vista de detalles y seleccionando el panel de capa. Consulte Visualización y edición de capas de archivos PSD.

   * **[!UICONTROL Crear plantilla]** : crea una plantilla a partir de las capas del archivo PSD.

   * **[!UICONTROL Extraer texto]** : extrae el texto para que los usuarios puedan buscar texto en un visualizador.

   * **[!UICONTROL Ampliar capas a tamaño de fondo]** : amplía el tamaño de las capas de imagen arrancadas al tamaño de la capa de fondo.

   * **[!UICONTROL Nombre de capa]** : las capas del archivo PSD se cargan como imágenes independientes. Para asignar un nombre a estas imágenes en Adobe Dynamic Media Classic, elija entre las siguientes opciones:

      * **[!UICONTROL Nombre de capa]** : nombra las imágenes después de sus nombres de capa en el archivo PSD. Por ejemplo, una capa con el nombre Etiqueta de precio en el archivo PSD original se convierte en una imagen con el nombre Etiqueta de precio. Sin embargo, si los nombres de capa del archivo PSD son nombres de capa predeterminados de Photoshop (Fondo, Capa 1, Capa 2, etc.), las imágenes reciben el nombre de sus números de capa en el archivo PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop y número de capa]** : nombra las imágenes después de sus números de capa en el archivo PSD, ignorando los nombres de capa originales. Las imágenes reciben el nombre del archivo de Photoshop y un sufijo de número de capa. Por ejemplo, la segunda capa de un archivo llamado `Spring Ad.psd` se llama `Spring Ad_2` aunque tenga un nombre no predeterminado en Photoshop.

      * **[!UICONTROL Photoshop y nombre de capa]** : nombra las imágenes después del archivo PSD seguido del nombre de la capa o del número de capa. El número de capa se utiliza si los nombres de capa en el archivo PSD son nombres de capa predeterminados de Photoshop. Por ejemplo, una capa denominada `Price Tag` en un archivo PSD llamado `SpringAd` se denomina `Spring Ad_Price Tag`. Una capa con el nombre predeterminado Capa 2 se llama `Spring Ad_2`.
   * **[!UICONTROL Anclaje]** : especifique cómo se anclan las imágenes en plantillas generadas a partir de la composición en capas producida a partir del archivo PSD. De forma predeterminada, el anclaje es al centro. Un anclaje central permite la sustitución de imágenes para rellenar mejor el mismo espacio, independientemente de la proporción de la imagen de sustitución. Las imágenes con una proporción diferente que sustituyan esta imagen, al hacer referencia a la plantilla y usar la sustitución paramétrica, ocuparán el mismo espacio. Cambie a otra configuración si la aplicación requiere que las imágenes de sustitución rellenen el espacio asignado en la plantilla.


## Ver y editar capas en un archivo PSD {#viewing-and-editing-layers-in-a-psd-file}

Si seleccionó la opción Mantener capas al cargar el archivo PSD, Adobe Dynamic Media Classic dividió las capas individuales en recursos. Para ver y editar las capas de recursos que pertenecen a un archivo PSD, abra el archivo en el panel Examinar de la Vista de detalles.

1. Haga doble clic en el archivo PSD completo en el panel Examinar. El archivo se abre en la Vista de detalles.

   >[!NOTE]
   >
   >Asegúrese de abrir el recurso completo y no una de las capas del PSD.

1. Seleccione **[!UICONTROL Capas]**. Todas las capas aparecen como imágenes independientes en el panel Capas.
1. Haga doble clic en una capa y realice una de las siguientes acciones:

   * Para crear un mapa de imagen en la capa, seleccione el icono **[!UICONTROL Mapa de imagen]**. (Consulte [Crear mapas de imagen](creating-image-maps.md#creating_image_maps)).
   * Para crear destinos de zoom en la capa, seleccione el icono **[!UICONTROL Destinos de zoom]**. (Consulte [Crear destinos de zoom para zoom guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).
   * Para recortar la capa, seleccione el icono **[!UICONTROL Recortar]**. (Consulte [Recortar una imagen](cropping-image.md#cropping_an_image)).
   * Para enfocar la capa, seleccione **[!UICONTROL Enfocar]**. (Consulte [Perfilar una imagen](sharpening-image.md#sharpening_an_image)).
   * Para ajustar la capa, seleccione **[!UICONTROL Ajustar]**. (Consulte [Ajustar una imagen](adjusting-image.md#adjusting_an_image)).

1. Seleccione **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como]**.
1. Para ver o editar una capa diferente, seleccione una flecha en la parte inferior de la vista previa de la capa.
1. Para salir de la Vista de detalles de la capa, seleccione el icono **[!UICONTROL Vista de cuadrícula]**.
