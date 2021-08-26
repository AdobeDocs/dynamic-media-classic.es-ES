---
title: Creación de mapas de imagen de catálogos electrónicos
description: Aprenda a crear mapas de imágenes de catálogos electrónicos en Adobe Dynamic Media Classic.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 40%

---

# Creación de mapas de imagen de catálogos electrónicos{#creating-ecatalog-image-maps}

Un mapa de imagen es una región de una página de catálogo electrónico que puede pasar el ratón o seleccionar para almacenar en déclencheur acciones de varios tipos. Al mover el puntero sobre un mapa de imagen, por ejemplo, se ve una descripción de un elemento con texto de sustitución. Al seleccionar un mapa de imagen, se inicia otra acción. Por ejemplo, se puede abrir una página web para que los usuarios que la vean puedan obtener más información sobre un elemento o adquirirlo, o bien puede iniciar un vídeo para ver un elemento en uso.

## Dibujar mapas de imagen del catálogo electrónico {#drawing-ecatalog-image-maps}

Los mapas de imagen de los catálogos electrónicos se dibujan en la ficha Páginas de mapa, que se encuentra en la pantalla Catálogo electrónico. En esta pantalla aparece el área del mapa de imagen en la que se muestran las páginas del catálogo electrónico y, a la derecha, la lista de mapas de imagen. A medida que cree los mapas de imagen, sus nombres se añadirán a la lista de mapas de imagen.

1. Seleccione el botón **[!UICONTROL Edit]** de sustitución del catálogo electrónico.
1. Seleccione **[!UICONTROL Páginas de mapa]**.
1. En la parte izquierda de la pantalla Páginas de mapa, seleccione la página que desee.
1. En el área del mapa de imagen, dibuje un mapa de imagen rectangular o poligonal (con varios lados):

   * **Mapa rectangular** : seleccione la herramienta Mapa de imagen rectangular y arrastre la página para crear el rectángulo.

   * **Mapa poligonal** : seleccione la herramienta Mapa de imagen poligonal y, a continuación, seleccione tantas veces como sea necesario alrededor del perímetro de la imagen. Mientras selecciona, Adobe Dynamic Media Classic dibuja los bordes del mapa de imagen.

      Después de dibujar un mapa de imagen, Adobe Dynamic Media Classic le asigna un nombre en la lista Mapa de imagen. Para formar el nombre, Adobe Dynamic Media Classic añade un número secuencial al nombre de la página del catálogo electrónico en la que está trabajando.

1. (Opcional) En la lista Mapa de imágenes, en la columna [!UICONTROL Nombre], puede introducir un nuevo nombre para el Mapa de imágenes. No incluya espacios en blanco en el nombre.
1. Puede hacer que los visualizadores abran una nueva página web cuando seleccionen el mapa de imagen. En el panel de lista de mapas de imagen, introduzca la dirección URL de la página web en la columna URL.

   Para facilitar la introducción de direcciones URL (plantillas Href), seleccione **[!UICONTROL Editar]** e introduzca una plantilla.

