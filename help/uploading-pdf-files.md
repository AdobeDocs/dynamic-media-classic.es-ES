---
title: Carga de archivos PDF
seo-title: Carga de archivos PDF
description: nulo
seo-description: Aprenda a cargar los archivos PDF asociados a un catálogo electrónico.
uuid: 9 e 178 bb 2-ac 09-427 a-b 61 a-aad 4 e 87 a 5837
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0097 cba 5-c 886-4115-bc 35-7 ae 7 a 500202 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Carga de archivos PDF{#uploading-the-pdf-files}

Los catálogos electrónicos suelen crearse a partir de archivos PDF; estos archivos contienen toda la información de imágenes, así como fuentes y gráficos vectoriales. También puede generar un catálogo electrónico a partir de imágenes. Tras preparar los archivos PDF que desea cargar, seleccione el botón Cargar en la barra de navegación global para iniciar la carga de los archivos PDF.

## Preparación de los archivos PDF {#preparing-your-pdf-files}

Antes de cargar los archivos PDF a Scene7 Publishing System, debe prepararlos:

* Coloque todos los archivos en la misma carpeta del ordenador o de la red para facilitar la carga de los mismos.
* Asigne un nombre alfanumérico a los archivos para determinar el orden de las páginas. Si ordena las páginas, resultará más fácil colocarlas correctamente una vez se hayan cargado los archivos.
* Examine las páginas PDF y compruebe si contienen marcas de recorte, destinos de registro o barras de color. Estas marcas determinan dónde se corta el papel al imprimir; deben eliminarse antes de colocar el catálogo electrónico en la Web. Dynamic Media Classic proporciona opciones para las marcas de recorte al cargar archivos PDF.
* Si desea que los usuarios del catálogo electrónico tengan la posibilidad de realizar búsquedas por palabra clave dentro del mismo, averigüe si los archivos PDF están "acoplados". Si los archivos PDF están acoplados, no se podrán extraer palabras de búsqueda. Para averiguar si un archivo PDF está acoplado, intente seleccionar texto dentro del mismo. Si no puede seleccionar texto, significa que el archivo PDF está acoplado y por lo tanto los usuarios no pueden realizar búsquedas por palabra clave dentro del catálogo electrónico.
* Puesto que están diseñados para imprimirse, los archivos PDF suelen contener imágenes en CMYK. De forma predeterminada, SPS puede detectar estas imágenes CMYK de forma inteligente y convertirlas con un perfil de color CMYK interno. Sin embargo, si desea usar un perfil de color personalizado para convertir imágenes CMYK, puede hacerlo.

   Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Prácticas recomendadas para cargar PDF {#best-practice-pdf-upload-options}

Para obtener información más detallada sobre los diferentes métodos de carga, consulte [Carga de archivos](uploading-files.md#uploading_your_files).

Elija los archivos que desea cargar y seleccione estas opciones de PDF *recomendadas*:

**Recortarseleccione el** menú Recortar y elija Manual si las páginas contienen marcas de recorte, marcas de registro u otras marcas. Elija el número de píxeles que desea recortar en la parte superior, derecha, inferior e izquierda de las páginas. Las marcas de recorte suelen tener un margen de media pulgada. Suponiendo que ha elegido una resolución de 150 píxeles por pulgada (la configuración recomendada), si introduce 75, 75, 75, 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, recortará media pulgada de los márgenes (en una resolución es 150 ppp, media pulgada equivale a 75 píxeles).

**Procesamiento** Seleccione el menú Procesamiento y elija Rasterizar. Para que todas las páginas y las imágenes se muestren en el catálogo electrónico, debe rasterizar el archivo PDF.

**Extraer palabras de búsqueda (opcional)** Seleccione esta opción si desea que los visores puedan buscar por palabra clave en el catálogo electrónico.

**Generar catálogo electrónico automáticamente a partir de PDF de varias páginas (opcional)** Seleccione esta opción para crear automáticamente un catálogo electrónico al cargarlo. Puede ir directamente a la pantalla del catálogo electrónico y comenzar a trabajar en el catálogo electrónico sin necesidad de seleccionar primero los archivos PDF y el comando Generar. El catálogo electrónico recibe el mismo nombre que el archivo PDF.

**Resolution** Dynamic Media Classic recomienda 150 píxeles por pulgada.

**Colorspace** Dynamic Media Classic recomienda seleccionar Detectar automáticamente. Los archivos PDF creados para imprimirse suelen estar en modo CMYK, mientras que los diseñados para visualizarse en línea están en modo RGB. Si un archivo PDF utiliza ambos espacios de color, puede seleccionar un espacio específico si elige Forzar RGB o Forzar CMYK. Los archivos PDF pueden utilizar ambos espacios de color, por ejemplo, cuando los gráficos utilizan un espacio de color CMYK pero las imágenes utilizan RGB. Si ha cargado un perfil ICC, su nombre aparecerá en el menú Espacio de color, desde donde lo podrá elegir.

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

**Perfil de color** Elija una opción de Perfil de color:

**Convertir
a SRGB** Convierte a SRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

**Mantener espacio de color original** Conserva el espacio de color original.

**Personalizar &gt; Para** abrir menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o uno que haya cargado en SPS. 

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Para ver los detalles de todas las opciones del PDF, consulte [Opciones de carga de PDF](pdfs.md#pdf_upload_options).

