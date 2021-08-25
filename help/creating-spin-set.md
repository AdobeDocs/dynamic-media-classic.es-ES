---
title: Crear un conjunto de giros
description: Aprenda a crear un conjunto de giros en Dynamic Media Classic.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 56%

---

# Crear un conjunto de giros{#creating-a-spin-set}

Si desea crear un conjunto de giros eficaz, asegúrese de tomar las imágenes correctamente. Para crear un conjunto de giros en Dynamic Media Classic, seleccione el botón Generar y elija Conjuntos de giros. Edite los conjuntos de giros en la pantalla Conjunto de giros.

>[!NOTE]
>
>Las versiones anteriores de Dynamic Media Classic no ofrecían conjuntos de giros bidimensionales. Si ha creado un conjunto de giros en una versión anterior de Dynamic Media Classic, no puede guardar el conjunto de giros unidimensional sin guardarlo primero con un nombre diferente. Seleccione **[!UICONTROL Guardar como]** en la pantalla Conjunto de giros e introduzca un nuevo nombre para poder editarlo en Dynamic Media Classic.

## Instrucciones para obtener imágenes para conjuntos de giros {#guidelines-for-shooting-spin-set-images}

Por normal general, cuantas más imágenes tenga un conjunto de giros, mejor será el efecto de giro. Sin embargo, si se incluyen muchas imágenes en el conjunto también se aumentará el tiempo que tardan en cargarse las imágenes. Dynamic Media Classic recomienda estas directrices para la grabación de imágenes para su uso en conjuntos de giros:

* Como mínimo, utilice entre 8 y 12 imágenes en un conjunto de giros unidimensional y entre 16 y 24 imágenes en un conjunto de giros bidimensional.
* Utilice un formato sin pérdida; se recomiendan TIFF y PNG.
* Aplique máscara a todas las imágenes para que el elemento aparezca en un fondo blanco puro o con otro color de alto contraste. Si lo desea, agregue sombras.
* Asegúrese de que los detalles del producto están bien iluminados y enfocados.
* Tome las imágenes de giro para las prendas de ropa con un maniquí o una persona. A menudo el maniquí está enmascarado (usando un maniquí de vidrio) o un maniquí estilizado/forma de vestir se muestra en la imagen. Puede crear un conjunto de giros con persona definiendo el número de ángulos. Marque cada ángulo con cinta en el suelo para que pueda guiar al modelo para que se desplace y mire en la dirección de cada toma.

## Crear un conjunto de giros {#create}

Es importante el orden en que se crea o crea el conjunto de giros en Dynamic Media Classic. Dependiendo del orden de los recursos al arrastrar y colocar imágenes en la cuadrícula de la pantalla Conjunto de giros, el conjunto girará en una dirección determinada. Por lo tanto, el orden en el que se muestra visualmente en el generador es el modo en que se envía el recurso cuando un usuario mueve el puntero del ratón o mueve el dedo, de izquierda a derecha.

Al crear un conjunto, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL ¿Publicar después de]** guardar está seleccionada la opción antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

Después de guardar un conjunto de giros, use la opción Vista previa de la página Generar: Conjunto de giros para comprobar el aspecto del conjunto de giros en el visor predeterminado.

**Para crear un conjunto de giros:**

1. En el menú desplegable **[!UICONTROL Build]**, seleccione **[!UICONTROL Conjuntos de giros]**.
1. En el cuadro de diálogo Tamaño del conjunto de giros, defina el número de filas y celdas que desee.

   Para crear un conjunto de giros de una dimensión, seleccione solo una fila.

   Para crear un conjunto de giros de dos dimensiones, seleccione dos filas o más.

1. Seleccione **[!UICONTROL OK]**.
1. Arrastre las imágenes y suéltelas en la cuadrícula de la pantalla Conjunto de giros.
1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el conjunto de giros. En el campo Nombre de archivo, escriba el nombre del conjunto de giros.
1. Seleccione **[!UICONTROL Guardar]**.

## Editar un conjunto de giros {#editing-a-spin-set}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL ¿Publicar después de]** guardar una opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para editar un conjunto de giros:**

1. Seleccione el botón de rollover **[!UICONTROL Editar]** del conjunto de giros.
1. Realice una de las siguientes acciones:

   * **Eliminación de imágenes** : seleccione la imagen y, a continuación, seleccione  **[!UICONTROL Eliminar]**.

   * **Adición de imágenes** : arrastre la imagen a una celda.

   * **Reordenación de filas (conjuntos de giros bidimensionales)** : seleccione un cuadro de selector de filas (a la izquierda de la fila) y, a continuación, seleccione  **[!UICONTROL Mover fila]** o  **[!UICONTROL Subir fila]**.

   * **Adición de filas y celdas** : introduzca un número en el cuadro Filas y el cuadro Celdas para determinar el número de filas y el número de celdas en cada fila.

1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **[!UICONTROL Publicar después de guardar]** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, introduzca un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un conjunto de giros {#deleting-a-spin-set}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para eliminar un conjunto de giros:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de giros.
1. En la barra de navegación global, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
