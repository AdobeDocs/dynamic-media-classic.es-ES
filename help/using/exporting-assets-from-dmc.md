---
title: Exportación de recursos desde Adobe Dynamic Media Classic
description: Obtenga información sobre cómo exportar recursos desde Adobe Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# Exportación de recursos desde Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Puede guardar los recursos que editó en Adobe Dynamic Media Classic en una unidad de red local. Los recursos exportados se incluyen en un archivo ZIP que se puede descargar o enviar por correo electrónico.

El archivo ZIP comprimido tiene un tamaño máximo de 1 GB para el trabajo de exportación. Además, se le permite un máximo de 500 recursos totales por trabajo de exportación.

Adobe Dynamic Media Classic mantiene un registro de los trabajos de exportación en la pantalla Trabajos.

**Para exportar recursos desde Adobe Dynamic Media Classic:**

1. Seleccione los recursos que desea exportar y vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Exportar]**.
1. En la ventana Exportar recursos seleccionados, haga clic en **[!UICONTROL Opciones de imagen]** y especifique cualquiera de las siguientes opciones (los administradores determinan las opciones que están disponibles para los usuarios):

   * **[!UICONTROL Ajustes preestablecidos]** - Si lo desea, seleccione un ajuste preestablecido de imagen para dar formato al recurso al exportarlo. Si elige un ajuste preestablecido de imagen, las otras opciones de formato no estarán disponibles, ya que el recurso adopta los formatos definidos en el ajuste preestablecido de imagen.

   * **[!UICONTROL Conversión]** : convierta el archivo de recursos o la imagen original.

   * **[!UICONTROL Tamaño]** - Puede seleccionar un tamaño estándar. O bien, puede seleccionar **[!UICONTROL Otros]** desde el **[!UICONTROL Tamaño]** , elija la unidad de medida que desee y, a continuación, especifique la anchura y la altura.

     Consulte también [Especificar las opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Formato]** - Elija un formato de imagen.

   * **[!UICONTROL Color]** - Elija RGB, CMYK o Gris.

   * **[!UICONTROL Resolución]** - Elija 72 ppp, 150 ppp o 300 ppp.

   * **[!UICONTROL Nombre de trabajo]** : Puede asignar un nombre de trabajo a la exportación.

   * **[!UICONTROL Enviar correo electrónico a]** - Si lo desea, escriba una dirección de correo electrónico si desea enviar los recursos por correo electrónico. Este mensaje de correo electrónico contiene una URL a la que el destinatario puede ir para descargar los recursos.

1. Seleccionar **[!UICONTROL Exportar]**.

Se admiten tres acciones de exportación básicas:

* Archivo original (se exporta el archivo original del recurso)
* Opción de conversión con un ajuste preestablecido (se utiliza un ajuste preestablecido de imagen para dar formato al recurso)
* Opción de conversión sin un ajuste preestablecido (se utiliza el cuadro de diálogo de exportación para especificar los modificadores de la imagen)

No se pueden exportar los siguientes tipos de recursos. Todos los demás generan una exportación.

* Conjuntos de imágenes
* Conjuntos de procesamiento
* Conjuntos de giros
* Conjuntos de medios
* Conjuntos de múltiples velocidades
* Catálogos electrónicos

Además, las plantillas no se pueden exportar como “archivos originales”.

Es posible usar la conversión con el fin de exportar los siguientes tipos de recursos:

* Imágenes
* Plantillas
* Imágenes ajustadas
* PDF (genera páginas convertidas)
* PostScript®

Si se indica una amplia selección de tipos de recursos diversos al proceso de exportación, se produce el siguiente comportamiento:

* Antes de enviar el trabajo, se eliminan de la lista todos los tipos de recursos que no se pueden exportar
* Si se solicita una conversión, se convierten todos los tipos susceptibles y todos los demás se exportan como originales
