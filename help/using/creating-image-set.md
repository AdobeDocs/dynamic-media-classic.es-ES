---
title: Creación de un conjunto de imágenes
description: Obtenga información sobre cómo crear un conjunto de imágenes en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 38%

---

# Creación de un conjunto de imágenes{#creating-an-image-set}

Para crear un conjunto de imágenes con varias vistas, necesita imágenes que muestren un elemento desde distintos puntos de vista o que muestren distintos aspectos del mismo elemento. El objetivo es que las imágenes del elemento que vean los usuarios les den una idea clara de cuál es su aspecto y función.

## Creación de un conjunto de imágenes {#create}

Cuando crea un conjunto, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Se seleccionó la opción **[!UICONTROL `Publish after a save`]** antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

Al crear un conjunto de imágenes, Adobe recomienda las siguientes prácticas recomendadas y aplica los límites siguientes:

| Tipo de límite | Práctica recomendada | Límite impuesto |
| --- | --- | --- |
| Número de recursos duplicados por conjunto | No hay duplicados | 20 ‡ |
| Número máximo de imágenes por conjunto | 5-10 imágenes por conjunto | 1.000 |

‡ práctica recomendada es no tener recursos duplicados en un conjunto. El límite es de 20 duplicados para un solo recurso. Si, dentro del conjunto, agrega otro duplicado para ese recurso, la solicitud generará un error o ignorará el duplicado.

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

**Para crear un conjunto de imágenes:**

1. Realice una de las siguientes acciones:

   * **Seleccione las imágenes primero**: en el panel Examinar, seleccione las imágenes que desee para su conjunto de imágenes y vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de imágenes]**.

   * **Empiece desde la pantalla del conjunto de imágenes**: Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de imágenes]**. Aparecerá la pantalla Conjunto de imágenes. Seleccione una carpeta en la biblioteca de recursos y arrastre las imágenes que desea agregar al conjunto de imágenes a la pantalla Conjunto de imágenes.

1. Para cambiar el orden de las imágenes, arrastre cada una a su nueva ubicación.
1. Cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta para almacenar su conjunto de imágenes, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.
1. Para ver tu conjunto de imágenes en el visor de conjuntos de imágenes, selecciona **[!UICONTROL Vista previa]** en la pantalla Conjunto de imágenes. Puede seleccionar miniaturas de muestra en el visualizador de conjuntos de imágenes para ver cómo se comportan.

## Edición de un conjunto de imágenes {#editing-an-image-set}

Tanto si edita un conjunto publicado como no publicado, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | ¿Ha seleccionado la opción **[!UICONTROL `Publish after a save`]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de imágenes:**

1. En la vista de cuadrícula, busque un conjunto de imágenes y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Realice una de las siguientes acciones:

   * Para agregar una imagen (publicada o no publicada), arrástrela desde una carpeta en Agregar Assets a la página **[!UICONTROL Vistas]** del conjunto de imágenes.
   * Para quitar una imagen, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]** en la barra de herramientas.
   * Para reordenar las imágenes, arrastre cada imagen a una nueva posición.

1. Cuando haya terminado de editar el conjunto, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar]** esté seleccionado (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento para el conjunto, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un conjunto de imágenes

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de imágenes:**

1. En la vista Cuadrícula, Vista de lista o Vista de detalles, seleccione un conjunto de imágenes o más.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
