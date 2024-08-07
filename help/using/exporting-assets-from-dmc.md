---
title: Exportación de recursos desde Adobe Dynamic Media Classic
description: Obtenga información sobre cómo exportar recursos desde Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 38%

---

# Exportación de recursos desde Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Puede guardar los recursos que editó en Adobe Dynamic Media Classic en una unidad de red local. Los recursos exportados se incluyen en un archivo ZIP que se puede descargar o enviar por correo electrónico.

El archivo ZIP comprimido tiene un tamaño máximo de 1 GB para el trabajo de exportación. Además, se le permite un máximo de 500 recursos totales por trabajo de exportación.

Adobe Dynamic Media Classic mantiene un registro de los trabajos de exportación en la pantalla Trabajos.

**Para exportar recursos desde Adobe Dynamic Media Classic:**

1. Seleccione los recursos que desea exportar y, a continuación, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Exportar]**.
1. En la ventana Exportar recursos seleccionados, haga clic en **[!UICONTROL Opciones de imagen]** y especifique cualquiera de las siguientes opciones (los administradores determinan las opciones que están disponibles para los usuarios):

   * **[!UICONTROL Ajustes preestablecidos]**: de forma opcional, elija un Ajuste preestablecido de imagen para dar formato al recurso al exportarlo. Si elige un ajuste preestablecido de imagen, las otras opciones de formato no estarán disponibles, ya que el recurso adopta los formatos definidos en el ajuste preestablecido de imagen.

   * **[!UICONTROL Conversión]**: convierta el archivo de recursos o la imagen original.

   * **[!UICONTROL Tamaño]**: puede seleccionar un tamaño estándar. O bien, puede seleccionar **[!UICONTROL Otro]** de la lista desplegable **[!UICONTROL Tamaño]**, elegir la unidad de medida deseada y, a continuación, especificar la anchura y la altura.

     Consulte también [Especificar opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Formato]**: Elija un formato de imagen.

   * **[!UICONTROL Color]**: elige RGB, CMYK o Gris.

   * **[!UICONTROL Resolución]**: Elija 72 ppp, 150 ppp o 300 ppp.

   * **[!UICONTROL Nombre de trabajo]**: puede asignar un nombre de trabajo a la exportación.

   * **[!UICONTROL Enviar Correo Electrónico A]**: Opcional. Escriba una dirección de correo electrónico si desea enviar los recursos por correo electrónico. Este mensaje de correo electrónico contiene una URL a la que el destinatario puede ir para descargar los recursos.

1. Seleccione **[!UICONTROL Exportar]**.

Se admiten tres acciones de exportación básicas:

* Archivo original (se exporta el archivo original del recurso)
* Convertir mediante ajuste preestablecido (utilice un ajuste preestablecido de imagen para dar formato al recurso)
* Opción de conversión sin un ajuste preestablecido (se utiliza el cuadro de diálogo de exportación para especificar los modificadores de la imagen)

No se pueden exportar los siguientes tipos de recursos. Todos los demás generan una exportación.

* Conjuntos de imágenes
* Conjuntos de procesamiento
* Conjuntos de giros
* Conjuntos de medios
* Conjuntos de múltiples velocidades
* Catálogos electrónicos

Además, las plantillas no se pueden exportar como un &quot;archivo original&quot;.

Es posible usar la conversión con el fin de exportar los siguientes tipos de recursos:

* Imágenes
* Plantillas
* Imágenes ajustadas
* PDF (genera páginas convertidas)
* PostScript®

Si se indica una amplia selección de tipos de recursos diversos al proceso de exportación, se produce el siguiente comportamiento:

* Todos los tipos de recursos que no se pueden exportar se eliminan de la lista antes del envío del trabajo
* Si se solicita una conversión, todos los tipos que se pueden convertir son y todos los demás se exportan como originales
