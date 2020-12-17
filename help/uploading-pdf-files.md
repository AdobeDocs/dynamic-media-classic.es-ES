---
title: Carga de archivos PDF
seo-title: Carga de archivos PDF
description: nulo
seo-description: Obtenga información sobre cómo cargar los archivos PDF asociados a un catálogo electrónico.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 71%

---


# Carga de archivos PDF{#uploading-the-pdf-files}

Los catálogos electrónicos suelen crearse a partir de archivos PDF; estos archivos contienen toda la información de imágenes, así como fuentes y gráficos vectoriales. También puede generar un catálogo electrónico a partir de imágenes. Tras preparar los archivos PDF que desea cargar, seleccione el botón Cargar en la barra de navegación global para iniciar la carga de los archivos PDF.

## Preparación de los archivos PDF  {#preparing-your-pdf-files}

Prepare sus archivos PDF antes de cargarlos en Dynamic Media Classic:

* Coloque todos los archivos en la misma carpeta del ordenador o de la red para facilitar la carga de los mismos.
* Asigne un nombre alfanumérico a los archivos para determinar el orden de las páginas. Si ordena las páginas, resultará más fácil colocarlas correctamente una vez se hayan cargado los archivos.
* Examine las páginas PDF y compruebe si contienen marcas de recorte, destinos de registro o barras de color. Estas marcas determinan dónde se corta el papel al imprimir; deben eliminarse antes de colocar el catálogo electrónico en la Web. Dynamic Media Classic proporciona opciones para recortar marcas al cargar archivos PDF.
* Si desea que los usuarios del catálogo electrónico tengan la posibilidad de realizar búsquedas por palabra clave dentro del mismo, averigüe si los archivos PDF están &quot;acoplados&quot;. Si los archivos PDF están acoplados, no se podrán extraer palabras de búsqueda. Para averiguar si un archivo PDF está acoplado, intente seleccionar texto dentro del mismo. Si no puede seleccionar texto, significa que el archivo PDF está acoplado y por lo tanto los usuarios no pueden realizar búsquedas por palabra clave dentro del catálogo electrónico.
* Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. De forma predeterminada, Dynamic Media Classic puede detectar de forma inteligente estas imágenes CMYK y convertirlas mediante un perfil de color CMYK interno. Sin embargo, si desea usar un perfil de color personalizado para convertir imágenes CMYK, puede hacerlo.

   Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Prácticas recomendadas para cargar PDF  {#best-practice-pdf-upload-options}

Para obtener información más detallada sobre los diferentes métodos de carga, consulte [Carga de archivos](uploading-files.md#uploading_your_files).

Elija los archivos que desea cargar y seleccione estas opciones de PDF *recomendadas*:

* ****
RecortarSeleccione el menú Recortar y elija Manual si las páginas contienen marcas de recorte, marcas de registro u otras marcas. Elija el número de píxeles que desea recortar en la parte superior, derecha, inferior e izquierda de las páginas. Las marcas de recorte suelen tener un margen de media pulgada. Suponiendo que ha elegido una resolución de 150 píxeles por pulgada (la configuración recomendada), si introduce 75, 75, 75, 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, recortará media pulgada de los márgenes (en una resolución es 150 ppp, media pulgada equivale a 75 píxeles).

* ****
ProcesamientoSeleccione el menú Procesamiento y elija Rasterizar. Para que todas las páginas y las imágenes se muestren en el catálogo electrónico, debe rasterizar el archivo PDF.

* **Extraer palabras de búsqueda (opcional)**
Seleccione esta opción si desea que los visores puedan buscar por palabra clave en el catálogo electrónico.

* **Generar catálogo electrónico automáticamente a partir de PDF de varias páginas (opcional)**
Seleccione esta opción para crear automáticamente un catálogo electrónico al cargar. Puede ir directamente a la pantalla del catálogo electrónico y comenzar a trabajar en el catálogo electrónico sin necesidad de seleccionar primero los archivos PDF y el comando Generar. El catálogo electrónico recibe el mismo nombre que el archivo PDF.

* ****
ResoluciónDynamic Media Classic recomienda 150 píxeles por pulgada.

* ****
ColorspaceDynamic Media Classic recomienda elegir Detectar automáticamente. Los archivos PDF creados para imprimirse suelen estar en modo CMYK, mientras que los diseñados para visualizarse en línea están en modo RGB. Si un archivo PDF utiliza ambos espacios de color, puede seleccionar un espacio específico si elige Forzar RGB o Forzar CMYK. Los archivos PDF pueden utilizar ambos espacios de color, por ejemplo, cuando los gráficos utilizan un espacio de color CMYK pero las imágenes utilizan RGB. Si ha cargado un perfil ICC, su nombre aparecerá en el menú Espacio de color, desde donde lo podrá elegir.

   Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

* **Perfil**
de colorElija una opción de Perfil de color:

* **Convertir a**
SRGBConvertidos a SRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

* **Mantener**
espacio de color originalConserva el espacio de color original.

* **Personalizado de >**
AAbre los menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Dynamic Media Classic.

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para ver los detalles de todas las opciones del PDF, consulte [Opciones de carga de PDF](pdfs.md#pdf_upload_options).

