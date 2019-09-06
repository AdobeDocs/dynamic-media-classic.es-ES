---
title: Fuentes
seo-title: Fuentes
description: nulo
seo-description: Aprenda a utilizar fuentes en Dynamic Media Classic.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 97 cecd 6 a -30 aa -44 fe-a 611-fd 71 b 02 fd 5 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Fuentes{#fonts}

En algunas ocasiones, debe cargar un archivo de fuente a Scene7 Publishing System para introducir o procesar el texto de una fuente determinada. Por ejemplo, para utilizar una fuente determinada para el texto de una capa de plantilla, cargue el archivo de fuente. Para mostrar los números de página del visor de catálogos electrónicos con una fuente determinada, cargue el archivo de fuente.

Dynamic Media Classic admite estos tipos de fuente:

* Todas las fuentes TrueType
* Fuentes postscript®
* Fuentes OpenType/TrueType
* Fuentes OpenType/PostScript
* PhotoFonts

Una vez que haya cargado el archivo de fuente, puede cambiar su ID de SPS, nombre de fuente e información de tipo en la pantalla Editar información.

>[!NOTE]
>
>Dynamic Media Classic recomienda cargar todos los estilos de fuente (negrita, cursiva, negrita/cursiva y normal) si planea utilizar fuentes en capas de plantilla. Dynamic Media Classic necesita estos estilos de fuente para procesar solicitudes. También se recomienda cargar todos los archivos Type 1 de PostScript/Adobe que estén asociados con la fuente, ya que algunas de estas fuentes contienen información detallada de espaciado.

## Carga de archivos de fuente {#uploading-font-files}

Cargue archivos de fuente utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar archivos de fuente en cualquier carpeta de SPS. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Edición de información sobre archivos de fuente {#editing-font-file-information}

Puede cambiar el nombre del ID y la información de tipo de las fuentes. Editar una fuente puede resultar útil en las búsquedas y facilitar la identificación de fuentes.

En el panel Examinar, acceda al archivo de fuente que desea editar en la vista de detalles y elija Archivo &gt; Editar información. Se abrirá la pantalla Editar información. Elija las siguientes opciones y seleccione el botón Enviar.

**Nombre** de fuente Este nombre identifica la fuente cuando se publica.

**Nombre postscript** Este nombre es el nombre postscript completo para la fuente. Suele referirse al grosor o el estilo.

**Nombre RTF** Este nombre aparece en un menú emergente del editor RTF donde se crean las capas de texto de plantilla.

**Nombre de familia de fuente** Este nombre indica el nombre de la fuente sin el indicador, grosor o indicador de tipo de fuente.

**Estilo de fuente** Las opciones son normal, negrita, cursiva y negrita-cursiva.

**Tipo de fuente** Las opciones son truetype y Adobe Type 1. Si utiliza otro nombre para denominar estas fuentes, puede introducirlo.

**Abreviatura de tipo de fuente** Las opciones son las siguientes:

**Archivos** de fuente Truetype TTF utilizados para el procesamiento y servicio de imágenes PDF/postscript.

**Archivos de fuente de Adobe** postscript que contienen información de Métricas de Adobe Font y que se utilizan para el servicio de imágenes.

**Archivos de fuente PFM** de Adobe postscript que contienen información binaria de métrica de fuentes.

**Archivos de fuente PFB** Adobe postscript que contienen información binaria contorno de fuente y se utilizan para el procesamiento y servicio de imágenes PDF/postscript.
