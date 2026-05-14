---
title: Carga de los archivos de PDF
description: Obtenga información sobre cómo cargar los archivos de PDF asociados a un catálogo electrónico en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:17:17.647Z'
TQID: 'https://experienceleague.adobe.com/SNoRYiCgjJK2TBx6X7HAzv3Xqet64-lm4oSOcat7DfM'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 858
ht-degree: 29%

---

# Carga de los archivos de PDF{#uploading-the-pdf-files}

Normalmente, los archivos Adobe PDF son el origen de un catálogo electrónico. Estos archivos contienen toda la información de la imagen, fuentes y gráficos vectoriales. También puede generar un catálogo electrónico a partir de imágenes. Una vez que haya preparado los archivos PDF para cargarlos, en la barra de navegación global, seleccione **[!UICONTROL Cargar]** para comenzar a cargar los archivos PDF.

Al cargar un PDF para la extracción de páginas, Adobe aplica el siguiente límite:

| Tipo de límite de PDF | Límite impuesto | Cambio del límite el 31 de diciembre de 2022 |
| --- | --- | --- |
| Número máximo de páginas de un PDF que se deben tener en cuenta para la extracción | 5000 (para nuevas cargas) | 100 (para todos los PDF) |

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

## Preparación de los archivos de PDF

Prepare los archivos de PDF antes de cargarlos en Adobe Dynamic Media Classic:

* Para facilitar la carga de los archivos, coloque todos los archivos en la misma carpeta del equipo o de la red.
* Asigne un nombre alfanumérico a los archivos para determinar el orden de las páginas. Si ordena las páginas, resultará más fácil colocarlas correctamente una vez se hayan cargado los archivos.
* Para ver si las páginas de PDF contienen marcas de recorte, destinos de registro o barras de color, examine las páginas. Estas marcas determinan dónde se corta el papel al imprimir; deben eliminarse antes de colocar el catálogo electrónico en la Web. Adobe Dynamic Media Classic proporciona opciones para marcas de recorte al cargar archivos PDF.
* Si desea que los visualizadores busquen en el catálogo electrónico por palabra clave, averigüe si los archivos PDF están &quot;aplanados&quot;. Si los archivos PDF están acoplados, no se podrán extraer palabras de búsqueda. Para averiguar si una PDF está aplanada, intente seleccionar el texto que contiene. Si no puede seleccionar texto, PDF se acopla y los visualizadores no pueden buscar por palabra clave en el catálogo electrónico.
* Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. De forma predeterminada, Adobe Dynamic Media Classic puede detectar de forma inteligente estas imágenes CMYK y convertirlas con un perfil de color CMYK interno. Sin embargo, si desea usar un perfil de color personalizado para convertir imágenes CMYK, puede hacerlo.

  Ver [perfiles ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

## Prácticas recomendadas para cargar PDF {#best-practice-pdf-upload-options}

Para obtener información más detallada sobre los diferentes métodos de carga, consulte [Carga de archivos](uploading-files.md#uploading_your_files).

Seleccione los archivos que desea cargar y, a continuación, seleccione estas *prácticas recomendadas* Opciones de PDF:

* **Opciones de recorte**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de recorte]**. Si las páginas de PDF contienen marcas de recorte, marcas de registro u otras marcas, en la lista desplegable **[!UICONTROL Recortar]**, elija **[!UICONTROL Manual]**. Introduzca el número de píxeles que desea recortar de los lados superior, derecho, inferior e izquierdo de las páginas. Las marcas de recorte suelen tener un margen de media pulgada. Supongamos que elige **[!UICONTROL 150]** (recomendado) como resolución de píxel por pulgada. A continuación, escriba 75, 75, 75, 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda. En tal caso, recorta media pulgada de los márgenes (a 150 ppp, la mitad de 1 equivale a 75 píxeles).

* **Procesando**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de PDF]**. En la lista desplegable **[!UICONTROL Procesando]**, elija **[!UICONTROL Rasterizar]**. Para que todas las páginas y las imágenes se muestren en el catálogo electrónico, debe rasterizar el archivo PDF.

* **Extraer palabras de búsqueda (opcional)**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de PDF]**. En la lista desplegable Extraer, elija **[!UICONTROL Palabras de búsqueda]** si quiere que sus visualizadores puedan buscar por palabra clave en su catálogo electrónico.

* **Generar catálogo electrónico automáticamente a partir de PDF de varias páginas (opcional)**: en el cuadro de diálogo Opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de PDF]**. Haga clic en **[!UICONTROL Generar catálogo electrónico automáticamente a partir de PDF de varias páginas]** para que pueda crear automáticamente un catálogo electrónico al cargarlo. Puede ir directamente a la pantalla del catálogo electrónico y comenzar a trabajar en el catálogo electrónico sin necesidad de seleccionar primero los archivos PDF y el comando Generar. El catálogo electrónico recibe el mismo nombre que el archivo PDF.

* **Resolución**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de PDF]**. En el campo de texto **[!UICONTROL Resolución]**, escriba un valor. Adobe Dynamic Media Classic recomienda 150 píxeles por pulgada.

* **Espacio de color**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de PDF]**. En la lista desplegable Espacio de color, elija **[!UICONTROL Detectar automáticamente]**. Los archivos PDF creados para imprimirse suelen estar en modo CMYK, mientras que los diseñados para visualizarse en línea están en modo RGB. Si un archivo PDF utiliza ambos espacios de color, puede seleccionar un espacio específico si elige Forzar RGB o Forzar CMYK. Los archivos PDF pueden utilizar ambos espacios de color, por ejemplo, cuando los gráficos utilizan un espacio de color CMYK pero las imágenes utilizan RGB. Si ha cargado un perfil ICC, su nombre aparecerá en el menú Espacio de color, desde donde lo podrá elegir.

  Ver [perfiles ICC (International Color Consortium)](/help/using/icc-profiles.md).

* **Opciones de perfil de color**: en el cuadro de diálogo de opciones del trabajo de carga, seleccione **[!UICONTROL Opciones de perfil de color]** y, a continuación, elija una opción de perfil de color:

   * **Conservar el espacio de color original**: conserva el espacio de color original.

   * **Personalizar de > A**: abre submenús para que pueda elegir un espacio de color de **[!UICONTROL Convertir de]** y **[!UICONTROL Convertir a]**. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Ver [perfiles ICC (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para ver los detalles de todas las opciones del PDF, consulte [Opciones de carga de PDF](pdfs.md#pdf_upload_options).
