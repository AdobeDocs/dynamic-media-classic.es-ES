---
title: Fuentes
description: Aprenda a utilizar fuentes en Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: Profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 39%

---


# Fuentes{#fonts}

En algunos casos, Dynamic Media Classic requiere que cargue un archivo de fuente para introducir o procesar texto en una fuente determinada. Por ejemplo, para utilizar una fuente determinada para el texto de una capa de plantilla, cargue el archivo de fuente. Para mostrar los números de página del visor de catálogos electrónicos con una fuente determinada, cargue el archivo de fuente.

Dynamic Media Classic admite estos tipos de fuentes:

* Todas las fuentes TrueType
* fuentes de PostScript®
* Fuentes OpenType/TrueType
* Fuentes OpenType/PostScript
* PhotoFonts

Una vez cargado un archivo de fuente, puede cambiar su ID de Dynamic Media Classic, su nombre y la información de tipo en la pantalla Editar información.

>[!NOTE]
>
>Dynamic Media Classic recomienda cargar todos los estilos de fuente (negrita, cursiva, negrita/cursiva y normal) si planea utilizar fuentes en las capas de plantilla. Dynamic Media Classic necesita estos estilos de fuente para procesar las solicitudes. También se recomienda cargar todos los archivos Type 1 de PostScript/Adobe que estén asociados con la fuente, ya que algunas de estas fuentes contienen información detallada de espaciado.

## Carga de archivos de fuente  {#uploading-font-files}

Cargue archivos de fuente utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar archivos de fuente en cualquier carpeta de Dynamic Media Classic. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Edición de información sobre archivos de fuente  {#editing-font-file-information}

Puede cambiar el nombre del ID y la información de tipo de las fuentes. Editar una fuente puede resultar útil en las búsquedas y facilitar la identificación de fuentes.

En el panel Examinar, acceda al archivo de fuente que desea editar en la vista de detalles y elija Archivo > Editar información. Se abrirá la pantalla Editar información. Elija las siguientes opciones y seleccione el botón Enviar.

**Nombre de** fuenteEste nombre identifica la fuente cuando se publica.

**Nombre de** PostScriptEste nombre es el nombre completo de PostScript para la fuente. Suele referirse al grosor o el estilo.

**Nombre RTF** Este nombre aparece en un menú emergente del editor RTF donde se crean las capas de texto de la plantilla.

**Nombre de la familia de** fuentesEste nombre enumera el nombre de la fuente sin el indicador de estilo, peso o tipo de fuente.

**Estilo** de fuenteLas opciones son Normal, Negrita, Cursiva y Negrita-Cursiva.

**Tipo** de fuenteLas opciones son TrueType y Adobe Type 1. Si utiliza otro nombre para denominar estas fuentes, puede introducirlo.

**Abreviación de tipo** de fuenteLas opciones son las siguientes:

**** Archivos de fuente TTFTrueType utilizados para el procesamiento de PDF/PostScript y el servicio de imágenes.

**** Archivos de fuentes de AFMAdobe PostScript que contienen información de métricas de fuentes de Adobe y se utilizan para el servicio de imágenes.

**** Archivos de fuente PostScript de PFMAdobe que contienen información de métricas de fuentes binarias.

**** Archivos de fuente PostScript de PFBAdobe que contienen información binaria sobre el contorno de la fuente y que se utilizan para el procesamiento y el servicio de imágenes de PDF/PostScript.
