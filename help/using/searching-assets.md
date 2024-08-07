---
title: Buscar recursos de Dynamic Media Classic
description: Obtenga información sobre cómo buscar recursos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 17%

---

# Búsqueda de recursos en Adobe Dynamic Media Classic{#searching-assets}

Para localizar recursos de archivo en Adobe Dynamic Media Classic, puede ver los recursos por tipo, ordenarlos en el panel Examinar, realizar una búsqueda sencilla, realizar una búsqueda avanzada y filtrar los recursos.

>[!NOTE]
>
>La página Configuración personal ofrece opciones para elegir cómo desea llevar a cabo las búsquedas. Por ejemplo, puede elegir un tipo de búsqueda predeterminado e indicar si desea incluir campos definidos por el usuario en las búsquedas. Para obtener más información, consulte [Ajustes personales](personal-setup.md#personal_setup).

## Ver recursos por tipo {#viewing-assets-by-type}

Para ver sólo los archivos de un tipo determinado mientras explora, en la biblioteca de recursos del lado izquierdo, en la lista desplegable **[!UICONTROL Mostrar]**, elija un tipo de archivo. En la biblioteca de recursos solo aparecen los recursos del tipo que ha elegido mostrar.

>[!NOTE]
>
>Si no ve el panel Biblioteca de recursos en el lado izquierdo, haga clic en la flecha triangular derecha del lado izquierdo, a mitad de camino por la ventana de Dynamic Media Classic, para abrir la Biblioteca de recursos.

## Ordenar archivos en el panel Examinar {#sorting-files-in-the-browse-panel}

Puede ordenar el contenido de una carpeta o los resultados de búsqueda que aparecen en el panel Examinar de la derecha. En la barra de navegación global, seleccione **[!UICONTROL Ordenar]** y, a continuación, elija una opción. Las opciones son **[!UICONTROL Nombre]**, **[!UICONTROL Tamaño (KB)]**, **[!UICONTROL Tipo]**, **[!UICONTROL Fecha de creación]** y **[!UICONTROL Última modificación]**.

También puede elegir **[!UICONTROL Ascendente]** o **[!UICONTROL Descendente]** para ordenar los recursos en orden ascendente o descendente según los criterios que elija.

En Vista de lista, puede ordenar seleccionando un nombre de columna.

## Búsqueda sencilla {#conducting-a-simple-search}

Utilice el campo Buscar de la biblioteca de recursos para realizar búsquedas sencillas. Puede buscar elementos por nombre o buscar los elementos cuyos metadatos contengan una palabra clave determinada. 

1. En la Biblioteca de recursos, en el panel **[!UICONTROL Carpetas]**, seleccione la carpeta en la que buscar en una carpeta concreta y sus subcarpetas.
1. A la izquierda del campo Buscar en la Biblioteca de recursos, seleccione el icono **[!UICONTROL Lupa]** para abrir la lista desplegable.
1. En la lista desplegable, elija una opción que describa lo estrecha o amplia que desea que sea la búsqueda. Puede elegir **[!UICONTROL En todos los archivos y carpetas]**, **[!UICONTROL En la carpeta seleccionada]** o **[!UICONTROL En la carpeta y subcarpetas seleccionadas]**.
1. En el campo Buscar, introduzca un término de búsqueda.
1. A la derecha del campo Buscar, selecciona **[!UICONTROL Ir]** o pulsa **[!UICONTROL Entrar]**.

   Los resultados de la búsqueda aparecen en el panel Examinar de la derecha.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Búsqueda avanzada {#conducting-an-advanced-search}

En la Biblioteca de recursos, directamente debajo del campo Buscar, seleccione **[!UICONTROL Búsqueda avanzada]** para buscar según muchos criterios, incluidos los valores de los campos de metadatos.

Especifique cualquiera de los siguientes criterios en la búsqueda avanzada:

* **Filtrar por tipo de recurso**: Reduzca la búsqueda a un solo tipo de recurso. Elija un tipo de recurso en el menú.

* **Archivos y carpetas**: Elija dónde desea buscar: **[!UICONTROL En todos los archivos y carpetas]**, **[!UICONTROL En la carpeta seleccionada]** o **[!UICONTROL En las carpetas y subcarpetas seleccionadas]**.

* **Todos los estados de publicación**: busque los archivos marcados como listos para publicación, no marcados como listos para publicación o todos los archivos.

* **Condiciones**: si especifica criterios de metadatos para la búsqueda, seleccione si la búsqueda debe coincidir con todas las condiciones (una búsqueda ALL) o con cualquier condición (una búsqueda OR).

* **Criterios de búsqueda**: Cree uno o más campos de búsqueda para buscar metadatos. Para crear campos de búsqueda:

   1. En Búsqueda avanzada, bajo el encabezado **[!UICONTROL Criterios de búsqueda]** y a la izquierda del menú **[!UICONTROL Agregar un campo]**), seleccione el icono de flecha de triángulo hacia abajo para abrir la lista desplegable. Elija una vista de metadatos. Puede elegir **[!UICONTROL Todas las propiedades con valores]**, **[!UICONTROL Vista compacta]**, **[!UICONTROL IPTC]**, **[!UICONTROL Campos Publish XMP del servidor de metadatos]** o ****.
   1. Seleccione el menú desplegable **[!UICONTROL Agregar un campo]** y elija un nombre de campo.
   1. Elija una opción **[!UICONTROL Contains]**: **[!UICONTROL Contains]**, **[!UICONTROL Does Not Contain]**, **[!UICONTROL Begins With]**, **[!UICONTROL Ends With]** o **[!UICONTROL Equals]**.
   1. En el caso de los campos numéricos, elija un valor o introduzca un intervalo de fechas personalizado.
   1. (Opcional) Repita los pasos del 1 al 4 para crear más campos de búsqueda.

Seleccione el icono **[!UICONTROL Quitar un campo de búsqueda]** (círculo con &quot;X&quot; dentro) para que se elimine el campo de búsqueda.

En la esquina inferior derecha del panel Búsqueda avanzada, selecciona **[!UICONTROL Buscar]** para comenzar la búsqueda. Los resultados de la búsqueda aparecen en el panel Examinar de la derecha. Puede cambiar cualquier condición de búsqueda y seleccionar **[!UICONTROL Buscar]** para volver a ejecutar la búsqueda.

Seleccione **[!UICONTROL Borrar]** si desea borrar los criterios de búsqueda e iniciar una nueva búsqueda. Seleccione **[!UICONTROL Cerrar]** cuando termine de buscar para cerrar el panel Buscar.

## Filtrado de recursos con metadatos {#filter-assets-using-metadata}

Filtre recursos en la ficha Filtros de la Biblioteca de recursos. Para filtrar recursos, utilice valores de metadatos como criterios. Después de elegir un campo de metadatos por el que filtrar, la pestaña Filtros muestra todos los valores de metadatos introducidos en el campo elegido. También indica el número de recursos que se asignaron a cada valor. Por ejemplo, en una operación de filtrado en el campo de metadatos **[!UICONTROL Creador]**, la pestaña **[!UICONTROL Filtros]** enumera todos los nombres que se han introducido en el campo de metadatos **[!UICONTROL Creador]** para diferentes recursos. También muestra para cada nombre, el número de recursos asignados al nombre. A continuación, seleccione un valor de metadatos para ver todos los recursos a los que se ha asignado ese valor. En el ejemplo, selecciona el valor de metadatos `Prairie Cat` para ver todos los recursos en los que se especificó el nombre `Prairie Cat` en el campo de metadatos **[!UICONTROL Creador]**. Puede filtrar utilizando más de un campo de metadatos como criterio de filtro.

Puede guardar operaciones de filtro para ejecutarlas muchas veces.

>[!NOTE]
>
>Solo los campos de metadatos de la Vista de metadatos predeterminada pueden utilizarse para las operaciones de filtrado. La página Vistas de metadatos muestra el nombre de la vista de metadatos predeterminada.

Consulte [Vistas de metadatos](application-setup.md#metadata_views).

### Ejecutar una operación de filtrado {#running-a-filter-operation}

Siga estos pasos para poder localizar los recursos filtrándolos con sus valores de metadatos:

1. En la Biblioteca de recursos, seleccione la ficha **[!UICONTROL Filtros]**.

   Los criterios de su operación de filtrado anterior se mostrarán en el panel Filtros. El panel Filtros está dividido en varios paneles; cada uno de ellos representa un campo de metadatos. Utilice los paneles para seleccionar con qué campos de metadatos filtrar y, dentro de cada campo, para seleccionar un valor de metadatos para la operación de filtrado.

   Para ejecutar una operación de filtro que creó y guardó, seleccione **[!UICONTROL Seleccionar ajuste preestablecido]** y, a continuación, elija el nombre de la operación en el menú.

   Ver [Guardar, repetir y eliminar operaciones de filtro](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Haga clic en **[!UICONTROL Campo]** en un panel y, a continuación, siga estas instrucciones para que pueda mostrar el menú de filtrado y construir la operación de filtrado:

   * **Elija un campo de metadatos**: seleccione el nombre del campo en el menú de filtrado.

     >[!NOTE]
     >
     >En el menú de filtrado solo aparecen los nombres de los campos de metadatos de la vista de metadatos predeterminada.

     Consulte [Vistas de metadatos](application-setup.md#metadata_views).

   * **Agregar un campo de metadatos**: seleccione **[!UICONTROL Agregar un panel]**. Una vez que el panel aparezca en el panel Filtros, seleccione su botón **[!UICONTROL Campo]** y elija el nombre de un campo de metadatos en el menú de filtrado.

   * **Quitar un campo de metadatos**: seleccione **[!UICONTROL Quitar este panel]** en el menú de filtrado.

   Al elegir un campo de metadatos, su panel muestra lo siguiente:

   * Todos los valores de los metadatos se introducen en el campo.
   * Para cada valor de metadatos, el número de recursos a los que se les ha dado el valor.

1. Repita el paso 2 tantas veces como sea necesario para mostrar en los paneles todos los campos de metadatos para la operación de filtrado.
1. En cada panel, seleccione un valor de metadatos con el que realizar la operación de filtrado. No se puede seleccionar más de un valor de metadatos en cada panel.

   Los Assets que coincidan con todos los valores seleccionados aparecerán en el panel Examinar.

   >[!NOTE]
   >
   >Elimine temporalmente un campo de la operación de filtrado haciendo clic en **[!UICONTROL Anular la selección de todos]**. Esta opción se encuentra en la parte superior de cada panel, encima de los valores de los metadatos.

1. (Opcional) Para guardar la operación de filtrado y poder ejecutarla más adelante, seleccione **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Guardar los ajustes preestablecidos actuales como nuevos]** y, a continuación, escriba un nombre en el cuadro de diálogo **[!UICONTROL Guardar]**.

### Guardar, repetir y eliminar operaciones de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instrucciones en la pestaña Filtros para poder guardar, repetir y eliminar operaciones de filtro:

* **Guardar una operación de filtro**: Vaya a **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Guardar los ajustes preestablecidos actuales como nuevos]** y, a continuación, escriba un nombre en el cuadro de diálogo **[!UICONTROL Guardar]**.

* **Repetir una operación de filtro**: elija **[!UICONTROL Seleccionar ajuste preestablecido]** y elija el nombre de una operación de filtro en el menú. El menú muestra las operaciones de filtrado guardadas.

* **Eliminar una operación de filtro del menú Seleccionar ajuste preestablecido**: ejecute la operación de filtro. A continuación, vaya a **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Eliminar ajuste preestablecido]** en el menú.

## Uso del servidor de metadatos {#using-the-metadata-server}

El servidor de metadatos es una API pública que puede utilizar para buscar recursos mediante metadatos a través de solicitudes http.

Para configurar el servidor de metadatos, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Configuración de Publish]** > **[!UICONTROL Servidor de metadatos]**.

La página Publish del servidor de metadatos le permite establecer las siguientes opciones:

* **[!UICONTROL Publish instantáneo]**: inserta automáticamente los cambios de metadatos que se realicen, incluidos los nuevos recursos, los cambios de palabras clave, etc.

* XMP XMP **[!UICONTROL Paquete de]**: Publica el paquete de paquetes de la aplicación. XMP Este paquete no se utiliza para la búsqueda, pero proporciona la información más actualizada de la versión de la aplicación de la interfaz de usuario de.

* **[!UICONTROL Palabras clave]**: publica las palabras clave en el servidor de metadatos para su uso en búsquedas.

* **[!UICONTROL Campos Publish del servidor de metadatos]**: seleccione los campos que desea incluir en los metadatos. Esta opción le permite determinar cuánta información sobre los recursos está disponible para el público. Estos campos también se muestran en Vistas de metadatos, pero solo se pueden modificar en el servidor de metadatos.

Seleccione **[!UICONTROL Publish Now]** para iniciar el trabajo. Aparece una confirmación de que el trabajo se ha iniciado.

>[!MORELIKETHIS]
>
>* [Conceptos básicos de navegación](navigation-basics.md#navigation_basics)
>* [Ver, agregar y exportar metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
