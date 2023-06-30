---
title: Carga de los archivos del PDF
description: Obtenga información sobre cómo cargar los archivos de PDF asociados a un catálogo electrónico en Adobe Dynamic Media Classic.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 36%

---

# Carga de los archivos del PDF{#uploading-the-pdf-files}

Normalmente, los archivos Adobe PDF son el origen de un catálogo electrónico. Estos archivos contienen toda la información de la imagen, fuentes y gráficos vectoriales. También puede generar un catálogo electrónico a partir de imágenes. Después de preparar los archivos del PDF para la carga, en la barra de navegación global, seleccione **[!UICONTROL Cargar]** para empezar a cargar los PDF.

Al cargar un PDF para la extracción de páginas, el Adobe aplica el siguiente límite:

| tipo de límite de PDF | Límite impuesto | Cambio del límite el 31 de diciembre de 2022 |
| --- | --- | --- |
| Número máximo de páginas para que un PDF se considere para la extracción | 5000 (para nuevas cargas) | 100 (para todos los PDF) |

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

## Preparación de los archivos del PDF {#preparing-your-pdf-files}

Prepare los archivos del PDF antes de cargarlos en Adobe Dynamic Media Classic:

* Para facilitar la carga de los archivos, coloque todos los archivos en la misma carpeta del equipo o de la red.
* Asigne un nombre alfanumérico a los archivos para determinar el orden de las páginas. Si ordena las páginas, resultará más fácil colocarlas correctamente una vez se hayan cargado los archivos.
* Para ver si las páginas de PDF contienen marcas de recorte, destinos de registro o barras de color, examine las páginas. Estas marcas determinan dónde se corta el papel al imprimir; deben eliminarse antes de colocar el catálogo electrónico en la Web. Adobe Dynamic Media Classic proporciona opciones para marcas de recorte al cargar archivos de PDF.
* Si desea que los usuarios del catálogo electrónico tengan la posibilidad de realizar búsquedas por palabra clave dentro del mismo, averigüe si los archivos PDF están &quot;acoplados&quot;. Si los archivos PDF están acoplados, no se podrán extraer palabras de búsqueda. Para averiguar si un archivo PDF está acoplado, intente seleccionar texto dentro del mismo. Si no puede seleccionar texto, el PDF se acopla y los visualizadores no pueden buscar por palabra clave en el catálogo electrónico.
* Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. De forma predeterminada, Adobe Dynamic Media Classic puede detectar de forma inteligente estas imágenes CMYK y convertirlas con un perfil de color CMYK interno. Sin embargo, si desea usar un perfil de color personalizado para convertir imágenes CMYK, puede hacerlo.

  Consulte [Perfiles ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Prácticas recomendadas para cargar PDF {#best-practice-pdf-upload-options}

Para obtener información más detallada sobre los diferentes métodos de carga, consulte [Carga de archivos](uploading-files.md#uploading_your_files).

Seleccione los archivos que desea cargar y, a continuación, seleccione los siguientes *práctica recomendada* Opciones del PDF:

* **Opciones de recorte** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de recorte]**. Si las páginas de PDF contienen marcas de recorte, marcas de registro u otras marcas, en la variable **[!UICONTROL Recorte]** lista desplegable, elija **[!UICONTROL Manual]**. Elija el número de píxeles que desea recortar en la parte superior, derecha, inferior e izquierda de las páginas. Las marcas de recorte suelen tener un margen de media pulgada. Supongamos que elige **[!UICONTROL 150]** (recomendado) como resolución de píxel por pulgada y escriba 75, 75, 75, 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda. En tal caso, recorta media pulgada de los márgenes (a 150 ppp, la mitad de 1 equivale a 75 píxeles).

* **Procesando** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones del PDF]**. En el **[!UICONTROL Procesando]** lista desplegable, elija **[!UICONTROL Rasterizar]**. Para que todas las páginas y las imágenes se muestren en el catálogo electrónico, debe rasterizar el archivo PDF.

* **Extraer palabras de búsqueda (opcional)** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones del PDF]**. En la lista desplegable Extraer, elija **[!UICONTROL Palabras de búsqueda]** si desea que sus espectadores puedan buscar por palabra clave en su catálogo electrónico.

* **Generar catálogo electrónico automáticamente desde un PDF de varias páginas (opcional)** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones del PDF]**. Seleccionar **[!UICONTROL Generar catálogo electrónico automáticamente a partir de un PDF de varias páginas]** para crear automáticamente un catálogo electrónico al cargar. Puede ir directamente a la pantalla del catálogo electrónico y comenzar a trabajar en el catálogo electrónico sin necesidad de seleccionar primero los archivos PDF y el comando Generar. El catálogo electrónico recibe el mismo nombre que el archivo PDF.

* **Resolución** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones del PDF]**. En el **[!UICONTROL Resolución]** Campo de texto, introduzca un valor. Adobe Dynamic Media Classic recomienda 150 píxeles por pulgada.

* **Colorspace** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones del PDF]**. En la lista desplegable Espacio de color, elija **[!UICONTROL Detectar automáticamente]**. Los archivos PDF creados para imprimirse suelen estar en modo CMYK, mientras que los diseñados para visualizarse en línea están en modo RGB. Si un archivo PDF utiliza ambos espacios de color, puede seleccionar un espacio específico si elige Forzar RGB o Forzar CMYK. Los archivos PDF pueden utilizar ambos espacios de color, por ejemplo, cuando los gráficos utilizan un espacio de color CMYK pero las imágenes utilizan RGB. Si ha cargado un perfil ICC, su nombre aparecerá en el menú Espacio de color, desde donde lo podrá elegir.

  Consulte [Perfiles ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opciones de perfil de color** - En el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de perfil de color]** y, a continuación, elija una opción de Perfil de color:

   * **Mantener el espacio de color original** - Conserva el espacio de color original.

   * **Personalizar De > A** - Abre submenús para que pueda elegir una **[!UICONTROL Convertir de]** y **[!UICONTROL Convertir a]** espacio de color. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Consulte [Perfiles ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para ver los detalles de todas las opciones del PDF, consulte [Opciones de carga de PDF](pdfs.md#pdf_upload_options).
