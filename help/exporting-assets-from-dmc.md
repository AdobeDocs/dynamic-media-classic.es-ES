---
title: Exportación de recursos desde Dynamic Media Classic
seo-title: Exportación de recursos desde Dynamic Media Classic
description: nulo
seo-description: Obtenga información sobre cómo exportar recursos desde Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 69%

---


# Exportación de recursos desde Dynamic Media Classic{#exporting-assets-from-dmc}

Puede guardar los recursos que haya editado en Dynamic Media Classic en una unidad de red local. Los recursos exportados se incluyen en un archivo ZIP que se puede descargar o enviar por correo electrónico.

El archivo ZIP comprimido tiene un tamaño máximo de 1 GB para el trabajo de exportación. Asimismo, tenga en cuenta que se permite un máximo de 500 recursos en total por trabajo de exportación.

Dynamic Media Classic mantiene un registro de los trabajos de exportación en la pantalla Trabajos.

**Para exportar recursos desde Dynamic Media Classic**

1. Seleccione los recursos que desea exportar y haga clic en **Archivo** > **Exportar**.
1. En la ventana Exportar recursos seleccionados, haga clic en **Opciones de imagen** y especifique cualquiera de las siguientes opciones (los administradores determinan las opciones que están disponibles para los usuarios):

   * **Ajustes preestablecidos** Si lo desea, puede elegir un ajuste preestablecido de imagen para dar formato al recurso al exportarlo. Si elige un ajuste preestablecido de imagen, las otras opciones de formato no estarán disponibles, ya que el recurso adopta los formatos definidos en el ajuste preestablecido de imagen.

   * **Conversión** Convertir el archivo de recurso o la imagen original.

   * **Tamaño** Puede seleccionar un tamaño estándar. O bien, puede hacer clic en Otro en la lista desplegable Tamaño, elegir la unidad de medida que desee y, a continuación, especificar la anchura y la altura.

      Consulte también [Especificación de opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **Formato** Elija un formato de imagen.

   * **Color** Elija RGB, CMYK o gris.

   * **Resolución** Elija 72, 150 o 300 ppp.

   * **Nombre** del trabajo Puede asignar un nombre de trabajo a la exportación.

   * **Enviar correo electrónico a** De forma opcional, introduzca una dirección de correo electrónico para enviar los recursos por correo electrónico. Este mensaje de correo electrónico contiene una URL a la que el destinatario puede ir para descargar los recursos.

1. Haga clic en **Exportar**.

Se admiten tres acciones de exportación básicas:

* Archivo original (se exporta el archivo original del recurso)
* Opción de conversión con un ajuste preestablecido (se utiliza un ajuste preestablecido de imagen para dar formato al recurso)
* Opción de conversión sin un ajuste preestablecido (se utiliza el cuadro de diálogo de exportación para especificar los modificadores de la imagen)

No se pueden exportar los siguientes tipos de recursos. Todos los demás sí deben generar una exportación.

* Conjuntos de imágenes
* Conjuntos de procesamiento
* Conjuntos de giros
* Conjuntos de medios
* Conjuntos de varias velocidades de bits
* Catálogos electrónicos

Además, las plantillas no se pueden exportar como “archivos originales”.

Es posible usar la conversión con el fin de exportar los siguientes tipos de recursos:

* Imágenes
* Plantillas
* Imágenes ajustadas
* PDF (se generarán páginas convertidas)
* PostScript

Si se indica una amplia selección de tipos de recursos diversos al proceso de exportación, se produce el siguiente comportamiento:

* Antes de enviar el trabajo, se eliminan de la lista todos los tipos de recursos que no se pueden exportar
* Si se solicita una conversión, se convierten todos los tipos susceptibles y todos los demás se exportan como originales

