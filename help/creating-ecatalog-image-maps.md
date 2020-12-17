---
title: Creación de mapas de imagen de catálogos electrónicos
seo-title: Creación de mapas de imagen de catálogos electrónicos
description: nulo
seo-description: Obtenga información sobre cómo crear mapas de imagen de catálogos electrónicos.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 77%

---


# Creación de mapas de imagen de catálogos electrónicos{#creating-ecatalog-image-maps}

Un mapa de imagen es una región dentro de una página del catálogo electrónico sobre la que se puede pasar el ratón o hacer clic para activar varios tipos de acciones. Al mover el puntero sobre un mapa de imagen se ve, por ejemplo, un texto de rollover en el que se describe un elemento. Al hacer clic en un mapa de imagen, se inicia otra acción. Por ejemplo, se puede abrir una página web para que los usuarios que la vean puedan obtener más información sobre un elemento o adquirirlo, o bien puede iniciar un vídeo para ver un elemento en uso.

## Dibujo de mapas de imagen de catálogos electrónicos  {#drawing-ecatalog-image-maps}

Los mapas de imagen de los catálogos electrónicos se dibujan en la ficha Páginas de mapa, que se encuentra en la pantalla Catálogo electrónico. En esta pantalla aparece el área del mapa de imagen en la que se muestran las páginas del catálogo electrónico y, a la derecha, la lista de mapas de imagen. A medida que cree los mapas de imagen, sus nombres se añadirán a la lista de mapas de imagen.

1. Haga clic en el botón de rollover Editar del catálogo electrónico.
1. Haga clic en **Páginas de mapa**.
1. En la parte izquierda de la pantalla Páginas de mapa, seleccione la página que desee.
1. En el área del mapa de imagen, dibuje un mapa de imagen rectangular o poligonal (con varios lados):

   * **Mapa rectangular**
Seleccione la herramienta Mapa de imagen rectangular y arrastre la página para crear el rectángulo.

   * **Mapa poligonalSeleccione la herramienta Mapa de imagen poligonal y haga clic tantas veces como sea necesario alrededor del perímetro de la imagen.**
Al hacer clic, Dynamic Media Classic dibuja los bordes del mapa de imagen.
   Después de dibujar un mapa de imagen, Dynamic Media Classic le asigna un nombre en la lista de mapa de imagen. Para formar el nombre, Dynamic Media Classic anexa un número secuencial al nombre de la página del catálogo electrónico en la que está trabajando.

1. (Opcional) En el panel de lista de mapas de imagen, en la columna Nombre, introduzca un nuevo nombre para el mapa de imagen. No incluya espacios en blanco en el nombre.
1. Puede hacer que los visores abran una página web nueva cuando se haga clic en el mapa de imagen. En el panel de lista de mapas de imagen, introduzca la dirección URL de la página web en la columna URL.

   Haga clic en Editar e introduzca una plantilla para facilitar la introducción de direcciones URL (plantillas href).

   Consulte [Uso de plantillas para introducir elementos de JavaScript y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Opcional) En la lista desplegable Mostrar, haga clic en **Texto de rollover** y, a continuación, escriba el texto que desea que vean los usuarios en pantalla cuando muevan sus punteros sobre el mapa de imagen.
