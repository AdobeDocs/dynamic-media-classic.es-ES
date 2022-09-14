---
title: Buscar recursos de Dynamic Media Classic
description: Obtenga información sobre cómo buscar recursos en Adobe Dynamic Media Classic.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 19%

---

# Buscar recursos en Adobe Dynamic Media Classic{#searching-assets}

Para localizar recursos de archivos en Adobe Dynamic Media Classic, puede ver los recursos por tipo, ordenarlos en el panel Examinar, realizar una búsqueda sencilla, avanzada y filtrar por recursos.

>[!NOTE]
>
>La página Configuración personal ofrece opciones para elegir cómo desea realizar búsquedas. Por ejemplo, puede elegir un tipo de búsqueda predeterminado e indicar si desea incluir campos definidos por el usuario en las búsquedas. Para obtener más información, consulte [Ajustes personales](personal-setup.md#personal_setup).

## Ver recursos por tipo {#viewing-assets-by-type}

Para ver solo archivos de un tipo determinado a medida que navega, en la biblioteca de recursos del lado izquierdo, en la sección **[!UICONTROL Show]** lista desplegable, elija un tipo de archivo. En la biblioteca de recursos solo aparecen los recursos del tipo que haya elegido mostrar.

>[!NOTE]
>
>Si no ve el panel Biblioteca de recursos en el lado izquierdo, seleccione la flecha de triángulo derecha en el lado izquierdo, a mitad de la ventana de Adobe Dynamic Media Classic, para abrir la Biblioteca de recursos).

## Ordenar archivos en el panel Examinar {#sorting-files-in-the-browse-panel}

Para ordenar el contenido de una carpeta o buscar los resultados que aparecen en el panel Examinar del lado derecho, en la barra de navegación global, seleccione **[!UICONTROL Ordenar]** y, a continuación, elija una opción. Las opciones son **[!UICONTROL Nombre]**, **[!UICONTROL Tamaño (KB)]**, **[!UICONTROL Tipo]**, **[!UICONTROL Fecha de creación]** y **[!UICONTROL Última modificación]**.

También puede elegir **[!UICONTROL Ascendente]** o **[!UICONTROL Descendente]** para ordenar los recursos en orden ascendente o descendente según el criterio que elija.

En la vista de lista, puede ordenar haciendo clic en el nombre de una columna.

## Búsqueda sencilla {#conducting-a-simple-search}

Utilice el campo Buscar de la biblioteca de recursos para realizar búsquedas sencillas. Puede buscar elementos por nombre o buscar los elementos cuyos metadatos contengan una palabra clave determinada. 

1. En la biblioteca de recursos, en la **[!UICONTROL Carpetas]** , seleccione la carpeta que desea buscar en una carpeta concreta y sus subcarpetas.
1. A la izquierda del campo Buscar en la biblioteca de recursos, seleccione la opción **[!UICONTROL Lupa]** para abrir la lista desplegable.
1. En la lista desplegable, elija una opción que describa el alcance o el alcance con el que desea que se realice la búsqueda. Puede elegir **[!UICONTROL Dentro de todos los archivos y carpetas]**, **[!UICONTROL Dentro de la carpeta seleccionada]** o **[!UICONTROL Dentro de carpetas y subcarpetas seleccionadas]**.
1. En el campo Buscar , introduzca un término de búsqueda.
1. A la derecha del campo Buscar , seleccione **[!UICONTROL Ir]** o presione **[!UICONTROL Entrar]**.

   Los resultados de la búsqueda aparecen en el panel Examinar de la derecha.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Búsqueda avanzada {#conducting-an-advanced-search}

En la biblioteca de recursos, directamente debajo del campo Buscar, seleccione **[!UICONTROL Búsqueda avanzada]** para buscar utilizando muchos criterios, incluidos los valores de los campos de metadatos.

Especifique cualquiera de los siguientes criterios en la búsqueda avanzada:

* **Filtrar por tipo de recurso** : limite la búsqueda a un solo tipo de recurso seleccionando un tipo de recurso en el menú.

* **Archivos y carpetas** - Elija dónde desea buscar: **[!UICONTROL Dentro de todos los archivos y carpetas]**, **[!UICONTROL Dentro de la carpeta seleccionada]** o **[!UICONTROL Dentro de carpetas y subcarpetas seleccionadas]**.

* **Todos los estados de publicación** - Busque archivos marcados como listos para publicar, no marcados como listos para publicar o todos los archivos.

* **Condiciones** - Si especifica criterios de metadatos para la búsqueda, seleccione si la búsqueda debe coincidir con todas las condiciones (una búsqueda ALL) o con cualquier condición (una búsqueda OR).

* **Criterios de búsqueda** - Cree uno o más campos de búsqueda para buscar metadatos. Para crear campos de búsqueda:

   1. En Búsqueda avanzada, en la sección **[!UICONTROL Criterios de búsqueda]** y a la izquierda del **[!UICONTROL Agregar un campo]** ), seleccione el icono de flecha hacia abajo del triángulo para abrir la lista desplegable. Elija una vista de metadatos. Puede elegir **[!UICONTROL Todas las propiedades con valores]**, **[!UICONTROL Vista compacta]**, **[!UICONTROL IPTC]**, **[!UICONTROL Campos de publicación del servidor de metadatos]** o **[!UICONTROL XMP]**.
   1. Seleccione el **[!UICONTROL Agregar un campo]** menú desplegable y elija un nombre de campo.
   1. Elija un **[!UICONTROL Contiene]** opción: **[!UICONTROL Contiene]**, **[!UICONTROL No contiene]**, **[!UICONTROL Comienza con]**, **[!UICONTROL Finaliza con]** o **[!UICONTROL Es igual a]**.
   1. En el caso de los campos numéricos, elija un valor o introduzca un intervalo de fechas personalizado.
   1. (Opcional) Repita los pasos del 1 al 4 para crear más campos de búsqueda.

