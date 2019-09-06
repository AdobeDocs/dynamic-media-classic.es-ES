---
title: '"Inicio rápido: Funciones básicas de plantilla"'
seo-title: '"Inicio rápido: Funciones básicas de plantilla"'
description: nulo
seo-description: Introducción e Inicio rápido a Funciones básicas de plantilla para ayudarle a empezar a utilizarlo rápidamente.
uuid: 16 d 78 cbb-f 762-4263-aea 9-5712 eb 933693
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: dd 0 fbb 39-3 f 6 a -496 b-a 9 b 6-63 b 11 dcb 823 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Inicio rápido: Funciones básicas de plantilla{#quick-start-template-basics}

Las funciones básicas de plantilla son archivos de imagen con capas creados de forma dinámica, como archivos con capas en aplicaciones de edición de imágenes como Adobe Photoshop. A diferencia de los archivos estáticos que contienen capas (por ejemplo, archivos PSD), una plantilla puede incluir parámetros. A través de parámetros, puede dirigir y personalizar los diferentes aspectos de la imagen.

>[!NOTE]
>
>También puede crear plantillas a partir de diseños basados en maquetaciones mediante Publicación de plantillas y archivos de Adobe Illustrator y Adobe indesign. Consulte [Publicación de plantillas](quick-start-template-publishing.md) .

Una plantilla puede contener un número cualquiera de capas de imagen y capas de texto. Puede convertir un archivo estático con capas, como un archivo PSD de capas, en una plantilla, así como crear plantillas en Dynamic Media Classic. Puede crear capas de texto en plantillas, con fuentes cargadas en SPS. Después de agregar texto a una plantilla, puede modificar las fuentes, el tamaño y el color de éstas y la justificación.

En la pantalla Parámetros puede convertir cualquier aspecto de una plantilla en un parámetro direccionable. De este modo podrá elegir qué imagen de capa o qué valor de texto usar en la plantilla. Los parámetros se pasan junto a la cadena URL, lo que le permite cambiar cualquier parámetro para personalizar de forma dinámica la imagen de respuesta generada por el servidor de imágenes.

**Inicio rápido**

Este inicio rápido se ha diseñado para el uso inicial de Funciones básicas de plantilla. 

**1. Carga de archivos**

Empiece por subir el archivo PSD o archivo de imagen para su plantilla. Dynamic Media Classic admite muchos formatos de archivo de imagen además de PSD, pero se recomiendan imágenes TIFF sin pérdida y PNG para plantillas porque permiten transparencia.

Si va a usar un archivo PSD para crear la plantilla, seleccione la opción Crear plantilla en el cuadro de diálogo Opciones de trabajo de carga cuando cargue el archivo PSD. También elija una opción de Nombre de capa para indicar a Dynamic Media Classic cómo nombrar capas PSD cuando se cargan en Scene 7 Publishing System.

Si utiliza archivos de imagen, puede recortar las imágenes y crear una máscara a partir de ruta de recorte al cargar las imágenes.

Seleccione el botón Cargar en la barra de navegación global para cargar un archivo PSD u otro archivo de imagen desde su ordenador a una carpeta en SPS. Consulte [Carga de archivos de plantilla](uploading-template-files.md#uploading_template_files).

**2. Creación de una plantilla**

Para crear una plantilla a partir de un archivo PSD, seleccione la opción Crear plantilla cuando cargue el archivo. Para crear una plantilla a partir de imágenes, seleccione Generar &gt; Funciones básicas de plantilla, introduzca las medidas de ancho y alto del lienzo, seleccione Diseñador o Desarrollador y arrastre las imágenes a la pantalla Plantilla. También puede seleccionar las imágenes antes de elegir Generar &gt; Funciones básicas de plantilla. En la pantalla Plantilla hay herramientas para:

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

Al publicar la plantilla, ésta se coloca en los servidores de imágenes de Dynamic Media para que se pueda distribuir de forma dinámica en el sitio web o en la aplicación. La publicación también activa la URL para llamar a la plantilla desde los servidores de imágenes de Dynamic Media hasta su sitio web o aplicación.

Debe publicar todas las imágenes asociadas a su plantilla.

Para publicar una plantilla, márquela para publicación y seleccione el botón Publicar en la barra de navegación global. A continuación, seleccione el botón Iniciar publicación. Consulte [Publicación de plantillas](publishing-templates.md#publishing_templates).

**5. Vinculación de una plantilla a una página web**

Dynamic Media Classic crea direcciones URL para plantillas y activa las URL al publicar plantillas en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas URL de la pantalla Vista previa de plantilla.

Seleccione la plantilla en el panel Examinar y, luego, haga clic en el botón Vista previa para abrir la pantalla Vista previa de plantilla. A continuación, elija un ajuste preestablecido de imagen para enviar la plantilla y seleccione el botón Copiar URL. Después de copiar la URL desde la pantalla Vista previa, ésta se podrá usar en el sitio web o en la aplicación. Consulte [Vinculación de una plantilla a una página web](linking-template-web-page.md#linking_a_template_to_a_web_page).
