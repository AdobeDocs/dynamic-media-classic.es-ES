---
title: '"Inicio rápido: Funciones básicas de plantilla"'
description: Introducción e Introducción a los conceptos básicos de plantilla para ayudarle a poner en marcha rápidamente.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Los conceptos básicos de plantilla son archivos de imagen en capas que se pueden dirigir y crear de forma dinámica, como archivos en capas en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático que contenga capas, como un archivo PSD en capas, en una plantilla y crear plantillas en Dynamic Media Classic. Puede crear capas de texto en plantillas utilizando las fuentes cargadas en Dynamic Media Classic. Después de agregar texto a una plantilla, puede modificar las fuentes, el tamaño y el color de éstas y la justificación.

Con la página Parámetros, puede convertir cualquier aspecto de una plantilla en un parámetro accesible. De este modo podrá elegir qué imagen de capa o qué valor de texto usar en la plantilla. Los parámetros se pasan junto a la cadena URL, lo que le permite cambiar cualquier parámetro para personalizar de forma dinámica la imagen de respuesta generada por el servidor de imágenes.

Este inicio rápido se ha diseñado para el uso inicial de Funciones básicas de plantilla. 

## 1. Cargue los archivos

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Dynamic Media Classic admite muchos formatos de archivo de imagen además de PSD, pero las imágenes TIFF y PNG sin pérdida se recomiendan para las plantillas porque permiten la transparencia.

Si utiliza un archivo PSD para crear la plantilla, seleccione **[!UICONTROL Crear plantilla]** en el cuadro de diálogo **[!UICONTROL Opciones de carga de trabajo]** al cargar el archivo PSD. Elija también una opción **[!UICONTROL Layer Naming]** para que Dynamic Media Classic sepa cómo asignar nombres a las capas PSD cuando se cargan en Dynamic Media Classic.

Si utiliza archivos de imagen, puede recortar las imágenes y crear una máscara a partir de ruta de recorte al cargar las imágenes.

En la barra de navegación global, haga clic en **[!UICONTROL Cargar]** para cargar un archivo PSD u otros archivos de imagen desde el equipo a una carpeta de Dynamic Media Classic. Consulte [Carga de archivos de plantilla](uploading-template-files.md#uploading_template_files).

## 2. Crear una plantilla

Para crear una plantilla a partir de un archivo PSD, seleccione **[!UICONTROL Crear plantilla]** al cargar el archivo. Para crear una plantilla a partir de imágenes, en la barra de navegación global, haga clic en **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]** e introduzca una medición de ancho y alto para el lienzo. Cerca de la esquina superior derecha de la página, seleccione **[!UICONTROL Designer]** o **[!UICONTROL Developer]** y arrastre imágenes a la página Plantilla. También puede seleccionar las imágenes *antes* de hacer clic en **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de la plantilla]**. La página Plantilla ofrece herramientas para:

* Agregar capas de imagen. Para agregar una capa, arrastre una imagen a la página Plantilla .
* Agregar capas de texto. Haga clic en el icono **[!UICONTROL Herramienta de texto]**. Arrastre el puntero para crear un cuadro para la capa de texto; a continuación, dé formato al texto con las herramientas de la página Texto .
* Cambiar el tamaño y la posición de capas.
* Cambiar el orden de capas.
* Aplicar efectos de sombra y resplandor en capas de imagen y texto.

Consulte [Creación de una plantilla](creating-template.md#creating_a_template).

## 3. Crear parámetros de plantilla

El siguiente paso es la parametrización de las propiedades de capas para determinar qué propiedades se incluyen en la cadena URL. Los parámetros aumentan la flexibilidad de uso de las plantillas. Después de convertir una propiedad de capa en parámetro, se puede cambiar de forma dinámica.

Para parametrizar una capa, abra la plantilla en la página Plantilla y, a continuación, haga clic en **[!UICONTROL Parámetros]** junto al nombre de una capa. En la página Parámetros, seleccione la opción situada junto a cada parámetro que desee añadir. Consulte [Creación de parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

## 4. Publicar plantillas

Al publicar la plantilla, esta se coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar dinámicamente a su sitio web o aplicación. La publicación también activa la URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media hasta su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, marque para publicarla y, en la barra de navegación global, haga clic en **[!UICONTROL Publicar]**. A continuación, haga clic en **[!UICONTROL Enviar publicación]**. Consulte [Publicación de plantillas](publishing-templates.md#publishing_templates).

## 5. Vincular una plantilla a una página web

Dynamic Media Classic crea direcciones URL para plantillas y las activa al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas URL desde la página Vista previa de plantilla .

Seleccione la plantilla en el panel Examinar y, a continuación, haga clic en **[!UICONTROL Vista previa]** para abrir la página Vista previa de plantilla. Elija un ajuste preestablecido de imagen para enviar la plantilla y haga clic en **[!UICONTROL Copiar URL]**. Después de copiar la URL de la página Vista previa, puede utilizarla en su sitio web o aplicación. Consulte [Vinculación de una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
