---
title: Creación de un catálogo electrónico
seo-title: Creación de un catálogo electrónico
description: nulo
seo-description: Aprenda a crear un catálogo electrónico.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 78%

---


# Creación de un catálogo electrónico{#creating-an-ecatalog}

Al crear un catálogo electrónico es preciso ordenar las páginas, elegir su presentación y vincular las páginas mediante mapas de imagen y datos de vínculos de hipertexto y de rollover. Si lo desea, también puede personalizar la tabla de contenido para que los usuarios vean nombres de página en lugar de números en el visor de catálogos electrónicos.

## Creación de un catálogo electrónico {#create}

El catálogo electrónico puede contener tanto archivos de imagen como archivos PDF. 

Al crear un catálogo electrónico, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un catálogo electrónico**

1. Comience la creación del catálogo electrónico utilizando una de estas técnicas:

   **Seleccione los archivos primero** En el panel Examinar, seleccione los archivos y, a continuación, haga clic en Generar > Catálogos electrónicos.

   **Inicio en la pantalla** Catálogo electrónico Haga clic en Generar > Catálogos electrónicos. Seleccione una carpeta en la biblioteca de recursos y arrastre los archivos deseados a la ficha Ordenar páginas que se encuentra en la página Catálogo electrónico.

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. Seleccione la presentación general que tendrá el catálogo electrónico. Haga clic en el botón 1 vertical  para mostrar una sola página, en el botón 2 verticales  para mostrar dos páginas, o en el botón Personalizar  para mostrar más de dos páginas. Aparecerá el cuadro de diálogo Cambiar la presentación del catálogo electrónico. Select the All Spreads options and click **OK**.
1. También puede cambiar la presentación de las páginas o distribuciones de páginas individuales seleccionándolas y eligiendo a continuación el botón 1 vertical, 2 verticales o Personalizar. Aparecerá el cuadro de diálogo Cambiar la presentación del catálogo electrónico. Select the Selected Spreads options and click **OK**.
1. Reordene las páginas según sea necesario con una de estas técnicas:

   **Arrastrar** Arrastre una página o un conjunto de páginas a una nueva ubicación. La barra vertical muestra el lugar al que se ha movido la página.

   **Botón** Mover aSeleccione una página o un pliego de páginas, haga clic en el botón Mover a y elija la página en el menú que desea que la página aparezca antes.

   **Secuencia #** En Vista de Lista, introduzca los números de página en los campos Nº de secuencia.

1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el catálogo electrónico. En el campo Nombre de archivo, escriba el nombre del conjunto de giros.
1. Haga clic en **Guardar**.

   Una vez que haya guardado el catálogo electrónico, podrá acceder a la vista previa de este si hace clic en **Vista previa**.

## Edición de un catálogo electrónico {#editing-an-ecatalog}

Según si edita un conjunto publicado o sin publicar, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservan su estado publicado.Los nuevos miembros del conjunto que haya agregado durante la edición conservarán su estado publicado o sin publicar. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un catálogo electrónico**

1. Haga clic en el botón de rollover **Editar** del catálogo electrónico.
1. Realice los cambios necesarios.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **Guardar**.

## Eliminación de un catálogo electrónico {#deleting-an-ecatalog}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un catálogo electrónico**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios catálogos electrónicos.
1. En la barra de navegación global, haga clic en **Archivo** > **Eliminar** > **Eliminar**.

## Personalización de la tabla de contenido (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic proporciona números de página predeterminados en el catálogo electrónico en la ficha Ordenar páginas de la pantalla Catálogo electrónico. Si desea personalizar el nombre de las páginas, puede cambiar las etiquetas de las páginas que forman la tabla de contenido (TOC). Se recomienda cambiar el nombre de la portada y la contraportada. Por ejemplo: la portada principal puede ser &quot;Portada&quot; en lugar de &quot;Página 0-1&quot;.

Puede crear una tabla de contenido (TOC) personalizada para el catálogo electrónico manualmente o importando los nombres de las páginas de un archivo CSV (solo Mac) o XML.

>[!NOTE]
>
>Para restaurar los títulos de página predeterminados, haga clic en el botón Etiquetas de tabla de contenido en la ficha Ordenar páginas y elija Restaurar valores (todos).

### Introducción manual de nombres de página {#manually-entering-page-names}

Para introducir manualmente nombres de página uno por uno, vaya a la ficha Ordenar páginas de la pantalla Catálogo electrónico. Haga clic en el campo del número de página e introduzca un nombre. Introduzca un nombre para cada página si lo desea.

### Importación de nombres de página {#importing-page-names}

Se recomienda la importación de nombres de página si se trabaja con un catálogo electrónico de muchas páginas. También puede importar los nombres de un archivo delimitado por tabuladores o XML.

La etiqueta TDC se almacena en el campo Datos de usuario de una imagen; formatear estos datos como una lista de `name=<value>`` pairs separated by two question marks “??” `. Por ejemplo, para establecer una etiqueta para un campo de TDC denominado tocEN &quot;, establezca los datos de usuario de la imagen en:

tocEN=&lt;EN_page_label>

Para establecer etiquetas independientes para campos de tabla de contenido con los nombres tocEN y tocFR:

tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>

Para importar el campo Datos de usuario en un archivo delimitado por tabuladores, incluya el campo userdata:

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label> |

Para importar el campo Datos de usuario en un archivo XML, incluya el atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nombres de página de un archivo delimitado por tabuladores o XML, seleccione el botón Etiquetas de tabla de contenido y elija Importar. Aparecerá el cuadro de diálogo Cargar metadatos. Haga clic en el botón Examinar e importe el archivo CSV (solo Mac) o XML que asocia cada página a un nombre de página. 
