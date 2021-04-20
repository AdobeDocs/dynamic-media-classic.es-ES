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
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 71%

---


# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Los conceptos básicos de plantilla son archivos de imagen en capas que se pueden dirigir y crear de forma dinámica, como archivos en capas en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático que contenga capas, como un archivo PSD en capas, en una plantilla, así como crear plantillas en Dynamic Media Classic. Puede crear capas de texto en plantillas utilizando las fuentes cargadas en Dynamic Media Classic. Después de agregar texto a una plantilla, puede modificar las fuentes, el tamaño y el color de éstas y la justificación.

En la pantalla Parámetros puede convertir cualquier aspecto de una plantilla en un parámetro direccionable. De este modo podrá elegir qué imagen de capa o qué valor de texto usar en la plantilla. Los parámetros se pasan junto a la cadena URL, lo que le permite cambiar cualquier parámetro para personalizar de forma dinámica la imagen de respuesta generada por el servidor de imágenes.

**Inicio rápido**

Este inicio rápido se ha diseñado para el uso inicial de Funciones básicas de plantilla. 

**1. Carga de archivos**

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Dynamic Media Classic admite muchos formatos de archivo de imagen además de PSD, pero las imágenes TIFF y PNG sin pérdida se recomiendan para las plantillas porque permiten la transparencia.

Si va a usar un archivo PSD para crear la plantilla, seleccione la opción Crear plantilla en el cuadro de diálogo Opciones de trabajo de carga cuando cargue el archivo PSD. Elija también una opción de nomenclatura de capas para indicar a Dynamic Media Classic cómo asignar nombres a las capas PSD cuando se cargan en Dynamic Media Classic.

Si utiliza archivos de imagen, puede recortar las imágenes y crear una máscara a partir de ruta de recorte al cargar las imágenes.

Seleccione el botón Cargar en la barra de navegación global para cargar un archivo PSD u otros archivos de imagen desde el equipo a una carpeta de Dynamic Media Classic. Consulte [Carga de archivos de plantilla](uploading-template-files.md#uploading_template_files).

**2. Creación de una plantilla**

Para crear una plantilla a partir de un archivo PSD, seleccione la opción Crear plantilla cuando cargue el archivo. Para crear una plantilla a partir de imágenes, seleccione Generar > Funciones básicas de plantilla, introduzca las medidas de ancho y alto del lienzo, seleccione Diseñador o Desarrollador y arrastre las imágenes a la pantalla Plantilla. También puede seleccionar las imágenes antes de elegir Generar > Funciones básicas de plantilla. En la pantalla Plantilla hay herramientas para:

* Agregar capas de imagen. Para agregar una capa, arrastre una imagen a la pantalla Plantilla.
* Agregar capas de texto. Seleccione la herramienta de texto  y arrastre el ratón para dibujar un cuadro para la capa de texto; a continuación, utilice las herramientas disponibles en la pantalla de texto para aplicar formato.
* Cambiar el tamaño y la posición de capas.
* Cambiar el orden de capas.
* Aplicar efectos de sombra y resplandor en capas de imagen y texto.

Consulte [Creación de una plantilla](creating-template.md#creating_a_template).

**3. Creación de los parámetros de plantilla**

El siguiente paso es la parametrización de las propiedades de capas para determinar qué propiedades se incluyen en la cadena URL. Los parámetros aumentan la flexibilidad de uso de las plantillas. Después de convertir una propiedad de capa en parámetro, se puede cambiar de forma dinámica.

Para parametrizar una capa, abra la plantilla en la pantalla Plantilla y seleccione el botón Parámetros junto al nombre de una capa. En la pantalla Parámetros, seleccione la opción correspondiente a cada parámetro que desee agregar. Consulte [Creación de parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

**4. Publicación de plantillas**

Al publicar la plantilla, esta se coloca en los servidores de imágenes de Dynamic Media para que se pueda enviar dinámicamente a su sitio web o aplicación. La publicación también activa la URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media hasta su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, márquela para publicación y seleccione el botón Publicar en la barra de navegación global. A continuación, seleccione el botón Iniciar publicación. Consulte [Publicación de plantillas](publishing-templates.md#publishing_templates).

**5. Vinculación de una plantilla a una página web**

Dynamic Media Classic crea direcciones URL para plantillas y las activa al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas URL de la pantalla Vista previa de plantilla.

Seleccione la plantilla en el panel Examinar y, luego, haga clic en el botón Vista previa para abrir la pantalla Vista previa de plantilla. A continuación, elija un ajuste preestablecido de imagen para enviar la plantilla y seleccione el botón Copiar URL. Después de copiar la URL desde la pantalla Vista previa, ésta se podrá usar en el sitio web o en la aplicación. Consulte [Vinculación de una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
