---
title: Fuentes
description: Aprenda a utilizar fuentes en Adobe Dynamic Media Classic.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# Fuentes{#fonts}

A veces, Adobe Dynamic Media Classic requiere que cargue un archivo de fuente para introducir o procesar texto en una fuente determinada. Por ejemplo, para utilizar una fuente determinada para el texto de una capa de plantilla, cargue el archivo de fuente. Para mostrar los números de página del visor de catálogos electrónicos con una fuente determinada, cargue el archivo de fuente.

Adobe Dynamic Media Classic admite estos tipos de fuentes:

* Todas las fuentes TrueType
* fuentes de PostScript®
* Fuentes OpenType/TrueType
* Fuentes OpenType/PostScript
* PhotoFonts

Una vez cargado un archivo de fuente, puede cambiar su ID de Dynamic Media Classic de Adobe, su nombre y la información de tipo en la pantalla Editar información.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda cargar todos los estilos de fuente (negrita, cursiva, negrita/cursiva y normal) si planea utilizar fuentes en las capas de plantilla. Adobe Dynamic Media Classic necesita estos estilos de fuente para procesar solicitudes. También se recomienda cargar todos los archivos Type 1 de PostScript/Adobe que estén asociados con la fuente, ya que algunas de estas fuentes contienen información detallada de espaciado.

## Cargar archivos de fuente {#uploading-font-files}

Cargue archivos de fuente utilizando las mismas técnicas que usa para cargar otros archivos. Puede almacenar archivos de fuente en cualquier carpeta de Adobe de Dynamic Media Classic. Consulte [Carga de los archivos](uploading-files.md#uploading_your_files).

## Editar información del archivo de fuente {#editing-font-file-information}

Puede cambiar el nombre de ID de una fuente y su información de tipo. Editar una fuente puede resultar útil en las búsquedas y facilitar la identificación de fuentes.

En el panel Examinar, seleccione el archivo de fuente que desea editar en la Vista de detalles y elija Archivo > Editar información. Se abrirá la pantalla Editar información. Elija las siguientes opciones y, a continuación, seleccione **[!UICONTROL Enviar]**.

* **[!UICONTROL Nombre de fuente]** : este nombre identifica la fuente cuando se publica.

* **[!UICONTROL Nombre PostScript]** : este nombre es el nombre completo de PostScript para la fuente. Suele referirse al grosor o el estilo.

* **[!UICONTROL Nombre RTF]** : este nombre aparece en un menú emergente del editor RTF donde se crean las capas de texto de la plantilla.

* **[!UICONTROL Nombre de la familia de fuentes]** : este nombre enumera el nombre de la fuente sin el indicador de estilo, peso o tipo de fuente.

* **[!UICONTROL Estilo de fuente]** : las opciones son Normal, Negrita, Cursiva y Negrita-Cursiva.

* **[!UICONTROL Tipo de fuente]** : las opciones son TrueType y Adobe Type 1. Si utiliza otro nombre para denominar estas fuentes, puede introducirlo.

* **[!UICONTROL Abreviación de tipo de fuente]** : las opciones son las siguientes:

   * **[!UICONTROL TTF]** : Archivos de fuente TrueType utilizados para la representación de PDF/PostScript y el servicio de imágenes.

   * **[!UICONTROL AFM]** : archivos de fuente de Adobe PostScript que contienen información de métricas de fuente de Adobe y que se utilizan para el servicio de imágenes.

   * **[!UICONTROL PFM]** : archivos de fuente Adobe PostScript que contienen información de métrica de fuente binaria.

   * **[!UICONTROL PFB]** : archivos de fuente Adobe PostScript que contienen información de esquema de fuente binaria y que se utilizan para el procesamiento y el servicio de imágenes de PDF/PostScript.
