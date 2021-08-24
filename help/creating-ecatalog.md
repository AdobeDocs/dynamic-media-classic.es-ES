---
title: Crear un catálogo electrónico
description: Aprenda a crear un catálogo electrónico en Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Visualizadores,Catálogo electrónico
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 57%

---

# Creación de un catálogo electrónico {#creating-an-ecatalog}

Al crear un catálogo electrónico es preciso ordenar las páginas, elegir su presentación y vincular las páginas mediante mapas de imagen y datos de vínculos de hipertexto y de rollover. Si lo desea, también puede personalizar la tabla de contenido para que los usuarios vean nombres de página en lugar de números en el visor de catálogos electrónicos.

## Crear un catálogo electrónico {#create}

Puede incluir archivos de imagen y archivos PDF en el catálogo electrónico.

Al crear un catálogo electrónico, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un catálogo electrónico:**

1. Comience la creación del catálogo electrónico utilizando una de estas técnicas:

   * **Seleccione los archivos primero** : en el panel Examinar, seleccione archivos y, a continuación, vaya a  **[!UICONTROL Generar]**  >  **[!UICONTROL Catálogos electrónicos]**.

   * **Comience desde la pantalla**  Catálogo electrónico: vaya a  **[!UICONTROL Generar]**  >  **[!UICONTROL Catálogos electrónicos]**. Seleccione una carpeta en la biblioteca de recursos y arrastre los archivos deseados a la ficha Ordenar páginas que se encuentra en la página Catálogo electrónico.

      >[!NOTE]
      >
      >Para ver los elementos de la biblioteca de recursos por su nombre en lugar de ver las miniaturas, seleccione la opción Nombre en la vista de biblioteca de recursos predeterminada en Ajustes personales.

1. Seleccione la presentación general que tendrá el catálogo electrónico. Seleccione **[!UICONTROL 1 Up]** para páginas individuales, **[!UICONTROL 2 Up]** para pliegos de doble página o **[!UICONTROL Personalizado]** para pliegos de páginas de más de dos páginas. En el cuadro de diálogo **[!UICONTROL Cambiar diseño del catálogo electrónico]**, seleccione las opciones **[!UICONTROL Todas las distribuciones]** y seleccione **[!UICONTROL Aceptar]**.
1. Opcionalmente, puede cambiar el diseño de páginas individuales o de pliegos de páginas seleccionándolas y luego eligiendo el botón **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** o **[!UICONTROL Custom]**. En el cuadro de diálogo **[!UICONTROL Cambiar diseño del catálogo electrónico]**, seleccione las opciones **[!UICONTROL Difusiones seleccionadas]** y seleccione **[!UICONTROL Aceptar]**.
1. Reordene las páginas según sea necesario con una de estas técnicas:

   * **Arrastrar** : arrastre una página o página a una nueva ubicación. La barra vertical muestra el lugar al que se ha movido la página.

   * **Botón Mover a** : seleccione una página o un pliego de páginas, seleccione  **[!UICONTROL Mover a]** y elija la página en el menú que desea que su página aparezca antes.

   * **Secuencia #**  - En la vista de lista, introduzca los números de página en los campos Número de secuencia.

1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el catálogo electrónico. En el campo Nombre de archivo, escriba el nombre del conjunto de giros.
1. Seleccione **[!UICONTROL Guardar]**.

   Puede obtener una vista previa del catálogo electrónico, después de guardarlo, seleccionando **[!UICONTROL Preview]**.

## Editar un catálogo electrónico {#editing-an-ecatalog}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un catálogo electrónico:**

1. Seleccione el botón **[!UICONTROL Edit]** de sustitución del catálogo electrónico.
1. Realice los cambios necesarios.
1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un catálogo electrónico {#deleting-an-ecatalog}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un catálogo electrónico:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios catálogos electrónicos.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.

## Personalización de la tabla de contenido (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic proporciona números de página predeterminados en el catálogo electrónico en la ficha Ordenar páginas de la pantalla Catálogo electrónico. Si desea personalizar el nombre de las páginas, puede cambiar las etiquetas de las páginas que forman la tabla de contenido (TOC). Se recomienda cambiar el nombre de la portada y la contraportada. Por ejemplo, la portada puede decir &quot;Portada&quot; en lugar de &quot;Página 0-1&quot;.

Puede crear una tabla de contenido (TOC) personalizada para el catálogo electrónico manualmente o importando los nombres de las páginas de un archivo CSV (solo Mac) o XML.

>[!NOTE]
>
>Para restaurar los títulos de página predeterminados, en la ficha **[!UICONTROL Ordenar páginas]**, seleccione **[!UICONTROL Etiquetas de tabla de contenido]** y, a continuación, seleccione **[!UICONTROL Restaurar predeterminados (todos)]**.

### Introducción manual de nombres de página {#manually-entering-page-names}

Para introducir manualmente nombres de página uno por uno, vaya a la ficha Ordenar páginas de la pantalla Catálogo electrónico. A continuación, en el campo número de página , introduzca un nombre para cada página que desee nombrar.

### Importar nombres de páginas {#importing-page-names}

Se recomienda la importación de nombres de página si se trabaja con un catálogo electrónico de muchas páginas. También puede importar los nombres de un archivo delimitado por tabuladores o XML.

La etiqueta TOC se almacena en el campo Datos de usuario de una imagen; formatee estos datos como una lista de `name=<value>` ` pairs separated by two question marks “??” `. Por ejemplo, para establecer una etiqueta para una tabla de contenido con el nombre `tocEN`, establezca los datos de usuario de la imagen en:

`tocEN=&lt;EN_page_label>`

Para establecer etiquetas independientes para campos de TDC llamados `tocEN` y `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Para importar el campo Datos de usuario en un archivo delimitado por tabuladores, incluya los datos del usuario del campo:

| IPSID | Datos de usuario |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Para importar el campo Datos de usuario en un archivo XML, incluya el atributo `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Para importar nombres de páginas de un archivo XML o delimitado por tabuladores, seleccione el botón **[!UICONTROL Etiquetas de tabla de contenido]** y seleccione **[!UICONTROL Importar]**. En el cuadro de diálogo Cargar metadatos, seleccione **[!UICONTROL Examinar]** y, a continuación, importe el archivo CSV (solo Mac) o el archivo XML que asocia cada página con un nombre de página.
