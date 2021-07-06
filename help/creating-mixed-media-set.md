---
title: Creación de un conjunto de medios mixtos
description: Aprenda a crear un conjunto de medios mixtos.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Visualizadores,Conjuntos de medios mixtos
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: f99832bc9660a16b06e63b19f9ead1267dab0f35
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 88%

---

# Creación de un conjunto de medios mixtos{#creating-a-mixed-media-set}

Cree un conjunto de medios mixtos cuando desee combinar varios tipos de visores en una sola presentación. Asegúrese de que sus archivos, conjuntos de imágenes, conjuntos de muestras y conjuntos de giros están listos para su publicación antes de agregarlos al conjunto de medios mixtos.

![Conjunto de medios mixtos](/help/assets/mm_mixed_media_set.png)

## Creación de un conjunto de medios mixtos {#create-a-mixed-media-set}

Al crear un conjunto, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de medios mixtos:**

1. Haga clic en **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de medios mixtos]**.
1. Arrastre los vídeos, los conjuntos de imágenes, los conjuntos de giros y las muestras de la biblioteca de recursos a la pantalla del conjunto de medios mixtos.

   >[!NOTE]
   >
   >Un conjunto de medios mixtos no admite recursos con nombres de archivo que contengan cualquiera de los siguientes caracteres: `( ) { }`.

1. Realice una de las siguientes acciones:

   * Para añadir una pista de sonido, arrastre un archivo de audio de la biblioteca de recursos al cuadro Pista de sonido. La pista de sonido se reproduce mientras se muestran las imágenes. Se detiene cuando se reproduce vídeo.
   * Para cambiar el orden de los conjuntos, arrástrelos a nuevas ubicaciones en la pantalla Conjunto de medios mixtos. El orden de los conjuntos en la pantalla determina el orden de izquierda a derecha en que los usuarios verán los conjuntos en el visor de conjuntos de medios mixtos.
   * (Opcional) Para añadir una miniatura personalizada que represente el vídeo en el visor, arrastre el archivo de imagen desde la biblioteca de recursos hasta el cuadro de posición de miniaturas.

1. Asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **[!UICONTROL Guardar]**, seleccione una carpeta para almacenar su conjunto de medios mixtos, escriba un nombre para el conjunto y haga clic en **[!UICONTROL Guardar]**.

   Para ver el aspecto del conjunto de imágenes combinado en un visualizador de conjuntos de imágenes, haga clic en **[!UICONTROL Vista previa]**.

## Edición de un conjunto de medios mixtos {#edit-a-mixed-media-set}

Puede editar un conjunto de medios mixtos. Si desea editar un conjunto dentro de un conjunto de medios mixtos, abra el conjunto por separado, edítelo y guárdelo. Los cambios aparecen en el conjunto de medios mixtos.

Tanto si edita un conjunto publicado como si no, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de medios mixtos:**

1. Haga clic en el botón de rollover **[!UICONTROL Editar]** del conjunto de medios mixtos.
1. Realice una de las siguientes acciones:

   * Para eliminar elementos, selecciónelos y haga clic en **[!UICONTROL Eliminar]**.
   * Para reordenar elementos, arrástrelos a sus nuevas ubicaciones.

1. Cuando haya terminado de editar el conjunto, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como]**.

## Eliminación de un conjunto de medios mixtos {#deleting-a-mixed-media-set}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de medios mixtos:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de medios mixtos.
1. En la barra de navegación global, haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