1. (Opcional) En la lista desplegable Mostrar, haga clic en **Otras acciones** e introduzca un atributo para activar una acción de enfoque o desenfoque cuando los usuarios muevan el puntero sobre un mapa de imagen.

   Consulte [Definición de otras acciones para los mapas de imagen](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Haga clic en **Guardar**.
1. (Opcional) Haga clic en **Previsualización** para vista del catálogo electrónico con el ajuste preestablecido de visor de catálogos electrónicos predeterminado.

Si desea eliminar un mapa de imagen, seleccione su nombre en la lista de mapas de imagen y haga clic en Eliminar. Si desea eliminar de forma temporal un mapa de imagen dentro de la página y no borrarlo definitivamente, desactive la opción Activado del mapa de imagen en la lista de mapas de imagen.

## Incrustación de medios enriquecidos en un catálogo electrónico  {#embedding-rich-media-in-an-ecatalog}

Puede utilizar la opción de medios enriquecidos de catálogo electrónico para agregar vídeos en formato MP4 o conjuntos de giros a mapas de imagen que se hayan añadido a un catálogo electrónico. Cuando un usuario hace clic en el área de mapa de imagen en el catálogo electrónico, se abre el vídeo o conjunto de giros asociado. Esta funcionalidad es especialmente útil si desea que los clientes vean un elemento en uso o vean un elemento desde diferentes ángulos y perspectivas.

Opcionalmente, también puede mostrar texto de información sobre herramientas cuando los clientes muevan el cursor sobre el mapa de imagen para que puedan saber en qué elemento están haciendo clic.

**Para incrustar medios enriquecidos en un catálogo electrónico**

1. Dibuje un mapa de imagen de catálogo electrónico.

   Consulte [Dibujo de mapas de imagen de catálogos electrónicos](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. En la lista desplegable Mostrar, seleccione Medios enriquecidos.
1. En el panel Agregar recursos en la parte izquierda, navegue hasta la carpeta que contenga el conjunto de giros o el vídeo (formato MP4) que desee incrustar.
1. Arrastre el recurso al mapa de imagen.
1. (Opcional) En el panel de lista de mapas de imagen, en el encabezado de columna Información sobre herramientas, introduzca el texto que desee que vean en pantalla los usuarios cuando muevan el puntero sobre el mapa de imagen.
1. Haga clic en Guardar.

## Edición de mapas de imagen de catálogos electrónicos {#editing-ecatalog-image-maps}

En la pantalla Catálogo electrónico, vaya a la ficha Páginas de mapa, desde donde podrá utilizar estas técnicas para editar los mapas de imagen del catálogo electrónico:

* **Ajuste de la**
posiciónSeleccione la herramienta de desplazamiento y mueva el puntero cerca del borde del mapa, pero no sobre él. Cuando el puntero se convierta en una flecha con cuatro puntas, arrastre el mapa completo de imagen a una nueva ubicación.

   Consulte [Ajuste de la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Cambio de la forma y el**
tamañoPara cambiar el tamaño de un mapa de imagen rectangular, seleccione la herramienta de desplazamiento. A continuación, mueva el puntero sobre un lado o una esquina y, cuando vea la flecha con dos puntas, arrastre el ratón. Para cambiar el tamaño de un mapa de imagen poligonal, arrastre el ratón para crear un tirador de selección cuadrada. Para crear un tirador de selección, haga clic en el borde del mapa de imagen y arrastre el ratón.

   Consulte [Ajuste de la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminación de**
mapas de imagenSeleccione la herramienta de desplazamiento, haga clic en el mapa de imagen para seleccionarlo y, a continuación, haga clic en 
**Eliminar**.

   Para eliminar todos los mapas de imagen de un catálogo electrónico, haga clic en la ficha **Ordenar páginas** y, a continuación, haga clic en **Borrar mapas**.

* **Gestión de**
mapas de imagen superpuestosArrastre para cambiar el orden de los mapas de imagen en la lista de mapa de imagen.

   Consulte [Control de superposición de mapas de imagen](creating-image-maps.md#handling_overlapping_image_maps).

* **Copia de mapas de imagen a otras**
páginasSeleccione el botón Copiar mapas a (asegúrese de que está en la ficha Páginas de mapa). En la pantalla Seleccionar imágenes, seleccione la página o páginas en las que quiere copiar los mapas de imagen y haga clic en el botón Seleccionar.

   Consulte [Copia de mapas de imagen a otras imágenes](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Además de copiar mapas de imagen a otras páginas del catálogo electrónico, puede copiar todos los mapas de imagen de un catálogo electrónico a otro. Consulte [Copia de mapas de imagen entre catálogos electrónicos](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Revisión e importación de datos de mapa de imagen  {#reviewing-and-importing-image-map-data}

En la pantalla Resumen de mapas se pueden ver los metadatos del catálogo electrónico. Desde esta pantalla, también puede importar datos de mapas de imagen por lotes para el catálogo electrónico. Si se importan datos de mapas de imagen de esta forma, será más fácil introducir direcciones URL y texto de rollover para los mapas de imagen.

Para ver la pantalla Resumen de mapas, en la ficha Páginas de mapa de la pantalla Catálogo electrónico haga clic en Resumen.

### Visualización del resumen de datos de mapas de imagen  {#review-image-map-data-summary}

1. En la pantalla Páginas de mapa, haga clic en Resumen.

   En la pantalla Resumen de mapas, se puede ver la cantidad de mapas de imagen, direcciones URL, textos descriptivos de rollover y otras acciones que hay en el catálogo electrónico.

1. Si hay errores de tecla de rollover, haga clic en el error en la columna de error Rollover_Key para ver qué se debe cambiar en la hoja de cálculo y corregir el error. Puede seleccionar y copiar el texto de este mensaje, y pegarlo en la hoja de cálculo.
1. Haga clic en Vista previa para examinar la página en el visor de catálogos electrónicos, haga clic en X para cerrar la pantalla Resumen y volver a la pantalla Páginas de mapa o haga clic en Cerrar para volver a Examinar.

### Importación de datos de mapa de imagen  {#import-image-map-data}

En lugar de introducir datos de mapa de imagen en cada página, puede importar los datos de todo el catálogo desde la pantalla Resumen de mapas. Los datos de mapa de imagen se importan como un archivo delimitado por tabuladores o DTD de XML. Los campos del archivo deben tener el orden que se muestra en la pantalla Resumen de mapas: Nombre, Etiquetas de tabla de contenido, Mapas, Direcciones URL, Texto de rollover, Otras acciones y Cadenas de búsqueda. Si importa los datos de mapa de imagen, no tendrá que introducir los datos en la lista de mapas de imagen cada vez que crea un mapa de imagen.

>[!NOTE]
>
>Antes de importar estos datos, debe haber creado los mapas de imagen.

Vaya a la pantalla Resumen de mapas y siga estos pasos para importar los datos de mapa de imagen para los mapas de imagen creados:

1. Haga clic en Importar datos de mapa.
1. En el cuadro de diálogo Importar metadatos, haga clic en Examinar y, a continuación, seleccione el archivo DTD de XML o delimitado por tabuladores.
1. Escriba el nombre que desea asignar al archivo (mantenga la extensión) en el campo Nombre de trabajo.
1. Haga clic en Cargar.

## Copia de mapas de imagen entre catálogos electrónicos  {#copying-image-maps-between-ecatalogs}

Puede copiar todos los mapas de imagen de un catálogo electrónico a otro. La copia de mapas de imagen con este método es una forma cómoda de copiar los mapas de imagen entre las distintas traducciones en otros idiomas del mismo catálogo electrónico. Para que la copia sea correcta, Dynamic Media Classic recomienda copiar entre catálogos electrónicos con el mismo número de páginas y las mismas imágenes.

>[!NOTE]
>
>si el catálogo electrónico al que copia los mapas de imagen ya contiene otros mapas de imagen, dichos mapas se eliminarán cuando se realice la copia.

Siga estos pasos para copiar todos los mapas de imagen de un catálogo electrónico a otro:

1. Seleccione el catálogo electrónico que contenga los mapas de imagen que desea copiar y haga clic en el botón de rollover Editar del catálogo electrónico.
1. En la ficha Ordenar páginas, haga clic en Copiar mapas.
1. En el cuadro de diálogo Seleccionar recurso, elija el catálogo electrónico en el que desea copiar los mapas de imagen y haga clic en Seleccionar.

Dynamic Media Classic muestra un mensaje de advertencia si el catálogo electrónico de destinatario (el catálogo electrónico al que se copian los mapas de imagen) tiene un número diferente de páginas o imágenes con un tamaño diferente. Puede hacer clic en Continuar si desea copiar los mapas de imagen a pesar de la advertencia.
