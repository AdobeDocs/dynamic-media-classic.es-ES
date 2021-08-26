---
title: Carga de archivos PDF
description: Aprenda a cargar los archivos PDF asociados a un catálogo electrónico.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 44%

---

# Carga de archivos PDF{#uploading-the-pdf-files}

Normalmente, los archivos Adobe PDF son la fuente de un catálogo electrónico. Estos archivos contienen toda la información de la imagen, las fuentes y los gráficos vectoriales. También puede generar un catálogo electrónico a partir de imágenes. Después de preparar los archivos PDF para su carga, en la barra de navegación global, haga clic en **[!UICONTROL Cargar]** para comenzar a cargar los archivos PDF.

## Preparación de los archivos PDF {#preparing-your-pdf-files}

Prepare sus archivos PDF antes de cargarlos en Adobe Dynamic Media Classic:

* Para que la carga de los archivos sea más sencilla, coloque todos los archivos en la misma carpeta del equipo o de la red.
* Asigne un nombre alfanumérico a los archivos para determinar el orden de las páginas. Si ordena las páginas, resultará más fácil colocarlas correctamente una vez se hayan cargado los archivos.
* Para ver si las páginas PDF contienen marcas de recorte, destinos de registro o barras de color, examine las páginas. Estas marcas determinan dónde se corta el papel al imprimir; deben eliminarse antes de colocar el catálogo electrónico en la Web. Adobe Dynamic Media Classic proporciona opciones para recortar marcas al cargar archivos PDF.
* Si desea que los usuarios del catálogo electrónico tengan la posibilidad de realizar búsquedas por palabra clave dentro del mismo, averigüe si los archivos PDF están &quot;acoplados&quot;. Si los archivos PDF están acoplados, no se podrán extraer palabras de búsqueda. Para averiguar si un archivo PDF está acoplado, intente seleccionar texto dentro del mismo. Si no puede seleccionar texto, el PDF se acopla y los visualizadores no pueden buscar por palabra clave en el catálogo electrónico.
* Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. De forma predeterminada, Adobe Dynamic Media Classic puede detectar de forma inteligente estas imágenes CMYK y convertirlas mediante un perfil de color CMYK interno. Sin embargo, si desea usar un perfil de color personalizado para convertir imágenes CMYK, puede hacerlo.

   Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Prácticas recomendadas para cargar PDF {#best-practice-pdf-upload-options}

Para obtener información más detallada sobre los diferentes métodos de carga, consulte [Carga de archivos](uploading-files.md#uploading_your_files).

Elija los archivos que desea cargar y seleccione estas opciones de PDF *recomendadas*:

* **Opciones de recorte** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en  **[!UICONTROL Opciones de recorte]**. Si las páginas PDF contienen marcas de recorte, marcas de registro u otras marcas, en la lista desplegable **[!UICONTROL Recortar]**, elija **[!UICONTROL Manual]**. Elija el número de píxeles que desea recortar en la parte superior, derecha, inferior e izquierda de las páginas. Las marcas de recorte suelen establecerse en un margen de media pulgada. Supongamos que elige **[!UICONTROL 150]** (recomendado) como resolución de píxeles por pulgada e introduce 75, 75, 75, 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda. En tal caso, recorta media pulgada de los márgenes (a 150 ppi, la mitad de 1 equivale a 75 píxeles).

* **Procesamiento** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de  **[!UICONTROL PDF]**. En la lista desplegable **[!UICONTROL Processing]**, elija **[!UICONTROL Rasterizar]**. Para que todas las páginas y las imágenes se muestren en el catálogo electrónico, debe rasterizar el archivo PDF.

* **Extraer palabras de búsqueda (opcional)** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de  **[!UICONTROL PDF]**. En la lista desplegable Extraer , elija **[!UICONTROL Palabras de búsqueda]** si desea que los visualizadores puedan buscar por palabra clave en el catálogo electrónico.

* **Generar catálogo electrónico automáticamente desde PDF de varias páginas (opcional)** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de  **[!UICONTROL PDF]**. Seleccione **[!UICONTROL Generación automática de catálogos electrónicos desde varias páginas PDF]** para crear automáticamente un catálogo electrónico al cargar. Puede ir directamente a la pantalla del catálogo electrónico y comenzar a trabajar en el catálogo electrónico sin necesidad de seleccionar primero los archivos PDF y el comando Generar. El catálogo electrónico recibe el mismo nombre que el archivo PDF.

* **Solución** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de  **[!UICONTROL PDF]**. En el campo de texto **[!UICONTROL Resolution]**, introduzca un valor. Adobe Dynamic Media Classic recomienda 150 píxeles por pulgada.

* **Espacio de color** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de  **[!UICONTROL PDF]**. En la lista desplegable Espacio de color, elija **[!UICONTROL Detectar automáticamente]**. Los archivos PDF creados para imprimirse suelen estar en modo CMYK, mientras que los diseñados para visualizarse en línea están en modo RGB. Si un archivo PDF utiliza ambos espacios de color, puede seleccionar un espacio específico si elige Forzar RGB o Forzar CMYK. Los archivos PDF pueden utilizar ambos espacios de color, por ejemplo, cuando los gráficos utilizan un espacio de color CMYK pero las imágenes utilizan RGB. Si ha cargado un perfil ICC, su nombre aparecerá en el menú Espacio de color, desde donde lo podrá elegir.

   Consulte [Perfiles ICC](/help/icc-profiles.md).

* **Opciones de perfil de color** : en el cuadro de diálogo Opciones de carga de trabajo, haga clic en Opciones de perfil de  **[!UICONTROL color]** y, a continuación, elija una opción de perfil de color:

   * **Mantener espacio de color original** : conserva el espacio de color original.

   * **Personalizar de > A** : abre submenús para que pueda elegir un espacio  **[!UICONTROL Convertir]** de y  **[!UICONTROL Convertir]** color de color. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para ver los detalles de todas las opciones del PDF, consulte [Opciones de carga de PDF](pdfs.md#pdf_upload_options).
