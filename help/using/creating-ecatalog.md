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
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 44%

---

# Creación de un catálogo electrónico {#creating-an-ecatalog}

Al crear un catálogo electrónico es preciso ordenar las páginas, elegir su presentación y vincular las páginas mediante mapas de imagen y datos de vínculos de hipertexto y de rollover. Si lo desea, también puede personalizar la tabla de contenido para que los usuarios vean nombres de página en lugar de números en el visor de catálogos electrónicos.

## Crear un catálogo electrónico {#create}

Puede incluir archivos de imagen y archivos de PDF en el catálogo electrónico.

Al crear un catálogo electrónico, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿La opción &quot;Publicar después de guardar&quot; está seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un catálogo electrónico:**

1. Comience la creación del catálogo electrónico utilizando una de estas técnicas:

   * **Seleccione primero los archivos** - En el panel Examinar, seleccione archivos y, a continuación, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Catálogos electrónicos]**.

   * **Empezar desde la pantalla Catálogo electrónico** - Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Catálogos electrónicos]**. Seleccione una carpeta en la biblioteca de recursos y arrastre los archivos deseados a la ficha Ordenar páginas que se encuentra en la página Catálogo electrónico.

     >[!NOTE]
     >
     >Para ver los elementos de la biblioteca de recursos por su nombre en lugar de ver las miniaturas, seleccione la opción Nombre en la vista de biblioteca de recursos predeterminada en Ajustes personales.

1. Seleccione la presentación general que tendrá el catálogo electrónico. Seleccionar **[!UICONTROL 1 vertical]** para páginas únicas, **[!UICONTROL 2 verticales]** para pliegos de dos páginas, o **[!UICONTROL Personalizado]** para pliegos de más de dos páginas. En el **[!UICONTROL Cambiar diseño de catálogo electrónico]** , seleccione la opción **[!UICONTROL Todas las distribuciones]** opciones y seleccione **[!UICONTROL OK]**.
1. Si lo desea, puede cambiar el diseño de páginas o pliegos de páginas individuales seleccionándolos y eligiendo **[!UICONTROL 1 vertical]**, **[!UICONTROL 2 verticales]**, o **[!UICONTROL Personalizado]** botón. En el **[!UICONTROL Cambiar diseño de catálogo electrónico]** , seleccione la opción **[!UICONTROL Distribuciones seleccionadas]** opciones y seleccione **[!UICONTROL OK]**.
1. Reordene las páginas según sea necesario con una de estas técnicas:

   * **Arrastrando** : arrastre una página o un pliego de páginas a una nueva ubicación. La barra vertical muestra el lugar al que se ha movido la página.

   * **Botón Mover a** : seleccione una página o un pliego de páginas, seleccione **[!UICONTROL Mover a]** y elija la página del menú antes de la que desea que aparezca la página.

   * **Nº de secuencia** - En Vista de lista, introduzca los números de página en los campos de Nº de secuencia.

1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccionar **[!UICONTROL Guardar]**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el catálogo electrónico. En el campo Nombre de archivo, escriba el nombre del conjunto de giros.
1. Seleccionar **[!UICONTROL Guardar]**.

   Puede obtener una vista previa del catálogo electrónico, después de guardarlo, seleccionando **[!UICONTROL Previsualizar]**.

## Editar un catálogo electrónico {#editing-an-ecatalog}

Si edita un conjunto publicado o no publicado, la variable **[!UICONTROL Publicar tras guardar]** afecta a los miembros set y set de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | ¿La opción &quot;Publicar después de guardar&quot; está seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un catálogo electrónico:**

1. Seleccione la sustitución del catálogo electrónico **[!UICONTROL Editar]** botón.
1. Realice los cambios necesarios.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccionar **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un catálogo electrónico

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un catálogo electrónico:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios catálogos electrónicos.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Personalizar la tabla de contenido (TDC) {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic proporciona números de página predeterminados en el catálogo electrónico en la ficha Ordenar páginas de la pantalla Catálogo electrónico. Si desea personalizar el nombre de las páginas, puede cambiar las etiquetas de las páginas que forman la tabla de contenido (TOC). Se recomienda cambiar el nombre de la portada y la contraportada. Por ejemplo, la portada puede decir &quot;Portada&quot; en lugar de &quot;Página 0-1&quot;.

Puede crear una tabla de contenido (TOC) personalizada para su catálogo electrónico manualmente o importando los nombres de página desde un archivo CSV (solo Mac) o XML.

>[!NOTE]
>
>Para restaurar los títulos de página predeterminados, en la **[!UICONTROL Ordenar páginas]** pestaña, seleccione **[!UICONTROL Etiquetas de TDC]**, y luego seleccione **[!UICONTROL Restaurar valores (todos)]**.

### Introducción manual de nombres de página {#manually-entering-page-names}

Para introducir manualmente nombres de página uno por uno, vaya a la ficha Ordenar páginas de la pantalla Catálogo electrónico. A continuación, en el campo del número de página, escriba un nombre para cada página a la que desee asignar un nombre.

### Importar nombres de página {#importing-page-names}

Se recomienda la importación de nombres de página si se trabaja con un catálogo electrónico de muchas páginas. También puede importar los nombres de un archivo delimitado por tabuladores o XML.

La etiqueta del índice se almacena en el campo Datos de usuario de una imagen; dé formato a estos datos como una lista de `name=<value>` ` pairs separated by two question marks "??" `. Por ejemplo, para establecer una etiqueta para un campo de índice denominado `tocEN`, establezca los Datos de usuario de la imagen en:

`tocEN=&lt;EN_page_label>`

Para establecer etiquetas independientes para los campos del índice llamados `tocEN` y `tocFR`:

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

Para importar nombres de página desde un archivo XML o delimitado por tabuladores, seleccione la opción **[!UICONTROL Etiquetas de TDC]** y seleccione **[!UICONTROL Importar]**. En el cuadro de diálogo Cargar metadatos, seleccione **[!UICONTROL Examinar]** e importe el archivo CSV (solo Mac) o el archivo XML que asocia cada página con un nombre de página.
