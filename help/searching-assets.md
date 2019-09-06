---
title: Búsqueda de recursos
seo-title: Búsqueda de recursos
description: nulo
seo-description: Aprenda a buscar recursos.
uuid: 058209 bc-bac 4-4 d 5 c -8261-e 242 a 543 beaf
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: effef 4 e 7-37 c 5-42 e 2-9266-ecd 026 cad 628
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Búsqueda de recursos{#searching-assets}

Para localizar recursos de archivos en Scene7 Publishing System, puede ver los recursos por tipo, clasificarlos en el panel Examinar, llevar a cabo una búsqueda sencilla, avanzada y filtrar por recursos.

>[!NOTE]
>
>La pantalla de Ajustes personales le permite seleccionar cómo desea realizar las búsquedas. Por ejemplo, puede elegir un tipo de búsqueda predeterminado e indicar si desea incluir campos definidos por el usuario en las búsquedas. Para obtener más información, consulte [Ajustes personales](personal-setup.md#personal_setup).

## Visualización de recursos por tipo {#viewing-assets-by-type}

Para ver archivos solo de un determinado tipo al examinar, abra el menú desplegable Mostrar de la Biblioteca de recursos y elija un tipo de archivo. Se mostrarán los recursos del tipo elegido en la biblioteca de recursos.

## Ordenación de archivos en el panel Examinar {#sorting-files-in-the-browse-panel}

Para ordenar el contenido de una carpeta o buscar resultados en el panel Examinar, seleccione el menú Ordenar y elija una opción. Las opciones son Nombre, Tamaño, Tipo, Fecha de creación y Última modificación. 

Puede elegir entre Ascendente o Descendente para colocar los recursos según los criterios elegidos.

En la vista de lista, puede ordenar haciendo clic en el nombre de una columna.

## Búsqueda simple {#conducting-a-simple-search}

Utilice el campo Buscar para realizar una búsqueda simple. Puede buscar elementos por nombre o buscar los elementos cuyos metadatos contengan una palabra clave determinada. 

Para realizar una búsqueda sencilla:

1. Seleccione la carpeta en la biblioteca de recursos para realizar búsquedas en una carpeta específica y sus subcarpetas.
1. Haga clic en  en la biblioteca de recursos y elija una opción según el ámbito de búsqueda deseado. Puede elegir En todos los archivos y carpetas, En la carpeta seleccionada o En carpetas y subcarpetas seleccionadas.
1. Introduzca un término de búsqueda. 
1. Haga clic en Ir y pulse Intro.

   Los resultados de la búsqueda se mostrarán en el panel Examinar. 

>[!NOTE]
>
>Dynamic Media Classic rastrea las búsquedas. Para volver a ejecutar una búsqueda, seleccione el botón de búsqueda y elija el nombre de la búsqueda deseada en la parte inferior del menú de búsqueda.

## Búsqueda avanzada {#conducting-an-advanced-search}

Haga clic en Búsqueda avanzada en la biblioteca de recursos para realizar búsquedas con muchos criterios, incluidos los valores de los campos de metadatos.

Especifique uno de los siguientes criterios de búsqueda:

**Filtrar por tipo de recurso** Reduzca la búsqueda a un solo tipo de recurso eligiendo un tipo de recurso en el menú.

**Archivos y carpetas** Elija dónde desea buscar: En todos los archivos y carpetas, En la carpeta seleccionada o En carpetas y subcarpetas seleccionadas.

**Todos los estados** de publicación Buscar archivos marcados para publicación, no están marcados para publicación o todos los archivos.

**Condiciones** Si especifica criterios de metadatos para la búsqueda, seleccione si la búsqueda debe coincidir con todas las condiciones (búsqueda TODAS) o con cualquier condición (búsqueda O).

**Especificar los criterios de búsqueda de metadatos** Cree uno o más campos de búsqueda para buscar los metadatos. Para crear campos de búsqueda:

1. Abra la lista Vistas de metadatos (a la izquierda del menú Agregar un campo) y elija una vista de metadatos. Puede elegir mostrar una vista compacta, IPTC, XMP, o bien, una vista que su administrador haya configurado.
1. Seleccione el menú Agregar un campo y elija un nombre de campo en la lista desplegable.
1. Elija una opción entre Contiene, No contiene, Comienza por, Termina por o Igual que.
1. En el caso de los campos numéricos, elija un valor o introduzca un intervalo de fechas personalizado.
1. (Opcional) Repita los pasos 1-4 para crear más campos de búsqueda.

Para eliminar un campo puede hacer clic en el botón Eliminar campo de búsqueda. 

Haga clic en Buscar para comenzar la búsqueda. Los resultados de la búsqueda se mostrarán en el panel Examinar. Puede modificar cualquier condición de búsqueda y hacer clic en Buscar para ejecutarla de nuevo.

Haga clic en Borrar para borrar los criterios de búsqueda y comenzar una nueva búsqueda. Seleccione el botón Cerrar cuando finalice la operación para cerrar el panel de búsqueda.

## Filtrado de recursos con metadatos {#filter-assets-using-metadata}

Filtre recursos en la ficha Filtros de la Biblioteca de recursos. Para filtrar recursos, utilice valores de metadatos como criterios. Tras elegir el campo de metadatos que desea utilizar para filtrar, la ficha Filtros muestra todos los valores de metadatos introducidos en el campo elegido y el número de recursos asignado a cada valor. Por ejemplo, en una operación de filtrado en el campo de metadatos Creador, la ficha Filtros muestra todos los nombres introducidos en el campo de metadatos Creador de los diferentes recursos y, para cada nombre, el número de recursos asignados al nombre. Puede hacer clic en un valor de metadatos para ver todos los recursos a los que se les ha asignado dicho valor. En el ejemplo, el usuario hace clic en el valor de metadatos Jimmy para ver todos los recursos en el que se introdujo el nombre Jimmy en el campo de metadatos Creador. Puede filtrar utilizando más de un campo de metadatos como criterio de filtro.

Puede guardar las operaciones de filtrado para ejecutarlas más veces.

>[!NOTE]
>
>Solo los campos de metadatos de la Vista de metadatos predeterminada pueden utilizarse para las operaciones de filtrado. La pantalla Vistas de metadatos muestra el nombre de la vista de metadatos predeterminada.

Consulte [Vistas de metadatos](application-setup.md#metadata_views).

### Operación de filtrado {#running-a-filter-operation}

Siga estos pasos para localizar recursos mediante filtros con sus valores de metadatos:

1. Haga clic en la ficha Filtros de la Biblioteca de recursos.

   Los criterios de su operación de filtrado anterior se mostrarán en el panel Filtros. El panel Filtros está dividido en varios paneles; cada uno de ellos representa un campo de metadatos. Utilice los paneles para seleccionar con qué campos de metadatos filtrar y, dentro de cada campo, para seleccionar un valor de metadatos para la operación de filtrado.

   Para ejecutar una operación de filtrado que se ha creado y guardado anteriormente, haga clic en el botón de selección de ajustes preestablecidos y elija el nombre de la operación en el menú.

   Consulte [Guardado, repetición y eliminación de operaciones de filtrado](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Haga clic en el botón Campo  de un panel y siga estas instrucciones para mostrar el menú de filtrado y crear la operación correspondiente:

   **Selección
de un campo de metadatos** Seleccione el nombre del campo en el menú de filtrado.

   ***nota**: En el menú de filtrado solo aparecen los nombres de los campos de metadatos de la vista de metadatos predeterminada.*

   Consulte [Vistas de metadatos](application-setup.md#metadata_views).

   **Agregar un campo de metadatos** Elija Agregar un panel. Cuando éste aparezca en el panel Filtros, haga clic en el botón Campo y seleccione el nombre de un campo de metadatos en el menú de filtrado.

   **Al eliminar un campo** de metadatos, elija Quitar este panel en el menú de filtrado.

   Si selecciona un campo de metadatos, su panel muestra:

   * Todos los valores de metadatos introducidos en el campo.
   * Para cada valor de metadatos, el número de recursos a los que se les ha dado el valor.

1. Repita el paso 2 tantas veces como sea necesario para mostrar en los paneles todos los campos de metadatos para la operación de filtrado.
1. En cada panel, seleccione un valor de metadatos con el que realizar la operación de filtrado. No puede seleccionar más de un valor de metadatos en cada panel.

   Los recursos que coincidan con todos los valores seleccionados aparecerán en el panel Examinar.

   >[!NOTE]
   >
   >Para eliminar temporalmente un campo de la operación de filtrado, haga clic en Anular todas las selecciones. Esta opción está situada en la parte superior de cada panel, encima de los valores de metadatos.

1. (Opcional) Para guardar la operación de filtrado y poder ejecutarla más adelante, haga clic en el botón Seleccionar ajuste preestablecido, seleccione Guardar los ajustes preestablecidos actuales como nuevos e introduzca un nombre en el cuadro de diálogo Guardar. 

### Guardado, repetición y eliminación de operaciones de filtrado {#saving-repeating-and-deleting-filter-operations}

Siga estas instrucciones en la ficha Filtros para guardar, repetir y eliminar las operaciones de filtrado:

**Guardado de una operación de filtrado** Haga clic en el botón Seleccionar ajuste preestablecido, seleccione Guardar valores preestablecidos actuales como nuevos e introduzca un nombre en el cuadro de diálogo Guardar.

**Repetir una operación de filtrado** Haga clic en el botón Seleccionar ajuste preestablecido y elija el nombre de una operación de filtrado en el menú. El menú muestra las operaciones de filtrado guardadas.

**Eliminación de una operación de filtrado del menú Seleccionar ajuste preestablecido** 
Ejecute la operación de filtrado. A continuación, haga clic en el botón Seleccionar ajuste preestablecido y seleccione Eliminar ajuste preestablecido en el menú.

## Uso del servidor de metadatos {#using-the-metadata-server}

El servidor de metadatos es una API pública que permite buscar recursos por metadatos mediante solicitudes HTTP.

Para configurar el servidor de metadatos, haga clic en Ajustes &gt; Ajustes de aplicación &gt; Ajustes de publicación &gt; Servidor de metadatos.

Se abre la pantalla Publicación en el servidor de metadatos. Esta pantalla permite definir las siguientes opciones:

**Publicación** instantánea Inserta automáticamente cualquier cambio de metadatos cuando se realiza, incluidos nuevos recursos, cambios de palabras clave, etc.

**XMP Packet** publica el paquete XMP. Este paquete no se utiliza en las búsquedas, pero proporciona el XMP más actualizado.

**Palabras clave** Publica las palabras clave en el servidor de metadatos para usarlas en búsquedas.

**Campos de publicación del servidor de metadatos** Seleccione los campos que incluir en los metadatos. Permite determinar cuánta información sobre los recursos está a disposición pública. Estos campos también se muestran en Vistas de metadatos, pero solo se pueden modificar en el servidor de metadatos.

Click **Publish Now** to start the job. Aparece una confirmación de que el trabajo se ha iniciado.

>[!MORELIKETHIS]
>
>* [Nociones básicas de navegación](navigation-basics.md#navigation_basics)
>* [Visualización, adición y exportación de metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

