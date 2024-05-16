---
title: Crear mapas de imagen de catálogo electrónico
description: Obtenga información sobre cómo crear mapas de imágenes de catálogo electrónico en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 28%

---

# Crear mapas de imagen de catálogo electrónico{#creating-ecatalog-image-maps}

Un mapa de imagen es una región de una página de catálogo electrónico que se puede mover con el ratón o seleccionar para almacenar en déclencheur acciones de distintos tipos. Por ejemplo, cuando se mueve el puntero sobre un mapa de imagen, aparece una descripción de texto de rollover de un elemento. Al seleccionar un mapa de imagen, se inicia otra acción. Por ejemplo, puede abrir una página Web para que los usuarios puedan obtener más información sobre un elemento o comprarlo, o puede iniciar un vídeo para ver un elemento en uso.

## Dibujar mapas de imagen de catálogo electrónico {#drawing-ecatalog-image-maps}

Los mapas de imagen de los catálogos electrónicos se dibujan en la ficha Páginas de mapa, que se encuentra en la pantalla Catálogo electrónico. En esta pantalla aparece el área del mapa de imagen en la que se muestran las páginas del catálogo electrónico y, a la derecha, la lista de mapas de imagen. A medida que crea mapas de imagen, sus nombres se introducen en la lista Mapa de imagen.

1. Seleccione la sustitución del catálogo electrónico **[!UICONTROL Editar]** botón.
1. Seleccionar **[!UICONTROL Páginas de mapa]**.
1. En la parte izquierda de la pantalla Páginas de mapa, seleccione la página que desee.
1. En el área del mapa de imagen, dibuje un mapa de imagen rectangular o poligonal (con varios lados):

   * **Mapa rectangular**: seleccione la herramienta Mapa de imagen de rectángulo y arrastre el cursor sobre la página para crear el rectángulo.

   * **Mapa poligonal**: seleccione la herramienta Mapa de imagen poligonal y, a continuación, seleccione tantas veces como sea necesario alrededor del perímetro de la imagen. A medida que selecciona, Adobe Dynamic Media Classic dibuja los bordes del mapa de imagen.

     Después de dibujar un mapa de imagen, Adobe Dynamic Media Classic le asigna un nombre en la lista Mapa de imagen. Para formar el nombre, Adobe Dynamic Media Classic añade un número secuencial al nombre de la página del catálogo electrónico en la que está trabajando.

1. (Opcional) En la lista Mapa de imágenes, en el [!UICONTROL Nombre] , puede introducir un nuevo nombre para el mapa de imagen. No incluya espacios en blanco en el nombre.
1. Puede hacer que los visualizadores abran una nueva página web cuando seleccionen el mapa de imagen. En el panel de lista Mapa de imagen, introduzca la dirección URL de la página web en la columna URL.

   Para facilitar la introducción de direcciones URL (plantillas Href), seleccione **[!UICONTROL Editar]** e introduzca una plantilla.

