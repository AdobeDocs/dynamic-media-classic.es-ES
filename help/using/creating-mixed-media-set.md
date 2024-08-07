---
title: Creación de un conjunto de medios mixtos
description: Obtenga información sobre cómo crear un conjunto de medios mixtos en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Creación de un conjunto de medios mixtos{#creating-a-mixed-media-set}

Cree un conjunto de medios mixtos cuando desee combinar varios tipos de visores en una sola presentación. Asegúrese de que sus archivos, conjuntos de imágenes, conjuntos de muestras y conjuntos de giros están listos para su publicación antes de agregarlos al conjunto de medios mixtos.

![Conjunto de medios mixtos](/help/using/assets/mm_mixed_media_set.png)

## Creación de un conjunto de medios mixtos {#create-a-mixed-media-set}

Cuando crea un conjunto, la opción **Publish después de guardar** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿La opción &quot;Publish después de guardar&quot; está seleccionada antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de medios mixtos:**

1. Vaya a **[!UICONTROL Compilación]** > **[!UICONTROL Conjuntos de medios mixtos]**.
1. Arrastre los vídeos, los conjuntos de imágenes, los conjuntos de giros y las muestras de la biblioteca de recursos a la pantalla del conjunto de medios mixtos.

   >[!NOTE]
   >
   >Un conjunto de medios mixtos no admite recursos con nombres de archivo que contengan cualquiera de los siguientes caracteres: `( ) { }`.

1. Realice una de las siguientes acciones:

   * Para añadir una pista de sonido, arrastre un archivo de audio de la biblioteca de recursos al cuadro Pista de sonido. La pista de sonido se reproduce mientras se muestran las imágenes. Se detiene cuando se reproduce un vídeo.
   * Para cambiar el orden de los conjuntos, arrástrelos a nuevas ubicaciones en la pantalla Conjunto de medios mixtos. El orden de los conjuntos en la pantalla determina el orden de izquierda a derecha en que los usuarios verán los conjuntos en el visor de conjuntos de medios mixtos.
   * (Opcional) Para añadir una miniatura personalizada que represente el vídeo en el visor, arrastre el archivo de imagen desde la biblioteca de recursos hasta el cuadro de posición de miniaturas.

1. Cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish después de guardar]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**.
1. Seleccione una carpeta para almacenar el conjunto de medios mixtos y, a continuación, introduzca un nombre para el conjunto.
1. Seleccione **[!UICONTROL Guardar]**.

   Para ver el aspecto del conjunto de imágenes combinado en un visor de conjuntos de imágenes, seleccione **[!UICONTROL Vista previa]**.

## Edición de un conjunto de medios mixtos {#edit-a-mixed-media-set}

Puede editar un conjunto de medios mixtos. Si desea editar un conjunto dentro de un conjunto de medios mixtos, abra el conjunto por separado, edítelo y guárdelo. Las ediciones aparecerán en el conjunto de medios mixtos.

Tanto si edita un conjunto publicado como no publicado, la opción **[!UICONTROL Publish después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publish después de seleccionar una opción para guardar]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de medios mixtos:**

1. Seleccione el botón de rollover **[!UICONTROL Editar]** del conjunto de medios mixtos.
1. Realice una de las siguientes acciones:

   * Para quitar elementos, selecciónelos y seleccione **[!UICONTROL Eliminar]**.
   * Para reordenar elementos, arrástrelos a sus nuevas ubicaciones.

1. Cuando termine de editar el conjunto, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish después de guardar]** esté seleccionado (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como]**.

## Eliminar un conjunto de medios mixtos

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de medios mixtos:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de medios mixtos.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
