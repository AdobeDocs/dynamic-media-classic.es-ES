---
title: Uso de archivos PSD
seo-title: Uso de archivos PSD
description: nulo
seo-description: Aprenda a trabajar con archivos PSD.
uuid: 5836 b 660-6 bca -46 e 7-ab 39-1 a 31 d 1 e 0 cff 2
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4086 e 3 db -5 aca -41 a 0-8 f 15-302 afbf 67 ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Uso de archivos PSD{#working-with-psd-files}

Los archivos PSD (Photoshop Document) se utilizan con más frecuencia en Dynamic Media Classic para crear plantillas. Al cargar un archivo PSD, puede crear una plantilla de Media Media Classic automáticamente a partir del archivo (seleccione la opción Crear plantilla en la pantalla Cargar).

SPS crea varias imágenes a partir de un archivo PSD con capas si se usa el archivo para crear una plantilla; crea una imagen para cada capa.

## Opciones de carga de archivos PSD {#psd-upload-options}

Las opciones de carga de archivos PSD están disponibles en Opciones de Photoshop, en la sección Opciones de trabajo de carga. Puede recortar un archivo, elegir un perfil de color para el mismo, usarlo para crear una plantilla y seleccionar un anclaje.

Estas opciones están disponibles al cargar archivos PSD:

**Recorte** (ubicado en Opciones de recorte). Elija Recortar para recortar automáticamente espacio en blanco de los bordes de un archivo PSD; elija Manual para recortar los lados del archivo PSD:

**Recortar** Seleccione el menú Recortar basándose en y elija Color o Transparencia.

Si selecciona la opción Color, seleccione el menú Esquina y elija la esquina del PSD que mejor represente el color de espacio en blanco que desea recortar.

Arrastre el control deslizante para especificar una tolerancia de 0 a 1:

Para un recorte basado en color, especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina del PSD. Los números más cercanos a 1 permiten una mayor diferencia de color.

Para un recorte basado en transparencia, especifique 0 para recortar píxeles solo si son totalmente transparentes; los números más cercanos a 1 permiten una mayor transparencia.

**Manual** Introduzca el número de píxeles que recortar de uno o ambos lados de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, si la imagen muestra 150 ppp y se introduce 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, se recortará media pulgada de cada lado de la imagen.

**Perfil de color** (ubicado en Opciones de perfil de color). Elija una opción:

**Convertir a SRGB (predeterminado)** Convierte a SRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

**Mantener espacio de color original** Conserva el espacio de color original de la imagen.

**Personalizar &gt; Para** abrir menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o uno que haya cargado en SPS. Consulte Perfiles ICC.

**Mantener capas** extrae las capas del PSD, si las hay, en recursos individuales. Las capas de recursos permanecen asociadas al PSD. Para verlas, abra el archivo PSD en la vista de detalles y seleccione el panel de capas. Consulte Visualización y edición de capas de archivos PSD.

**Crear plantilla** Crea una plantilla a partir de las capas del archivo PSD.

**Extraer texto** Extrae el texto para que los usuarios puedan buscar texto en un visor.

**Ampliar capas al tamaño de fondo** Amplía el tamaño de las capas de imagen extraídas al tamaño de la capa de fondo.

**Las capas de nomenclatura** de capas del archivo PSD se cargan como imágenes independientes. Elija una opción para asignar nombres a estas imágenes en Scene7 Publishing System:

**Nombre de capa** Asigna a las imágenes los nombres de sus capas en el archivo PSD. Por ejemplo, una capa con el nombre Etiqueta de precio en el archivo PSD original se convierte en una imagen con el nombre Etiqueta de precio. Sin embargo, si los nombres de capa en el archivo PSD son de forma predeterminada nombres de capa de Photoshop (Fondo, Capa 1, Capa 2, etc), las imágenes recibirán como nombre su número de capa en el archivo PSD, no su nombre de capa predeterminado.

**Número de Photoshop y de capa** Los nombres de las imágenes siguen los números de sus capas en el archivo PSD e ignoran los nombres de capa originales. Las imágenes reciben el nombre del archivo de Photoshop y un sufijo de número de capa. Por ejemplo, la segunda capa de un archivo con el nombre Anuncio primavera.psd recibirá el nombre Anuncio primavera_2 aunque tenga un nombre no predeterminado en Photoshop.

**Nombre de Photoshop y de capa** Nombre las imágenes después del archivo PSD seguido del nombre de capa o del número de capa. El número de capa se utiliza si los nombres de capa en el archivo PSD son nombres de capa predeterminados de Photoshop. Por ejemplo, una capa con el nombre Etiqueta de precio en un archivo PSD con el nombre Anuncio primavera se llamará Anuncio primavera_Etiqueta de precio. Una capa con el nombre predeterminado Capa 2 se llamará Anuncio primavera_2.

**Delimitador** especifique cómo se anclan las imágenes en las plantillas generadas a partir de la composición de capas producida a partir del archivo PSD. De forma predeterminada, el anclaje es al centro. Un anclaje central permite la sustitución de imágenes para rellenar mejor el mismo espacio, independientemente de la proporción de la imagen de sustitución. Las imágenes con una proporción diferente que sustituyan esta imagen, al hacer referencia a la plantilla y usar la sustitución paramétrica, ocuparán el mismo espacio. Cambie a otra configuración si la aplicación requiere que las imágenes de sustitución rellenen el espacio asignado en la plantilla.

## Visualización y edición de capas de archivos PSD {#viewing-and-editing-layers-in-a-psd-file}

Si seleccionó la opción Mantener capas al cargar el PSD, Dynamic Media Classic extrajo las capas individuales en recursos. Puede visualizar y editar las capas de recurso pertenecientes a un archivo PSD abriendo el archivo en el panel Examinar, en la vista de detalles.

1. Haga doble clic en el archivo PSD completo en el panel Examinar para abrirlo en la vista de detalles.

   ***nota**: Asegúrese de abrir el recurso completo y no una de las capas PSD.*

1. Haga clic en Capas para abrir el panel Capas. Todas las capas aparecen como imágenes independientes en el panel Capas.
1. Haga doble clic en una capa para abrirla y realizar cualquiera de las siguientes acciones:

   * Haga clic en el icono Mapa de imagen para crear un mapa de imagen en la capa. (Consulte [Creación de mapas de imagen](creating-image-maps.md#creating_image_maps)).
   * Haga clic en el icono Destinos de zoom para crear destinos de zoom en la capa. (Consulte [Creación de destinos de zoom para zoom guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).
   * Haga clic en el icono Recortar para recortar la capa. (Consulte [Recorte de imágenes](cropping-image.md#cropping_an_image)).
   * Haga clic en Enfocar para enfocar la capa. (Consulte [Enfoque de imágenes](sharpening-image.md#sharpening_an_image)).
   * Haga clic en Ajustar para ajustar la capa. (Consulte [Ajuste de imágenes](adjusting-image.md#adjusting_an_image)).

1. Haga clic en Guardar o Guardar como.
1. Para ver o editar una capa diferente, haga clic en una de las flechas de la parte inferior de la vista previa de la capa.
1. Para salir de la vista de detalles de la capa, haga clic en el icono de vista de cuadrícula.