Consulte [Utilice una plantilla para introducir JavaScript y direcciones URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Opcional) En la lista desplegable Mostrar, seleccione **[!UICONTROL Texto de rollover]** y, a continuación, escriba el texto que desea que los usuarios vean en pantalla cuando muevan sus punteros sobre el mapa de imagen.
1. (Opcional) En la lista desplegable Mostrar, seleccione **[!UICONTROL Otras acciones]** e introduzca un atributo para almacenar en déclencheur una acción de desenfoque o enfoque cuando los usuarios muevan sus punteros sobre un mapa de imagen.

   Consulte [Definir otras acciones para los mapas de imagen](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Seleccionar **[!UICONTROL Guardar]**.
1. (Opcional) Seleccione **[!UICONTROL Previsualizar]** para ver el catálogo electrónico con el ajuste preestablecido por defecto eCatalog Viewer.

Para eliminar un mapa de imagen, seleccione su nombre en la lista Mapa de imagen y seleccione **[!UICONTROL Eliminar]**. Puede deshabilitar temporalmente un mapa de imagen en una página sin eliminar el mapa de imagen. Seleccione la opción Mapas de imagen activados en el panel de lista Mapa de imagen.

## Incrustar medios enriquecidos en un catálogo electrónico {#embedding-rich-media-in-an-ecatalog}

Puede utilizar la opción Rich Media del catálogo electrónico para agregar vídeos en formato MP4 o conjuntos de giros a mapas de imágenes que haya agregado a un catálogo electrónico. Cuando un usuario selecciona el área de Mapa de imagen en el catálogo electrónico, se muestra el conjunto de giros o vídeo asociado. Esta funcionalidad es especialmente útil si desea que los clientes vean un elemento en uso o vean un elemento desde diferentes ángulos y perspectivas.

También puede mostrar, de forma opcional, el texto de la información del objeto cuando los clientes muevan sus punteros sobre el mapa de imagen para que sepan lo que están seleccionando.

**Para incrustar medios enriquecidos en un catálogo electrónico:**

1. Dibuje un mapa de imagen de catálogo electrónico.

   Consulte [Dibujar mapas de imagen de catálogo electrónico](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. En la lista desplegable Mostrar, seleccione **[!UICONTROL Medios enriquecidos]**.
1. En el panel Agregar recursos en la parte izquierda, navegue hasta la carpeta que contenga el conjunto de giros o el vídeo (formato MP4) que desee incrustar.
1. Arrastre el recurso al mapa de imagen.
1. (Opcional) En el panel de lista Mapa de imagen, en la variable **[!UICONTROL Información de herramienta]** Encabezado de columna, introduzca el texto que desea que los visualizadores vean en pantalla cuando muevan el puntero sobre el mapa de imagen.
1. Seleccionar **[!UICONTROL Guardar]**.

## Edición de mapas de imagen de catálogos electrónicos {#editing-ecatalog-image-maps}

En la pantalla Catálogo electrónico, vaya a la ficha Páginas de mapa, desde donde podrá utilizar estas técnicas para editar los mapas de imagen del catálogo electrónico:

* **Ajuste de la posición**: seleccione la herramienta Panorámica y mueva el puntero cerca del borde del mapa, pero no sobre él. Cuando el puntero muestre una flecha de cuatro puntas, arrastre todo el mapa de imagen a una nueva ubicación.

  Consulte [Ajustar la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Cambiar la forma y el tamaño**: para cambiar el tamaño de un mapa de imagen rectangular, seleccione la herramienta Panorámica. A continuación, mueva el puntero sobre un lado o una esquina y, cuando vea la flecha con dos puntas, arrastre el ratón. Para cambiar el tamaño de un mapa de imagen poligonal, arrastre el ratón para crear un tirador de selección cuadrada. Para crear un controlador de selección, seleccione el borde del mapa de imagen y arrastre.

  Consulte [Ajustar la posición, la forma y el tamaño de los mapas de imagen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Eliminando mapas de imagen**: seleccione la herramienta Panorámica, seleccione el mapa de imagen para seleccionarlo y, a continuación, seleccione **[!UICONTROL Eliminar]**.

  Para eliminar todos los mapas de imagen de un catálogo electrónico, seleccione la **[!UICONTROL Ordenar páginas]** , y luego seleccione **[!UICONTROL Borrar asignaciones]**.

* **Gestión de mapas de imagen superpuestos**: arrastre para cambiar el orden de los mapas de imagen en la lista Mapa de imagen.

  Consulte [Gestión de mapas de imagen superpuestos](creating-image-maps.md#handling_overlapping_image_maps).

* **Copia de mapas de imagen en otras páginas**: Seleccionar **[!UICONTROL Copiar asignaciones en]** (asegúrese de que está en la pestaña Páginas de mapa). En la pantalla Seleccionar imágenes, seleccione la página o páginas en las que desea copiar los mapas de imagen y seleccione **[!UICONTROL Seleccionar]**.

  Consulte [Copiar mapas de imagen en otras imágenes](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Al copiar mapas de imágenes en diferentes páginas de un catálogo electrónico, puede copiar todos los mapas de imágenes de un catálogo electrónico en otro catálogo electrónico. Consulte [Copia de mapas de imagen entre otros catálogos electrónicos](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Revisión e importación de datos de mapa de imagen {#reviewing-and-importing-image-map-data}

En la pantalla Resumen de mapas se pueden ver los metadatos del catálogo electrónico. Desde esta pantalla, también puede importar datos de mapas de imagen por lotes para el catálogo electrónico. Si se importan datos de mapas de imagen de esta forma, será más fácil introducir direcciones URL y texto de rollover para los mapas de imagen.

Para ver la pantalla Resumen de mapas, en la pestaña Páginas de mapa de la pantalla Catálogo electrónico, seleccione **[!UICONTROL Resumen]**.

### Visualización del resumen de datos de mapas de imagen {#review-image-map-data-summary}

1. En la pantalla Asignar páginas, seleccione **[!UICONTROL Resumen]**.

   La pantalla Resumen de mapas muestra cuántos mapas de imágenes, direcciones URL, descripciones de texto de rollover y otras acciones hay en el catálogo electrónico.

1. Si hay errores de clave de rollover, seleccione el error en la **[!UICONTROL Error de Rollover_Key]** para ver qué debe cambiar en la hoja de cálculo y corregir el error. Puede seleccionar y copiar el texto de este mensaje, y pegarlo en la hoja de cálculo.
1. Seleccionar **[!UICONTROL Previsualizar]** para que pueda examinar una página en el Visor de catálogos electrónicos. Seleccione la X para cerrar la pantalla Resumen y volver a la pantalla Páginas de mapa o seleccione **[!UICONTROL Cerrar]** para volver a Examinar.

### Importación de datos de mapa de imagen {#import-image-map-data}

En lugar de introducir datos de mapa de imagen en cada página, puede importar los datos de todo el catálogo desde la pantalla Resumen de mapas. Los datos de mapa de imagen se importan como un archivo delimitado por tabuladores o DTD de XML. Los campos del archivo deben tener el orden que se muestra en la pantalla Resumen de mapas: Nombre, Etiquetas de tabla de contenido, Mapas, Direcciones URL, Texto de rollover, Otras acciones y Cadenas de búsqueda. La importación de datos de mapa de imagen evita tener que introducir los datos en la lista de mapa de imagen a medida que se crea cada mapa de imagen.

>[!NOTE]
>
>Antes de importar estos datos, debe haber creado los mapas de imagen.

Vaya a la pantalla Resumen de mapas y siga estos pasos para importar los datos de mapa de imagen para los mapas de imagen creados:

1. Seleccionar **[!UICONTROL Importar datos de mapa]**.
1. En el cuadro de diálogo Importar metadatos, seleccione **[!UICONTROL Examinar]** y, a continuación, seleccione el archivo DTD XML o delimitado por tabuladores.
1. Escriba el nombre que desea asignar al archivo (mantenga la extensión) en el campo Nombre de trabajo.
1. Seleccionar **[!UICONTROL Cargar]**.

## Copia de mapas de imagen entre otros catálogos electrónicos {#copying-image-maps-between-ecatalogs}

Puede copiar todos los mapas de imagen de un catálogo electrónico a otro. La copia de mapas de imagen con este método es una forma cómoda de copiar los mapas de imagen entre las distintas traducciones en otros idiomas del mismo catálogo electrónico. Para que la copia se realice correctamente, Adobe Dynamic Media Classic recomienda copiar entre catálogos electrónicos con el mismo número de páginas y las mismas imágenes.

>[!NOTE]
>
>si el catálogo electrónico al que copia los mapas de imagen ya contiene otros mapas de imagen, dichos mapas se eliminarán cuando se realice la copia.

Para copiar todos los mapas de imagen de un catálogo electrónico en otro, haga lo siguiente:

1. Seleccione el catálogo electrónico con los mapas de imagen que desee copiar y seleccione la sustitución del catálogo electrónico **[!UICONTROL Editar]** botón.
1. En la pestaña Ordenar páginas, seleccione **[!UICONTROL Copiar asignaciones]**.
1. En el cuadro de diálogo Seleccionar recurso, seleccione el catálogo electrónico en el que desea copiar los mapas de imagen y, a continuación, seleccione **[!UICONTROL Seleccionar]**.

Adobe Dynamic Media Classic muestra un mensaje de advertencia si el catálogo electrónico de destino desde el que copia mapas de imágenes tiene un número diferente de páginas o imágenes con un tamaño diferente. Seleccionar **[!UICONTROL Continuar]** para copiar los mapas de imagen a pesar de la advertencia.
