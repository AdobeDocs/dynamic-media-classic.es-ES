---
title: Crear un catálogo electrónico
description: Obtenga información sobre cómo crear un catálogo electrónico en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# Creación de un catálogo electrónico {#creating-an-ecatalog}

La creación de un catálogo electrónico implica ordenar las páginas, elegir el diseño de página y vincular las páginas dibujando mapas de imágenes. También requiere la introducción de datos de rollover y de vínculos de hipertexto. Si lo desea, también puede personalizar la tabla de contenido para que los usuarios vean nombres de página en lugar de números en el visor de catálogos electrónicos.

## Crear un catálogo electrónico {#create}

Puede incluir archivos de imagen y archivos de PDF en el catálogo electrónico.

Cuando crea un catálogo electrónico, la opción **[!UICONTROL Publish después de guardar]** afecta a los miembros set y set de las siguientes maneras:

| ¿La opción &quot;Publish después de guardar&quot; está seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un catálogo electrónico:**

1. Comience la creación del catálogo electrónico utilizando una de estas técnicas:

   * **Seleccione los archivos primero**: en el panel Examinar, seleccione los archivos y, a continuación, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Catálogos electrónicos]**.

   * **Empiece desde la pantalla del catálogo electrónico**: Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Catálogos electrónicos]**. Seleccione una carpeta en la biblioteca de recursos. Arrastre archivos desde la carpeta a la ficha Ordenar páginas de la página Catálogo electrónico.

     >[!NOTE]
     >
     >Para ver los elementos de la biblioteca de recursos por su nombre en lugar de ver las miniaturas, seleccione la opción Nombre en la vista de biblioteca de recursos predeterminada en Ajustes personales.

1. Seleccione la presentación general que tendrá el catálogo electrónico. Seleccione **[!UICONTROL 1 Up]** para páginas individuales, **[!UICONTROL 2 Up]** para pliegos de dos páginas o **[!UICONTROL Custom]** para pliegos de más de dos páginas. En el cuadro de diálogo **[!UICONTROL Cambiar diseño de catálogo electrónico]**, seleccione las opciones **[!UICONTROL Todas las distribuciones]** y seleccione **[!UICONTROL Aceptar]**.
1. Si lo desea, puede cambiar el diseño de páginas o pliegos de páginas individuales seleccionándolos y eligiendo el botón **[!UICONTROL 1 arriba]**, **[!UICONTROL 2 arriba]** o **[!UICONTROL personalizado]**. En el cuadro de diálogo **[!UICONTROL Cambiar diseño de catálogo electrónico]**, seleccione las opciones **[!UICONTROL Distribuciones seleccionadas]** y seleccione **[!UICONTROL Aceptar]**.
1. Reordene las páginas según sea necesario con una de estas técnicas:

   * **Arrastrando**: arrastre una página o un pliego de páginas a una nueva ubicación. La barra vertical muestra el lugar al que se ha movido la página.

   * **Botón Mover a**: seleccione una página o un pliego de páginas, seleccione **[!UICONTROL Mover a]** y elija la página del menú antes de la cual desea que aparezca la página.

   * **Secuencia #**: en la vista de lista, escriba números de página en los campos de Secuencia #.

1. Cuando termine, cerca de la esquina inferior derecha de la página, asegúrese de seleccionar **[!UICONTROL Publish después de guardar]** (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el catálogo electrónico. En el campo Nombre de archivo, introduzca el nombre del conjunto de giros.
1. Seleccione **[!UICONTROL Guardar]**.

   Puede obtener una vista previa del catálogo electrónico, después de guardarlo, seleccionando **[!UICONTROL Vista previa]**.

## Editar un catálogo electrónico {#editing-an-ecatalog}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publish después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | ¿Ha seleccionado la opción &quot;Publish después de guardar&quot; antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un catálogo electrónico:**

1. Seleccione el botón de rollover **[!UICONTROL Editar]** del catálogo electrónico.
1. Realice los cambios necesarios.
1. Cuando termine de editar, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish después de guardar]** esté seleccionado (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un catálogo electrónico

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un catálogo electrónico:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios catálogos electrónicos.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Personalizar la tabla de contenido (TDC) {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic proporciona números de página predeterminados en el catálogo electrónico en la ficha Ordenar páginas de la pantalla Catálogo electrónico. Si desea personalizar el nombre de las páginas, puede cambiar las etiquetas de las páginas que forman la tabla de contenido (TOC). Se recomienda cambiar el nombre de la portada y la contraportada. Por ejemplo, la portada puede decir &quot;Portada&quot; en lugar de &quot;Página 0-1&quot;.

Puede crear manualmente una tabla de contenido (TOC) personalizada para su catálogo electrónico. También puede importar los nombres de las páginas desde un archivo CSV (solo Mac) o XML.

>[!NOTE]
>
>Para restaurar los títulos de página predeterminados, en la ficha **[!UICONTROL Ordenar páginas]**, seleccione **[!UICONTROL Etiquetas de tabla de contenido]** y, a continuación, seleccione **[!UICONTROL Restaurar valores predeterminados (todos)]**.

### Introducción manual de nombres de página {#manually-entering-page-names}

Introduzca manualmente los nombres de las páginas de uno en uno accediendo a la pestaña Ordenar páginas de la pantalla Catálogo electrónico. A continuación, en el campo del número de página, escriba un nombre para cada página a la que desee asignar un nombre.

### Importar nombres de página {#importing-page-names}

Se recomienda la importación de nombres de página si se trabaja con un catálogo electrónico de muchas páginas. También puede importar los nombres de un archivo delimitado por tabuladores o XML.

La etiqueta TOC se almacena en el campo Datos de usuario de una imagen; dé formato a estos datos como una lista de `name=<value>` ` pairs separated by two question marks "??" `. Por ejemplo, para establecer una etiqueta para un campo de índice denominado `tocEN`, establezca los Datos de usuario de la imagen en:

`tocEN=&lt;EN_page_label>`

Para establecer etiquetas independientes para los campos de índice llamados `tocEN` y `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Para importar el campo Datos de usuario en un archivo delimitado por tabuladores, incluya los datos de usuario del campo:

| IPSID | Datos de usuario |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Para importar el campo Datos de usuario en un archivo XML, incluya el atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nombres de páginas desde un archivo XML o delimitado por tabuladores, seleccione el botón **[!UICONTROL Etiquetas de tabla de contenido]** y seleccione **[!UICONTROL Importar]**. En el cuadro de diálogo Cargar metadatos, seleccione **[!UICONTROL Examinar]** y, a continuación, importe el archivo CSV (solo Mac) o el archivo XML que asocia cada página con un nombre de página.
