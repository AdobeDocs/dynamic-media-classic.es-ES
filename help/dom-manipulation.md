---
title: Manipulación DOM
seo-title: Manipulación DOM
description: nulo
seo-description: Obtenga información sobre manipulación DOM.
uuid: 275 cd 49 d -2 a 55-41 f 9-80 b 0-e 147 d 0 cd 2907
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/template-publishing
discoiquuid: 890 ca 93 e -3146-4347-864 b-bd 5 e 94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Manipulación DOM{#dom-manipulation}

La manipulación DOM ("document object model", modelo de objeto de documento) es una técnica para editar un archivo de diseño mediante la manipulación directa de su código XML. La manipulación DOM le proporciona más control sobre los elementos de diseño variables, incluido el cambio del contenido y la apariencia; también puede crear nuevos elementos según los necesite.

Dynamic Media Classic permite manipular el DOM de una plantilla FXG clásica de Media Media Classic mediante comandos URL después de publicar la plantilla. Los elementos de diseño de la plantilla FXG se manipulan al transferir comandos a través de la URL. De esta forma, puede manipular de forma dinámica y añadir atributos a los gráficos.

Para utilizar la manipulación DOM, cree s 7: Elementids en el archivo de Illustrator antes de convertirlo en un archivo FXG de Dynamic Media Classic y cargarlo en SPS.

>[!NOTE]
>
>para utilizar comandos de manipulación DOM, todos los valores pasados deben estar codificados en una URL.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Creación de ID de elemento de s7 en archivos de Illustrator {#creating-s-elementids-in-illustrator-files}

Para utilizar la manipulación DOM con un diseño creado en Illustrator, cree ID de elementos de s7 en su archivo de Illustrator. La creación de ID de elementos de s7 permite a los elementos del diseño modificarse con comandos de URL después de que la plantilla se haya publicado.

### Creación de ID de elementos de s7 para la manipulación DOM de texto {#creating-s-elementids-for-dom-manipulation-of-text}

Para crear un ID de elemento de s7 para la manipulación DOM de un objeto de texto, abra el panel Capas en Illustrator. A continuación, proporcione un ID de elemento de s7 como nombre a la capa de texto que tenga la variable de texto. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. A continuación, se muestran ejemplos de nombres de capas de texto con ID de elementos de s7:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Creación de ID de elementos de s7 para la manipulación DOM de objetos {#creating-s-elementids-for-dom-manipulation-of-objects}

Cree ID de elementos de s7 para los objetos si desea que los usuarios puedan cambiar los atributos de los objetos. Los objetos pueden estar compuestos por marcos de texto completos, gráficos e imágenes. Un color de fondo es un ejemplo de un ID de elemento de color. Al cambiar una promoción, el usuario final podrá cambiar el color de fondo de un póster para que esté acorde con la promoción.

Antes de crear un ID de elemento de s7 para un objeto en Illustrator, cree una capa independiente para éste.

Siga estos pasos para crear un ID de elemento de s7 para un objeto en Illustrator:

1. Seleccione el objeto.
1. Haga clic **en Ventanas** &gt; **Capas**.
1. En el panel Capas, asigne un nombre a la capa de objeto con un s 7: Elementid. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. A continuación, se muestran ejemplos de nombres de capas de objeto con ID de elementos de s7:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Publicación de plantillas FXG {#publish-fxg-templates}

Al publicar la plantilla FXG, ésta se coloca en los servidores de Dynamic Media Classic, donde está disponible para el sitio web y la aplicación. Durante el proceso de publicación, Scene7 Publishing System activa las URL necesarias para la aplicación o el sitio web.

>[!NOTE]
>
>Para usar la plantilla FXG, publique todo el contenido utilizado para crearla, incluidas fuentes e imágenes. Si no incluye todos los campos requeridos, aparecerá un mensaje de error durante la publicación.

### Marcado de plantillas FXG para publicación {#mark-fxg-templates-for-publish}

Las plantillas y todos los archivos de soporte se deben marcar para publicación para que se coloquen en los servidores de imágenes de Dynamic Media.

1. En el panel Examinar, seleccione la plantilla de FXG junto con los gráficos, imágenes y fuentes utilizadas.
1. Haga clic **en Marcar para publicación**.

### Publicación de la plantilla FXG {#publish-your-fxg-template}

1. En la barra de navegación global, haga clic en **Publicar**.
1. Seleccione una opción Cuándo e introduzca un nombre para el trabajo de publicación, si lo desea.
1. Click **Start Publish**.

### Indicador de desbordamiento de texto {#text-overflow-indicator-display}

El *indicador de desbordamiento de texto* muestra si el texto se sale del espacio que tiene asignado en un marco de texto (o en el último marco de texto si se trata de un texto enlazado). Este indicador es un cuadro rojo con un signo más en su interior. Los indicadores de desbordamiento de texto siempre están activados en SPS.

Los indicadores de desbordamiento de texto se controlan con el modificador `markOverflowingTextFrame`. Este modificador se usa de la manera siguiente:

| Modificador y valores | Descripción |
|--- |--- |
| Markoverflowingtextframe = 0,1 | Con el valor 1, aparecen los indicadores de flujo de texto. El valor predeterminado es 0. (Aunque el valor predeterminado es 0, los indicadores de desbordamiento de texto siempre están activados en SPS). Tenga en cuenta que, en el modificador markOverflowingTextFrame, se distingue entre mayúsculas y minúsculas. |

>[!MORELIKETHIS]
>
>* [Definición de variabilidad: parametrización y manipulación DOM](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publicación](publishing-files.md#publishing_files)

