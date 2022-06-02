---
title: Creación de un conjunto de imágenes
description: Aprenda a crear un conjunto de imágenes en Adobe Dynamic Media Classic.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: fe765d1acfa37e9d13f5ef1b655f8cf04195a8a6
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creación de un conjunto de imágenes{#creating-an-image-set}

Para crear un conjunto de imágenes con varias vistas, necesita imágenes que muestren un elemento desde distintos puntos de vista o que muestren distintos aspectos del mismo elemento. El objetivo es que las imágenes del elemento que vean los usuarios les den una idea clara de cuál es su aspecto y función.

## Creación de un conjunto de imágenes {#create}

Al crear un conjunto, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL Publicar después de guardar]** opción seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

>[!NOTE]
>
>Al crear un conjunto de imágenes, Adobe recomienda las siguientes directrices de prácticas recomendadas y límites obligatorios.
>
>* Número de recursos duplicados por conjunto de imágenes
   >   * Práctica recomendada: 20
   >   * Límite obligatorio: 20
> * Número máximo de páginas por conjunto de imágenes
   >   * Práctica recomendada: 1000
   >   * Límite ampliado: 1000


**Para crear un conjunto de imágenes:**

1. Realice una de las siguientes acciones:

   * **Seleccione primero las imágenes** - En el panel Examinar, seleccione las imágenes que desee para el conjunto de imágenes y vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de imágenes]**.

   * **Comenzar desde la pantalla Conjunto de imágenes** - Vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de imágenes]**. Aparecerá la pantalla Conjunto de imágenes. Seleccione una carpeta en la biblioteca de recursos y arrastre las imágenes que desea agregar al conjunto de imágenes a la pantalla Conjunto de imágenes.

1. Para cambiar el orden de las imágenes, arrastre cada una a su nueva ubicación.
1. Asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Select **[!UICONTROL Guardar]**, seleccione una carpeta para almacenar el conjunto de imágenes, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.
1. Para ver el conjunto de imágenes en el visualizador de conjuntos de imágenes, seleccione **[!UICONTROL Vista previa]** en la pantalla Conjunto de imágenes . Puede seleccionar miniaturas de muestra en el visor de conjuntos de imágenes para ver su comportamiento.

## Edición de un conjunto de imágenes {#editing-an-image-set}

Tanto si edita un conjunto publicado como si no, la variable **[!UICONTROL Publicar después de guardar]** afecta a los miembros de conjunto y de conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publicar después de guardar]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de imágenes:**

1. En la vista de cuadrícula, busque un conjunto de imágenes y, debajo de la imagen, seleccione **[!UICONTROL Editar]**.
1. Realice una de las siguientes acciones:

   * Para agregar una imagen (publicada o sin publicar), arrástrela desde una carpeta en Agregar recursos hasta la página **[!UICONTROL Vistas]** del conjunto de imágenes.
   * Para quitar una imagen, selecciónela y, a continuación, seleccione **[!UICONTROL Eliminar]** en la barra de herramientas.
   * Para reordenar las imágenes, arrastre cada imagen a una nueva posición.

1. Cuando haya terminado de editar el conjunto, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Select **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento para el conjunto, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un conjunto de imágenes {#deleting-an-image-set}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de imágenes:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione un conjunto de imágenes o más.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
