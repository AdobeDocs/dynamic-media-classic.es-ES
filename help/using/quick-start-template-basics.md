---
title: 'Inicio rápido: Funciones básicas de plantilla'
description: Introducción y Inicio rápido de los conceptos básicos de las plantillas para ayudarle a ponerse en marcha rápidamente con Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Los conceptos básicos de las plantillas se crean dinámicamente y se pueden dirigir mediante archivos de imagen en capas, como los archivos en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático que contenga capas, como un archivo PSD con capas, en una plantilla y crear plantillas en Adobe Dynamic Media Classic. Puede crear capas de texto en plantillas utilizando las fuentes cargadas en Adobe Dynamic Media Classic. Después de agregar texto a una plantilla, puede aplicarle formato cambiando su justificación, fuente, tamaño de fuente y color.

En la página Parámetros, puede convertir cualquier aspecto de una plantilla en un parámetro direccionable. Al hacerlo, puede cambiar qué imagen de capas utilizar o qué valor de texto utilizar en la plantilla. Los parámetros se pasan con la cadena URL, lo que permite cambiar cualquier parámetro para personalizar dinámicamente la imagen de respuesta generada desde el servidor de imágenes.

Vea también [Fundamentos de la plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de formación.

Este Inicio rápido está diseñado para ayudarle a ponerse en marcha rápidamente con Conceptos básicos de plantilla.

## &#x200B;1. Cargue los archivos

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen además de PSD, pero se recomiendan imágenes TIFF y PNG sin pérdidas para las plantillas porque permiten la transparencia.

Si usa un archivo PSD para crear la plantilla, seleccione **[!UICONTROL Crear plantilla]** en el cuadro de diálogo **[!UICONTROL Cargar opciones del trabajo]** al cargar el archivo PSD. Elija también una opción **[!UICONTROL Nombres de capas]** para que Adobe Dynamic Media Classic sepa cómo asignar nombres a las capas de PSD cuando se carguen en Adobe Dynamic Media Classic.

Si utiliza archivos de imagen, puede recortar las imágenes y también crear una máscara a partir de trazados de recorte en las imágenes a medida que las carga.

En la barra de navegación global, selecciona **[!UICONTROL Cargar]** para cargar un archivo de PSD u otros archivos de imagen de tu equipo a una carpeta en Adobe Dynamic Media Classic. Ver [Cargar archivos de plantilla](uploading-template-files.md#uploading_template_files).

## &#x200B;2. Crear una plantilla

Para crear una plantilla a partir de un archivo PSD, seleccione **[!UICONTROL Crear plantilla]** al cargar el archivo. Para crear una plantilla a partir de imágenes, en la barra de navegación global, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]** e introduzca una medida de anchura y altura para el lienzo. Cerca de la esquina superior derecha de la página, seleccione **[!UICONTROL Designer]** o **[!UICONTROL Desarrollador]** y arrastre imágenes a la página Plantilla. También puede seleccionar las imágenes *antes de* de ir a **[!UICONTROL Compilación]** > **[!UICONTROL Conceptos básicos de plantilla]**. La página Plantilla ofrece herramientas para lo siguiente:

* Agregar capas de imagen. Para agregar una capa, arrastre una imagen a la página Plantilla.
* Agregar capas de texto. Seleccione el icono **[!UICONTROL Herramienta de texto]**. Arrastre el puntero para crear un cuadro para la capa de texto; a continuación, dé formato al texto con herramientas en la página Texto.
* Cambiar el tamaño y la posición de capas.
* Cambiar el orden de capas.
* Aplicar efectos de sombra y resplandor en capas de imagen y texto.

Consulte [Crear una plantilla](creating-template.md#creating_a_template).

## &#x200B;3. Crear parámetros de plantilla

El siguiente paso es la parametrización de las propiedades de capas para determinar qué propiedades se incluyen en la cadena URL. Los parámetros aumentan la flexibilidad de uso de las plantillas. Después de convertir una propiedad de capa en parámetro, se puede cambiar de forma dinámica.

Para parametrizar una capa, abra la plantilla en la página Plantilla y, a continuación, seleccione **[!UICONTROL Parámetros]** junto al nombre de una capa. En la página Parámetros, seleccione la opción situada junto a cada parámetro que desee añadir. Consulte [Crear parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

## &#x200B;4. Publicar plantillas

La publicación de la plantilla la coloca en servidores de imágenes de Dynamic Media para que se pueda enviar dinámicamente al sitio web o a la aplicación. La publicación también activa la dirección URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, márquela para publicación y, en la barra de navegación global, seleccione **[!UICONTROL Publicar]**. Luego seleccione **[!UICONTROL Enviar publicación]**. Ver [plantillas de publicación](publishing-templates.md#publishing_templates).

## &#x200B;5. Vinculación de una plantilla a una página Web

Dynamic Media Classic crea direcciones URL para las plantillas y las activa al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas de URL desde la página Vista previa de plantilla.

Seleccione la plantilla en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]** para abrir la página Vista previa de la plantilla. Elija un ajuste preestablecido de imagen para enviar la plantilla y haga clic en el botón **[!UICONTROL Copiar URL]**. Después de copiar la dirección URL de la página Vista previa, puede utilizarla en su sitio Web o aplicación. Ver [Vincular una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
