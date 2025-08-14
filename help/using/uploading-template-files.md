---
title: Cargar archivos de plantilla
description: Obtenga información sobre cómo cargar archivos de plantilla en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 32%

---

# Cargar archivos de plantilla{#uploading-template-files}

Cargue en Adobe Dynamic Media Classic los archivos que necesite para la plantilla antes de empezar a crearla. Puede crear plantillas a partir de un Adobe® Photoshop® PSD o un archivo de imagen. Se recomienda usar imágenes TIFF y PNG, ya que permiten transparencia.

>[!NOTE]
>
>Adobe Dynamic Media Classic recomienda utilizar imágenes transparentes de TIFF o PSD en las plantillas con el tamaño exacto que desee para mostrarlas en el sitio web. Al publicar la plantilla, utilice un ajuste preestablecido de imagen del mismo tamaño para llamar a la imagen. Con esta precaución se evitará un remuestreo que dé como resultado un tamaño mayor o menor que el previsto.

Las plantillas pueden crearse a partir de archivos PSD de Adobe Photoshop o archivos de imagen. 

Para obtener instrucciones detalladas sobre la carga de archivos, consulte [Cargar archivos](uploading-files.md#uploading_files). Tenga en cuenta lo siguiente al cargar archivos de plantilla:

* Si está cargando un archivo de PSD, puede crear una plantilla a partir de él. Adobe Dynamic Media Classic crea una imagen independiente para cada capa en PSD. En el cuadro de diálogo Cargar opciones del trabajo, seleccione **[!UICONTROL Opciones de Photoshop]** y seleccione **[!UICONTROL Mantener capas]** y **[!UICONTROL Crear plantilla]**. A continuación, elija una opción en la lista desplegable **[!UICONTROL Nombres de capas]** para asignar un nombre a las imágenes que Adobe Dynamic Media Classic crea a partir de las capas de PSD.
Consulte [Opciones de carga de archivos PSD](psd-files.md#psd_upload_options).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Cargue sus archivos](uploading-files.md#uploading_your_files)
>* [Trabajar con archivos de PSD](psd-files.md#working_with_psd_files)
