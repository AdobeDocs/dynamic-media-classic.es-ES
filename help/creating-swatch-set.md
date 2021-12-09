---
title: Creación de un conjunto de muestras
description: Aprenda a crear un conjunto de muestras en Adobe Dynamic Media Classic.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: fe2aef174299366fc88309679ae29cc99e3d7f98
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 67%

---

# Creación de un conjunto de muestras{#creating-a-swatch-set}

Gracias a los conjuntos de muestras, los usuarios pueden ver un elemento en diferentes colores, motivos o acabados. Para crear un conjunto de muestras con muestras de color, necesitará una imagen para cada color, motivo o acabado diferente que desee incluir. También necesitará una muestra de color, motivo o acabado para cada color, motivo o acabado. 

Por ejemplo, supongamos que desea ofrecer imágenes de gorras con viseras de distintos colores; las viseras son de color rojo, verde y azul. En este caso, necesita tres tomas de la misma gorra. Necesitará una toma para la visera roja, otra para la verde y una tercera para la azul. También necesitará muestras de color en rojo, verde y azul. Las muestras de color sirven como miniaturas que los usuarios seleccionan en el visor de conjuntos de muestras para ver el gorro de facturación roja, verde o azul.

## Creación de un conjunto de muestras {#create}

Al crear un conjunto, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL Publicar después de guardar]** opción seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de muestras:**

1. Realice una de las siguientes acciones:

   * **Seleccione primero las imágenes** - En el panel Examinar, seleccione las imágenes y, a continuación, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de muestras]**.

   * **Comenzar desde la pantalla Conjunto de muestras** - Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de muestras]**. Seleccione una carpeta en la biblioteca de recursos y arrastre las imágenes a la sección Vistas de la página Conjunto de muestras.

1. Arrastre los colores, patrones o acabados de muestra al cuadro de marcador de posición Muestras de la página Conjunto de muestras.

   Asegúrese de que la muestra de color, motivo o acabado que arrastra hasta los marcadores de posición representa el color, el motivo o el acabado de la imagen adyacente.

1. Para cambiar el orden de las imágenes en su conjunto de muestras, arrastre las imágenes a su nueva ubicación.
1. Asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Select **[!UICONTROL Guardar]**, seleccione una carpeta para almacenar el conjunto de muestras de color, introduzca un nombre para el conjunto y seleccione **[!UICONTROL Submit]**.
1. Para ver el conjunto de muestras en el visor de conjuntos de muestras, seleccione **[!UICONTROL Vista previa]** en la pantalla Conjunto de muestras. Puede seleccionar miniaturas de muestra en el visor de conjuntos de muestras para ver su comportamiento.

## Edición de un conjunto de muestras {#editing-a-swatch-set}

Tanto si edita un conjunto publicado como si no, la variable **[!UICONTROL Publicar después de guardar]** afecta a los miembros de conjunto y de conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publicar después de]** guardar, opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de muestras:**

1. En la vista de cuadrícula, busque un conjunto de muestras y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Realice una de las siguientes acciones:

   * Para agregar una imagen (publicada o sin publicar), arrástrela desde una carpeta en Agregar recursos hasta la página **[!UICONTROL Vistas]** del conjunto de muestras.
   * Para quitar una imagen, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]** en la barra de herramientas.
   * Para reordenar las imágenes, arrastre cada imagen a una nueva posición.

1. Cuando haya terminado de editar el conjunto, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Select **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminación de un conjunto de muestras {#deleting-a-swatch-set}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de muestras:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione un conjunto de muestras o más.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