Seleccione el **[!UICONTROL Quitar campo de búsqueda]** (círculo con &quot;X&quot; dentro) para que se elimine el campo de búsqueda.

En la esquina inferior derecha del panel Búsqueda avanzada, seleccione **[!UICONTROL Buscar]** para comenzar la búsqueda. Los resultados de la búsqueda aparecen en el panel Examinar de la derecha. Puede cambiar cualquier condición de búsqueda y seleccionar **[!UICONTROL Buscar]** para volver a ejecutar la búsqueda.

Select **[!UICONTROL Borrar]** si desea borrar los criterios de búsqueda e iniciar una nueva búsqueda. Select **[!UICONTROL Cerrar]** cuando termine de buscar para cerrar el panel Buscar .

## Filtrado de recursos con metadatos {#filter-assets-using-metadata}

Filtre recursos en la ficha Filtros de la Biblioteca de recursos. Para filtrar recursos, utilice valores de metadatos como criterios. Después de elegir un campo de metadatos con el que desea filtrar, la ficha Filtros enumera todos los valores de metadatos introducidos en el campo que ha elegido. También muestra el número de recursos asignados a cada valor. Por ejemplo, en una operación de filtro en la **[!UICONTROL Creador]** campo de metadatos, la variable **[!UICONTROL Filtros]** lista todos los nombres introducidos en la **[!UICONTROL Creador]** campo de metadatos para diferentes recursos. También muestra para cada nombre el número de recursos asignados al nombre. A continuación, seleccione un valor de metadatos para ver todos los recursos asignados a ese valor. En el ejemplo, se selecciona la variable `Prairie Cat` valor de metadatos para ver todos los recursos en los que el nombre `Prairie Cat` se introdujo en la variable **[!UICONTROL Creador]** campo de metadatos. Puede filtrar utilizando más de un campo de metadatos como criterio de filtro.

Puede guardar las operaciones de filtro para ejecutarlas muchas veces.

>[!NOTE]
>
>Solo los campos de metadatos de la Vista de metadatos predeterminada pueden utilizarse para las operaciones de filtrado. La página Vistas de metadatos muestra el nombre de la vista de metadatos predeterminada.

