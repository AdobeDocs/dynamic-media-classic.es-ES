---
title: "Inicio rápido: Funciones básicas de plantilla"
description: Introducción y Inicio rápido de los conceptos básicos de las plantillas para ayudarle a ponerse en marcha rápidamente con Adobe Dynamic Media Classic.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 20%

---

# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Los conceptos básicos de las plantillas se crean dinámicamente y se pueden dirigir mediante archivos de imagen en capas, como los archivos en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático que contenga capas, como un archivo PSD con capas, en una plantilla y crear plantillas en Adobe Dynamic Media Classic. Puede crear capas de texto en plantillas utilizando las fuentes cargadas en Adobe Dynamic Media Classic. Después de agregar texto a una plantilla, puede aplicarle formato cambiando su justificación, fuente, tamaño de fuente y color.

En la página Parámetros, puede convertir cualquier aspecto de una plantilla en un parámetro direccionable. Al hacerlo, puede cambiar qué imagen de capas utilizar o qué valor de texto utilizar en la plantilla. Los parámetros se pasan junto a la cadena URL, lo que le permite cambiar cualquier parámetro para personalizar de forma dinámica la imagen de respuesta generada por el servidor de imágenes.

Consulte también [Conceptos básicos de plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de formación.

Este Inicio rápido está diseñado para ayudarle a ponerse en marcha rápidamente con Conceptos básicos de plantilla.

## 1. Cargue los archivos

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen además de PSD, pero se recomiendan imágenes de TIFF y PNG sin pérdidas para las plantillas porque permiten la transparencia.

Si utiliza un archivo de PSD para crear la plantilla, seleccione **[!UICONTROL Crear plantilla]** en el **[!UICONTROL Opciones del trabajo de carga]** al cargar el archivo del PSD. Elija también una **[!UICONTROL Nombres de capas]** opción para que Adobe Dynamic Media Classic sepa cómo asignar nombres a las capas de PSD cuando se cargan en Adobe Dynamic Media Classic.

Si utiliza archivos de imagen, puede recortar las imágenes y también crear una máscara a partir de trazados de recorte en las imágenes a medida que las carga.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar un archivo de PSD u otros archivos de imagen del equipo en una carpeta de Adobe Dynamic Media Classic. Consulte [Cargar archivos de plantilla](uploading-template-files.md#uploading_template_files).

## 2. Crear una plantilla

Para crear una plantilla a partir de un archivo de PSD, seleccione **[!UICONTROL Crear plantilla]** al cargar el archivo. Para crear una plantilla a partir de imágenes, en la barra de navegación global, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]**, introduzca una medida de anchura y altura para el lienzo. Cerca de la esquina superior derecha de la página, seleccione **[!UICONTROL Designer]** o **[!UICONTROL Desarrollador]** y arrastre imágenes a la página Plantilla. También puede seleccionar las imágenes *antes* vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conceptos básicos de plantilla]**. La página Plantilla ofrece herramientas para lo siguiente:

* Agregar capas de imagen. Para agregar una capa, arrastre una imagen a la página Plantilla.
* Agregar capas de texto. Seleccione el **[!UICONTROL Herramienta Texto]** icono. Arrastre el puntero para crear un cuadro para la capa de texto; a continuación, dé formato al texto con herramientas en la página Texto.
* Cambiar el tamaño y la posición de capas.
* Cambiar el orden de capas.
* Aplicar efectos de sombra y resplandor en capas de imagen y texto.

Consulte [Creación de una plantilla](creating-template.md#creating_a_template).

## 3. Crear parámetros de plantilla

El siguiente paso es la parametrización de las propiedades de capas para determinar qué propiedades se incluyen en la cadena URL. Los parámetros aumentan la flexibilidad de uso de las plantillas. Después de convertir una propiedad de capa en parámetro, se puede cambiar de forma dinámica.

Para parametrizar una capa, abra la plantilla en la página Plantilla y seleccione **[!UICONTROL Parámetros]** junto al nombre de una capa. En la página Parámetros, seleccione la opción situada junto a cada parámetro que desee añadir. Consulte [Crear parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

## 4. Publicar plantillas

La publicación de la plantilla la coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar dinámicamente al sitio web o a la aplicación. La publicación también activa la dirección URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, márquela para publicación y, en la barra de navegación global, seleccione **[!UICONTROL Publish]**. A continuación seleccione **[!UICONTROL Enviar publicación]**. Consulte [Publicar plantillas](publishing-templates.md#publishing_templates).

## 5. Vinculación de una plantilla a una página web

Dynamic Media Classic crea direcciones URL para las plantillas y las activa al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas de URL desde la página Vista previa de plantilla.

Seleccione la plantilla en el panel Examinar y, a continuación, seleccione **[!UICONTROL Previsualizar]** para abrir la página Vista previa de la plantilla. Elija un ajuste preestablecido de imagen para enviar la plantilla y, a continuación, seleccione **[!UICONTROL Copiar URL]**. Una vez copiada la dirección URL de la página de vista previa, puede utilizarla en su sitio web o aplicación. Consulte [Vinculación de una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
