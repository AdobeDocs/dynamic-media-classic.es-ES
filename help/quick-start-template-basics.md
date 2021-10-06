---
title: '"Inicio rápido: Funciones básicas de plantilla"'
description: Introducción e Introducción a los conceptos básicos de plantilla para ayudarle a poner en marcha Adobe Dynamic Media Classic rápidamente.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 28%

---

# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Los conceptos básicos de plantilla son archivos de imagen en capas que se pueden dirigir y crear de forma dinámica, como archivos en capas en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático que contenga capas, como un archivo PSD en capas, en una plantilla y crear plantillas en Adobe Dynamic Media Classic. Puede crear capas de texto en plantillas utilizando las fuentes cargadas en Adobe Dynamic Media Classic. Después de agregar texto a una plantilla, puede modificar las fuentes, el tamaño y el color de éstas y la justificación.

Con la página Parámetros, puede convertir cualquier aspecto de una plantilla en un parámetro accesible. De este modo podrá elegir qué imagen de capa o qué valor de texto usar en la plantilla. Los parámetros se pasan junto a la cadena URL, lo que le permite cambiar cualquier parámetro para personalizar de forma dinámica la imagen de respuesta generada por el servidor de imágenes.

Consulte también el vídeo de capacitación [Conceptos básicos de plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

Este inicio rápido está diseñado para ayudarle a empezar a utilizarlo rápidamente con los conceptos básicos de plantilla.

## 1. Cargue los archivos

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen además del PSD, pero las imágenes TIFF y PNG sin pérdida se recomiendan para las plantillas porque permiten la transparencia.

Si utiliza un archivo PSD para crear la plantilla, seleccione **[!UICONTROL Crear plantilla]** en el cuadro de diálogo **[!UICONTROL Cargar opciones de trabajo]** al cargar el archivo PSD. Elija también una opción **[!UICONTROL Layer Naming]** para que Adobe Dynamic Media Classic sepa cómo asignar nombres a las capas de PSD cuando se carguen en Adobe Dynamic Media Classic.

Si utiliza archivos de imagen, puede recortar las imágenes y crear una máscara a partir de ruta de recorte al cargar las imágenes.

En la barra de navegación global, seleccione **[!UICONTROL Upload]** para cargar un archivo PSD u otros archivos de imagen desde el equipo a una carpeta de Adobe Dynamic Media Classic. Consulte [Cargar archivos de plantilla](uploading-template-files.md#uploading_template_files).

## 2. Crear una plantilla

Para crear una plantilla a partir de un archivo de PSD, seleccione **[!UICONTROL Crear plantilla]** al cargar el archivo. Para crear una plantilla a partir de imágenes, en la barra de navegación global, vaya a **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**, introduzca una medición de ancho y alto para el lienzo. Cerca de la esquina superior derecha de la página, seleccione **[!UICONTROL Designer]** o **[!UICONTROL Developer]** y arrastre imágenes a la página Plantilla. También puede seleccionar las imágenes *antes* de ir a **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. La página Plantilla ofrece herramientas para:

* Agregar capas de imagen. Para agregar una capa, arrastre una imagen a la página Plantilla .
* Agregar capas de texto. Seleccione el icono **[!UICONTROL Text tool]**. Arrastre el puntero para crear un cuadro para la capa de texto; a continuación, dé formato al texto con las herramientas de la página Texto .
* Cambiar el tamaño y la posición de capas.
* Cambiar el orden de capas.
* Aplicar efectos de sombra y resplandor en capas de imagen y texto.

Consulte [Crear una plantilla](creating-template.md#creating_a_template).

## 3. Crear parámetros de plantilla

El siguiente paso es la parametrización de las propiedades de capas para determinar qué propiedades se incluyen en la cadena URL. Los parámetros aumentan la flexibilidad de uso de las plantillas. Después de convertir una propiedad de capa en parámetro, se puede cambiar de forma dinámica.

Para parametrizar una capa, abra la plantilla en la página Plantilla y, a continuación, seleccione **[!UICONTROL Parameters]** junto al nombre de una capa. En la página Parámetros, seleccione la opción situada junto a cada parámetro que desee añadir. Consulte [Crear parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

## 4. Publicar plantillas

Al publicar la plantilla, esta se coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar dinámicamente a su sitio web o aplicación. La publicación también activa la URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media hasta su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, marque para publicarla y, en la barra de navegación global, seleccione **[!UICONTROL Publicar]**. A continuación, seleccione **[!UICONTROL Enviar publicación]**. Consulte [Publicar plantillas](publishing-templates.md#publishing_templates).

## 5. Vincular una plantilla a una página web

Dynamic Media Classic crea direcciones URL para plantillas y las activa al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas URL desde la página Vista previa de plantilla .

Seleccione la plantilla en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]** para abrir la página Vista previa de la plantilla. Elija un ajuste preestablecido de imagen para enviar la plantilla y, a continuación, seleccione **[!UICONTROL Copiar URL]**. Después de copiar la URL de la página Vista previa, puede utilizarla en su sitio web o aplicación. Consulte [Vinculación de una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
