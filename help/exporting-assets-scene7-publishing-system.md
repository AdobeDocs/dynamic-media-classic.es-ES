---
title: Exportación de recursos de Scene7 Publishing System
seo-title: Exportación de recursos de Scene7 Publishing System
description: nulo
seo-description: Obtenga información sobre cómo exportar recursos desde Scene 7 Publishing System.
uuid: d 42 b 7 a 73-80 c 0-4 a 9 a-a 04 e -7 ef 53 e 6 fcf 22
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: eb 850 ec 7-a 669-41 ea-b 2 b 0-4 c 9178 e 34 f 95
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Exportación de recursos de Scene7 Publishing System{#exporting-assets-from-scene-publishing-system}

Puede guardar en una unidad de red local los recursos que haya editado en Scene7 Publishing System. Los recursos exportados se incluyen en un archivo ZIP que se puede descargar o enviar por correo electrónico.

El archivo ZIP comprimido tiene un tamaño máximo de 1 GB para el trabajo de exportación. Asimismo, tenga en cuenta que se permite un máximo de 500 recursos en total por trabajo de exportación.

Dynamic Media Classic mantiene un registro de los trabajos de exportación en la pantalla Trabajos.

**Para exportar recursos de Scene7 Publishing System**

1. Seleccione los recursos que desea exportar y haga clic en **Archivo** &gt; **Exportar**.
1. En la ventana Exportar recursos seleccionados, haga clic en **Opciones de imagen** y especifique cualquiera de las siguientes opciones (los administradores determinan las opciones que están disponibles para los usuarios):

   **Opcionalmente,** elija un ajuste preestablecido de imagen para dar formato al recurso al exportarlo. Si elige un ajuste preestablecido de imagen, las otras opciones de formato no estarán disponibles, ya que el recurso adopta los formatos definidos en el ajuste preestablecido de imagen.

   **Conversión** Convierta el archivo de recurso o la imagen original.

   **Tamañopuede seleccionar** un tamaño estándar. O bien, puede hacer clic en Otro en la lista desplegable Tamaño, elegir la unidad de medida que desee y, a continuación, especificar la anchura y la altura.

   Consulte también [Especificación de opciones de exportación disponibles para los usuarios de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   **Formato** Seleccione un formato de imagen.

   **Color** Seleccione RGB, CMYK o Gris.

   **Resolución** Seleccione 72, 150 o 300 ppp.

   **Nombre** de trabajo Puede asignar un nombre de trabajo a la exportación.

   **Enviar correo electrónico a** opcionalmente, introduzca una dirección de correo electrónico para enviar los recursos por correo electrónico. Este mensaje de correo electrónico contiene una URL a la que el destinatario puede ir para descargar los recursos.

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