Consulte [Uso de una plantilla para introducir JavaScript y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Opcional) En la lista desplegable Mostrar , seleccione **[!UICONTROL Texto de sustitución]** e introduzca el texto que desea que vean los usuarios en pantalla cuando desplacen sus punteros por el mapa de imagen.
1. (Opcional) En la lista desplegable Mostrar , seleccione **[!UICONTROL Otras acciones]** e introduzca un atributo para crear un déclencheur de una acción de enfoque o desenfoque cuando los usuarios muevan sus punteros sobre un mapa de imagen.

   Consulte [Definir otras acciones para mapas de imágenes](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Seleccione **[!UICONTROL Guardar]**.
1. (Opcional) Seleccione **[!UICONTROL Preview]** para ver el catálogo electrónico con el ajuste preestablecido predeterminado del visor de catálogos electrónicos.

Para eliminar un mapa de imagen, seleccione su nombre en la lista Mapa de imagen y seleccione **[!UICONTROL Eliminar]**. Si desea eliminar de forma temporal un mapa de imagen dentro de la página y no borrarlo definitivamente, desactive la opción Activado del mapa de imagen en la lista de mapas de imagen.

## Incrustar medios enriquecidos en un catálogo electrónico {#embedding-rich-media-in-an-ecatalog}

Puede utilizar la opción de medios enriquecidos de catálogo electrónico para agregar vídeos en formato MP4 o conjuntos de giros a mapas de imagen que se hayan añadido a un catálogo electrónico. Cuando un usuario selecciona el área de mapa de imagen en el catálogo electrónico, se muestra el conjunto de giros o vídeo asociado. Esta funcionalidad es especialmente útil si desea que los clientes vean un elemento en uso o vean un elemento desde diferentes ángulos y perspectivas.

También puede mostrar de forma opcional información sobre herramientas cuando los clientes muevan sus punteros sobre el mapa de imagen para que sepan lo que están seleccionando.

**Para incrustar medios enriquecidos en un catálogo electrónico:**

1. Dibuje un mapa de imagen de catálogo electrónico.

   Consulte [Dibujar mapas de imagen del catálogo electrónico](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. En la lista desplegable Mostrar , seleccione **[!UICONTROL Medios enriquecidos]**.
1. En el panel Agregar recursos en la parte izquierda, navegue hasta la carpeta que contenga el conjunto de giros o el vídeo (formato MP4) que desee incrustar.
1. Arrastre el recurso al mapa de imagen.
1. (Opcional) En el panel de lista Mapa de imágenes, en el encabezado de columna **[!UICONTROL Información del objeto]**, introduzca el texto que desea que vean los visualizadores en pantalla cuando desplacen el puntero sobre el Mapa de imágenes.
1. Seleccione **[!UICONTROL Guardar]**.

## Edición de mapas de imagen de catálogos electrónicos {#editing-ecatalog-image-maps}

En la pantalla Catálogo electrónico, vaya a la ficha Páginas de mapa, desde donde podrá utilizar estas técnicas para editar los mapas de imagen del catálogo electrónico:

* **Ajustar la posición** : seleccione la herramienta Panorámica y mueva el puntero cerca del borde del mapa, pero no más allá de él. Cuando el puntero se convierta en una flecha con cuatro puntas, arrastre el mapa completo de imagen a una nueva ubicación.

   Consulte [Ajuste de la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Cambiar la forma y el tamaño** : para cambiar el tamaño de un mapa de imagen rectangular, seleccione la herramienta Panorámica. A continuación, mueva el puntero sobre un lado o una esquina y, cuando vea la flecha con dos puntas, arrastre el ratón. Para cambiar el tamaño de un mapa de imagen poligonal, arrastre el ratón para crear un tirador de selección cuadrada. Para crear un controlador de selección, seleccione el borde del mapa de imagen y arrastre.

   Consulte [Ajuste de la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminación de mapas de imagen** : seleccione la herramienta Panorámica, seleccione el mapa de imagen para seleccionarlo y, a continuación, seleccione  **[!UICONTROL Eliminar]**.

   Para eliminar todos los mapas de imagen de un catálogo electrónico, seleccione la pestaña **[!UICONTROL Ordenar páginas]** y, a continuación, seleccione **[!UICONTROL Borrar mapas]**.

* **Gestión de mapas de imagen superpuestos** : arrastre para cambiar el orden de los mapas de imagen en la lista de mapas de imagen.

   Consulte [Gestión de mapas de imagen superpuestos](creating-image-maps.md#handling_overlapping_image_maps).

* **Copia de mapas de imagen a otras páginas** : seleccione  **[!UICONTROL Copiar asignaciones a]**  (asegúrese de que está en la ficha Páginas de mapa). En la pantalla Seleccionar imágenes, seleccione la página o páginas donde desee copiar los mapas de imagen y seleccione **[!UICONTROL Seleccionar]**.

   Consulte [Copiar mapas de imagen a otras imágenes](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Además de copiar mapas de imagen en diferentes páginas de un catálogo electrónico, puede copiar todos los mapas de imagen de un catálogo electrónico en otro. Consulte [Copiar mapas de imagen entre catálogos electrónicos](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Revisar e importar datos de mapa de imagen {#reviewing-and-importing-image-map-data}

En la pantalla Resumen de mapas se pueden ver los metadatos del catálogo electrónico. Desde esta pantalla, también puede importar datos de mapas de imagen por lotes para el catálogo electrónico. Si se importan datos de mapas de imagen de esta forma, será más fácil introducir direcciones URL y texto de rollover para los mapas de imagen.

Para ver la pantalla Resumen de mapa , en la ficha Páginas de mapa de la pantalla Catálogo electrónico, seleccione **[!UICONTROL Resumen]**.

### Visualización del resumen de datos de mapas de imagen {#review-image-map-data-summary}

1. En la pantalla Páginas de mapa, seleccione **[!UICONTROL Resumen]**.

   En la pantalla Resumen de mapas, se puede ver la cantidad de mapas de imagen, direcciones URL, textos descriptivos de rollover y otras acciones que hay en el catálogo electrónico.

1. Si hay errores de teclas de prórroga, seleccione el error en la columna **[!UICONTROL Rollover_Key Error]** para ver qué debe cambiar en la hoja de cálculo para corregir el error. Puede seleccionar y copiar el texto de este mensaje, y pegarlo en la hoja de cálculo.
1. Seleccione **[!UICONTROL Preview]** para que pueda examinar una página en el visor del catálogo electrónico; seleccione la X para cerrar la pantalla Resumen y volver a la pantalla Páginas de mapa o seleccione **[!UICONTROL Cerrar]** para volver a Examinar.

### Importación de datos de mapa de imagen {#import-image-map-data}

En lugar de introducir datos de mapa de imagen en cada página, puede importar los datos de todo el catálogo desde la pantalla Resumen de mapas. Los datos de mapa de imagen se importan como un archivo delimitado por tabuladores o DTD de XML. Los campos del archivo deben tener el orden que se muestra en la pantalla Resumen de mapas: Nombre, Etiquetas de tabla de contenido, Mapas, Direcciones URL, Texto de rollover, Otras acciones y Cadenas de búsqueda. Si importa los datos de mapa de imagen, no tendrá que introducir los datos en la lista de mapas de imagen cada vez que crea un mapa de imagen.

>[!NOTE]
>
>Antes de importar estos datos, debe haber creado los mapas de imagen.

Vaya a la pantalla Resumen de mapas y siga estos pasos para importar los datos de mapa de imagen para los mapas de imagen creados:

1. Seleccione **[!UICONTROL Importar datos de mapa]**.
1. En el cuadro de diálogo Importar metadatos, seleccione **[!UICONTROL Examinar]** y, a continuación, seleccione el archivo DTD XML o delimitado por tabulaciones.
1. Escriba el nombre que desea asignar al archivo (mantenga la extensión) en el campo Nombre de trabajo.
1. Seleccione **[!UICONTROL Upload]**.

## Copia de mapas de imagen entre catálogos electrónicos {#copying-image-maps-between-ecatalogs}

Puede copiar todos los mapas de imagen de un catálogo electrónico a otro. La copia de mapas de imagen con este método es una forma cómoda de copiar los mapas de imagen entre las distintas traducciones en otros idiomas del mismo catálogo electrónico. Para que la copia sea correcta, el Adobe de Adobe Dynamic Media Classic recomienda copiar entre catálogos electrónicos con el mismo número de páginas y las mismas imágenes.

>[!NOTE]
>
>si el catálogo electrónico al que copia los mapas de imagen ya contiene otros mapas de imagen, dichos mapas se eliminarán cuando se realice la copia.

Para copiar todos los mapas de imagen de un catálogo electrónico en otro, haga lo siguiente:

1. Seleccione el catálogo electrónico con los mapas de imagen que desea copiar y seleccione el botón de rollover **[!UICONTROL Edit]** del catálogo electrónico.
1. En la ficha Ordenar páginas, seleccione **[!UICONTROL Copiar mapas]**.
1. En el cuadro de diálogo Seleccionar recurso, seleccione el catálogo electrónico en el que desea copiar los mapas de imagen y, a continuación, seleccione **[!UICONTROL Seleccionar]**.

Adobe Dynamic Media Classic muestra un mensaje de advertencia si el Catálogo electrónico de destino (el Catálogo electrónico al que copia los Mapas de imagen) tiene un número diferente de páginas o imágenes con un tamaño diferente. Seleccione **[!UICONTROL Continue]** para copiar los mapas de imagen a pesar de la advertencia.