Consulte [Vistas de metadatos](application-setup.md#metadata_views).

### Ejecutar una operación de filtro {#running-a-filter-operation}

Siga estos pasos para poder localizar recursos filtrando con sus valores de metadatos:

1. En la biblioteca de recursos, seleccione la opción **[!UICONTROL Filtros]** pestaña .

   Los criterios de su operación de filtrado anterior se mostrarán en el panel Filtros. El panel Filtros está dividido en varios paneles; cada uno de ellos representa un campo de metadatos. Utilice los paneles para seleccionar con qué campos de metadatos filtrar y, dentro de cada campo, para seleccionar un valor de metadatos para la operación de filtrado.

   Para ejecutar una operación de filtro que ha creado y guardado, seleccione **[!UICONTROL Seleccionar ajuste preestablecido]** y, a continuación, elija el nombre de la operación en el menú .

   Consulte [Guardar, repetir y eliminar operaciones de filtro](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Select **[!UICONTROL Campo]** en un panel, siga estas instrucciones para mostrar el menú de filtrado y construir la operación de filtro:

   * **Elegir un campo de metadatos** - Seleccione el nombre del campo en el menú de filtrado.

      >[!NOTE]
      >
      >En el menú de filtrado solo aparecen los nombres de los campos de metadatos de la vista de metadatos predeterminada.

      Consulte [Vistas de metadatos](application-setup.md#metadata_views).

   * **Añadir un campo de metadatos** - Seleccionar **[!UICONTROL Agregar un panel]**. Una vez que aparezca el panel en el panel Filtros , seleccione su **[!UICONTROL Campo]** y elija el nombre de un campo de metadatos en el menú de filtrado.

   * **Eliminación de un campo de metadatos** - Seleccionar **[!UICONTROL Quitar este panel]** en el menú de filtrado.

   Al elegir un campo de metadatos, su panel enumera lo siguiente:

   * Todos los valores de metadatos introducidos en el campo.
   * Para cada valor de metadatos, el número de recursos a los que se les ha dado el valor.


1. Repita el paso 2 tantas veces como sea necesario para mostrar en los paneles todos los campos de metadatos para la operación de filtrado.
1. En cada panel, seleccione un valor de metadatos con el que realizar la operación de filtrado. No se puede seleccionar más de un valor de metadatos en cada panel.

   Los recursos que coinciden con todos los valores seleccionados aparecen en el panel Examinar.

   >[!NOTE]
   >
   >Para quitar temporalmente un campo de la operación de filtro, seleccione **[!UICONTROL Anular todas las selecciones]**. Esta opción se encuentra en la parte superior de cada panel, encima de los valores de metadatos.

1. (Opcional) Para guardar la operación de filtro y poder ejecutarla más tarde, seleccione **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Guardar actual como nuevos ajustes preestablecidos]** y, a continuación, introduzca un nombre en la variable **[!UICONTROL Guardar]** para abrir el Navegador.

### Guardar, repetir y eliminar operaciones de filtro {#saving-repeating-and-deleting-filter-operations}

Siga estas instrucciones en la ficha Filtros para guardar, repetir y eliminar operaciones de filtro:

* **Guardar una operación de filtro** - Vaya a **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Guardar actual como nuevos ajustes preestablecidos]** y, a continuación, introduzca un nombre en la variable **[!UICONTROL Guardar]** para abrir el Navegador.

* **Repetir una operación de filtro** - Elija **[!UICONTROL Seleccionar ajuste preestablecido]** y elija el nombre de una operación de filtro en el menú . El menú muestra las operaciones de filtrado guardadas.

* **Eliminar una operación de filtro del menú Seleccionar ajuste preestablecido** - Ejecute la operación de filtro. A continuación, vaya a **[!UICONTROL Seleccionar ajuste preestablecido]** > **[!UICONTROL Eliminar ajuste preestablecido]** en el menú

## Usar el servidor de metadatos {#using-the-metadata-server}

El servidor de metadatos es una API pública que permite buscar recursos por metadatos mediante solicitudes HTTP.

Para configurar el servidor de metadatos, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de publicación]** > **[!UICONTROL Servidor de metadatos]**.

La página Publicación del servidor de metadatos permite establecer las siguientes opciones:

* **[!UICONTROL Publicación instantánea]** : inserta automáticamente cualquier cambio de metadatos cuando se realice, incluidos nuevos recursos, cambios de palabras clave, etc.

* **[!UICONTROL Paquete XMP]** - Publica el paquete XMP. Este paquete no se utiliza para la búsqueda, pero proporciona los XMP más actualizados.

* **[!UICONTROL Palabras clave]** - Publica sus palabras clave en el servidor de metadatos para usarlas en búsquedas.

* **[!UICONTROL Campos de publicación del servidor de metadatos]** - Seleccione los campos que desea incluir en los metadatos. Esta opción le permite determinar cuánta información sobre los recursos está disponible para el público. Estos campos también se muestran en Vistas de metadatos, pero solo se pueden modificar en el servidor de metadatos.

Select **[!UICONTROL Publicar ahora]** para iniciar el trabajo. Aparece una confirmación de que el trabajo se ha iniciado.

>[!MORELIKETHIS]
>
>* [Nociones básicas de navegación](navigation-basics.md#navigation_basics)
>* [Ver, agregar y exportar metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

