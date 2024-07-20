---
title: Trabajo con archivos de PSD
description: Aprenda a trabajar con archivos de PSD en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 22%

---

# Trabajo con archivos de PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

Los PSD (archivos de documentos de Photoshop) se utilizan principalmente en Adobe Dynamic Media Classic para crear plantillas. Al cargar un archivo de PSD, puede crear una plantilla de Adobe Dynamic Media Classic automáticamente a partir del archivo (seleccione la opción Crear plantilla en la pantalla Cargar ).

Adobe Dynamic Media Classic crea varias imágenes a partir de un archivo de PSD con capas si utiliza el archivo para crear una plantilla; crea una imagen para cada capa.

## Opciones de carga de archivos PSD {#psd-upload-options}

Las opciones para cargar archivos de PSD se encuentran en Opciones de Photoshop, en el cuadro de diálogo Opciones del trabajo de carga. Puede recortar un archivo, elegir un perfil de color para el mismo, usarlo para crear una plantilla y seleccionar un anclaje.

Estas opciones están disponibles al cargar archivos PSD:

* **Opciones de recorte**: se encuentra en **[!UICONTROL Opciones de recorte]**. Seleccione **[!UICONTROL Recortar]** para que pueda recortar automáticamente el espacio en blanco de los bordes de un archivo de PSD. Seleccione **[!UICONTROL Manual]** para recortar los lados del archivo del PSD:

   * **[!UICONTROL Recortar]**: selecciona el menú **[!UICONTROL Recortar basándose en]** y elige **[!UICONTROL Color]** o **[!UICONTROL Transparencia]**.

  Si elige la opción **[!UICONTROL Color]**, seleccione el menú Esquina y elija la esquina del PSD con el color que mejor represente el color del espacio en blanco que desea recortar.

  Arrastre el control deslizante para especificar una tolerancia de 0 a 1. Para un recorte basado en color, especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PSD. Los números más cercanos a 1 permiten una mayor diferencia de color. Para recortar según la transparencia, especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

   * **[!UICONTROL Manual]**: Escriba el número de píxeles que desea recortar de cualquier lado o de cada lado de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, supongamos que la imagen muestra 150 ppp. A continuación, escriba 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda. Se recorta cada lado de la imagen, 0,5 pda.

* **Opciones de perfil de color**: se encuentra en **[!UICONTROL Opciones de perfil de color]**.

   * **[!UICONTROL Conservación de color predeterminada]**

   * **[!UICONTROL Conservar el espacio de color original]**: conserva el espacio de color original de la imagen.

   * **[!UICONTROL Personalizar desde]** > **[!UICONTROL hasta]**: abre menús para que pueda elegir un espacio de color Convertir desde y Convertir a. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic. Consulte [Perfiles ICC](/help/using/icc-profiles.md).

