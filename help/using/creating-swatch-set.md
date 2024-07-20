---
title: Creación de un conjunto de muestras
description: Obtenga información sobre cómo crear un conjunto de muestras en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# Creación de un conjunto de muestras{#creating-a-swatch-set}

Gracias a los conjuntos de muestras, los usuarios pueden ver un elemento en diferentes colores, motivos o acabados. Para crear un conjunto de muestras con muestras de color, necesitará una imagen para cada color, motivo o acabado diferente que desee incluir. También necesitará una muestra de color, motivo o acabado para cada color, motivo o acabado. 

Por ejemplo, supongamos que desea ofrecer imágenes de gorras con viseras de distintos colores; las viseras son de color rojo, verde y azul. En este caso, necesita tres tomas de la misma gorra. Necesitará una toma para la visera roja, otra para la verde y una tercera para la azul. También necesitará muestras de color en rojo, verde y azul. Las muestras de color sirven como miniaturas que los usuarios seleccionan en el Visor de conjuntos de muestras para ver el límite rojo, verde o azul.

## Creación de un conjunto de muestras {#create}

Cuando crea un conjunto, la opción **Publish después de guardar** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| **[!UICONTROL Publish después de seleccionar una opción de guardar]** antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de muestras:**

1. Realice una de las siguientes acciones:

   * **Seleccione las imágenes primero**: en el panel Examinar, seleccione las imágenes y, a continuación, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de muestras]**.

   * **Empiece desde la pantalla del conjunto de muestras**: Vaya a **[!UICONTROL Compilación]** > **[!UICONTROL Conjuntos de muestras]**. Seleccione una carpeta en la biblioteca de recursos y arrastre las imágenes a la sección Vistas de la página Conjunto de muestras.

1. Arrastre los colores, patrones o acabados de muestra al cuadro de marcador de posición Muestras de la página Conjunto de muestras.

   Asegúrese de que la muestra de color, motivo o acabado que arrastra hasta los marcadores de posición representa el color, el motivo o el acabado de la imagen adyacente.

1. Para cambiar el orden de las imágenes en su conjunto de muestras, arrastre las imágenes a su nueva ubicación.
1. Cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish después de guardar]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta para almacenar su conjunto de muestras de muestras de color, escriba un nombre para el conjunto y seleccione **[!UICONTROL Enviar]**.
1. Para ver tu conjunto de muestras en el visor de conjuntos de muestras, selecciona **[!UICONTROL Vista previa]** en la pantalla del conjunto de muestras. Puede seleccionar miniaturas de muestra en el Visor de conjuntos de muestras para ver cómo se comportan.

## Edición de un conjunto de muestras {#editing-a-swatch-set}

Tanto si edita un conjunto publicado como no publicado, la opción **[!UICONTROL Publish después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publish después de seleccionar una opción de guardado]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado. |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado. |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de muestras:**

1. En la vista de cuadrícula, busque un conjunto de muestras y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Realice una de las siguientes acciones:

   * Para agregar una imagen (publicada o no publicada), arrástrela desde una carpeta en Agregar Assets a la página **[!UICONTROL Vistas]** del conjunto de muestras.
   * Para quitar una imagen, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]** en la barra de herramientas.
   * Para reordenar las imágenes, arrastre cada imagen a una nueva posición.

1. Cuando termine de editar el conjunto, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish después de guardar]** esté seleccionado (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminación de un conjunto de muestras

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de muestras:**

1. En la vista de cuadrícula, vista de lista o vista de detalles, seleccione un conjunto de muestras o más.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
