---
title: Fuentes
description: Aprenda a utilizar fuentes en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 23%

---

# Fuentes{#fonts}

A veces, Adobe Dynamic Media Classic requiere que cargue un archivo de fuentes para introducir o procesar texto en una fuente concreta. Por ejemplo, para utilizar una fuente determinada para el texto de una capa de plantilla, cargue el archivo de fuente. Para mostrar los números de página del visor de catálogos electrónicos con una fuente determinada, cargue el archivo de fuente.

Adobe Dynamic Media Classic admite estos tipos de fuentes:

* Todas las fuentes TrueType
* Fuentes PostScript®
* Fuentes OpenType/TrueType
* Fuentes OpenType/PostScript
* PhotoFonts

Una vez cargado un archivo de fuente, puede cambiar su Adobe Dynamic Media Classic ID, el nombre de la fuente y escribir información en la pantalla Editar información.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda cargar todos los estilos de fuente (negrita, cursiva, negrita/cursiva y normal) si planea utilizar fuentes en las capas de plantilla. Adobe Dynamic Media Classic necesita estos estilos de fuente para procesar solicitudes. También se recomienda cargar todos los `PostScript/Adobe Type1` archivos asociados con una fuente, ya que algunas de estas fuentes contienen información detallada sobre el kerning.

## Cargar archivos de fuentes {#uploading-font-files}

Cargue archivos de fuente utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar archivos de fuentes en cualquier carpeta de Adobe Dynamic Media Classic. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Editar información del archivo de fuente {#editing-font-file-information}

Puede cambiar el nombre de ID de una fuente y su información de tipo. Editar una fuente puede resultar útil en las búsquedas y facilitar la identificación de fuentes.

En el panel Examinar, seleccione el archivo de fuente que desee editar en Vista de detalles y elija Archivo > Editar información. Se abrirá la pantalla Editar información. Elija las siguientes opciones y luego seleccione **[!UICONTROL Enviar]**.

* **[!UICONTROL Nombre de fuente]**: Este nombre identifica la fuente cuando se publica.

* **[!UICONTROL Nombre de PostScript]**: Este nombre es el nombre completo de PostScript para la fuente. Suele referirse al grosor o el estilo.

* **[!UICONTROL Nombre RTF]**: Este nombre aparece en un menú emergente del editor RTF donde se crean las capas de texto de la plantilla.

* **[!UICONTROL Nombre de familia de fuentes]**: este nombre muestra el nombre de fuente sin el indicador de estilo, grosor o tipo de fuente.

* **[!UICONTROL Estilo de fuente]**: las opciones son Sin formato, Negrita, Cursiva y Negrita-Cursiva.

* **[!UICONTROL Tipo de fuente]**: las opciones son TrueType y Adobe Type 1. Si utiliza otro nombre para denominar estas fuentes, puede introducirlo.

* **[!UICONTROL Abreviatura de tipo de fuente]**: Las opciones son las siguientes:

   * **[!UICONTROL TTF]**: Archivos de fuente TrueType utilizados para la representación y el servicio de imágenes de PDF/PostScript.

   * **[!UICONTROL AFM]**: archivos de fuentes de Adobe PostScript que contienen información de métricas de fuentes de Adobe y se utilizan para el servicio de imágenes.

   * **[!UICONTROL PFM]**: archivos de fuentes de Adobe PostScript que contienen información de métricas de fuentes binarias.

   * **[!UICONTROL PFB]**: archivos de fuentes de Adobe PostScript que contienen información de esquema de fuentes binarias y que se utilizan para el procesamiento y el servicio de imágenes de PDF/PostScript.