* **Opciones de Photoshop**

   * **[!UICONTROL Mantener capas]**: extrae las capas del PSD, si las hay, en recursos individuales. Las capas de recursos permanecen asociadas al PSD. Para verlos, abra el fichero PSD en Vista de detalles y seleccione el panel Capa. Consulte Visualización y edición de capas en un fichero de PSD.

   * **[!UICONTROL Crear plantilla]**: crea una plantilla a partir de las capas del archivo PSD.

   * **[!UICONTROL Extraer texto]**: extrae el texto para que los usuarios puedan buscar texto en un visor.

   * **[!UICONTROL Extender capas al tamaño del fondo]**: Extiende el tamaño de las capas de imagen copiada al tamaño de la capa de fondo.

   * **[!UICONTROL Nombres de capas]**: las capas del archivo del PSD se cargan como imágenes independientes. Para asignar un nombre a estas imágenes en Adobe Dynamic Media Classic, elija una de las siguientes opciones:

      * **[!UICONTROL Nombre de capa]**: asigna un nombre a las imágenes después de sus nombres de capa en el archivo PSD. Por ejemplo, una capa con el nombre Etiqueta de precio en el archivo PSD original se convierte en una imagen con el nombre Etiqueta de precio. Sin embargo, si los nombres de las capas del fichero de PSD son nombres de capas Photoshop por defecto (Fondo, Capa 1, Capa 2, etc.), las imágenes recibirán los nombres de sus números de capa en el fichero de PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop y número de capa]**: asigna un nombre a las imágenes después de sus números de capa en el archivo PSD, omitiendo los nombres de capa originales. Las imágenes reciben el nombre del archivo de Photoshop y un sufijo de número de capa. Por ejemplo, la segunda capa de un archivo denominado `Spring Ad.psd` se denomina `Spring Ad_2` aunque no tuviera un nombre predeterminado en Photoshop.

      * **[!UICONTROL Photoshop y nombre de capa]**: nombra las imágenes después del archivo de PSD seguido del nombre de capa o número de capa. El número de capa se utiliza si los nombres de capa en el archivo PSD son nombres de capa predeterminados de Photoshop. Por ejemplo, una capa denominada `Price Tag` en un archivo de PSD denominado `SpringAd` se denomina `Spring Ad_Price Tag`. Una capa con el nombre predeterminado Capa 2 se llama `Spring Ad_2`.

   * **[!UICONTROL Anclaje]**: especifique cómo se anclan las imágenes en las plantillas que se generan a partir de la composición con capas producida a partir del archivo PSD. De forma predeterminada, el anclaje es al centro. Un anclaje central permite imágenes de reemplazo que pueden rellenar mejor el mismo espacio, sin importar la proporción de aspecto de la imagen de reemplazo. Las imágenes con una proporción diferente que sustituyan esta imagen, al hacer referencia a la plantilla y usar la sustitución paramétrica, ocuparán el mismo espacio. Cambie a otra configuración si la aplicación requiere que las imágenes de sustitución rellenen el espacio asignado en la plantilla.

## Visualización y edición de capas en un archivo de PSD {#viewing-and-editing-layers-in-a-psd-file}

Si seleccionó la opción **[!UICONTROL Mantener capas]** al cargar el PSD, Adobe Dynamic Media Classic copió las capas individuales en los recursos. Puede ver y editar las capas de recursos que pertenecen a un archivo de PSD abriendo el archivo en el panel Examinar en la Vista de detalles.

>[!NOTE]
>
>Adobe Dynamic Media Classic admite hasta cinco niveles en un grupo de capas anidadas.

1. Haga doble clic en el archivo de PSD completo en el panel Examinar. El archivo se abre en la Vista de detalles.

   >[!NOTE]
   >
   >Asegúrese de abrir el recurso completo y no una de las capas del PSD.

1. Seleccionar **[!UICONTROL capas]**. Todas las capas aparecen como imágenes independientes en el panel Capas.
1. Haga doble clic en una capa y realice una de las acciones siguientes:

   * Para crear un mapa de imagen en la capa, seleccione el icono **[!UICONTROL Mapa de imagen]**. (Consulte [Crear mapas de imagen](creating-image-maps.md#creating_image_maps).)
   * Para crear destinos de zoom en la capa, seleccione el icono **[!UICONTROL destinos de zoom]**. (Consulte [Crear destinos de zoom para el zoom guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).
   * Para recortar la capa, seleccione el icono **[!UICONTROL Recortar]**. (Consulte [Recortar una imagen](cropping-image.md#cropping_an_image).)
   * Para enfocar la capa, seleccione **[!UICONTROL Enfoque]**. (Consulte [Enfoque de una imagen](sharpening-image.md#sharpening_an_image).)
   * Para ajustar la capa, seleccione **[!UICONTROL Ajustar]**. (Consulte [Ajustar una imagen](adjusting-image.md#adjusting_an_image).)

1. Seleccione **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como]**.
1. Para ver o editar una capa diferente, seleccione una flecha en la parte inferior de la vista previa de la capa.
1. Para salir de la vista de detalles de la capa, seleccione el icono **[!UICONTROL Vista de cuadrícula]**.
