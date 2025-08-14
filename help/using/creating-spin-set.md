---
title: Creación de un conjunto de giros
description: Obtenga información sobre cómo crear un conjunto de giros en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 32%

---

# Creación de un conjunto de giros{#creating-a-spin-set}

Si desea crear un conjunto de giros eficaz, asegúrese de tomar las imágenes correctamente. Puede crear un conjunto de giros en Adobe Dynamic Media Classic seleccionando el botón Generar y seleccionando Conjuntos de giros. Edite los conjuntos de giros en la pantalla Conjunto de giros.

>[!NOTE]
>
>Las versiones anteriores de Adobe Dynamic Media Classic no ofrecían conjuntos de giros bidimensionales. Si creó un conjunto de giros en una versión anterior de Adobe Dynamic Media Classic, guárdelo con un nombre diferente y, a continuación, podrá guardar el conjunto de giros unidimensional. Seleccione **[!UICONTROL Guardar como]** en la pantalla del conjunto de giros e introduzca un nombre nuevo para poder editarlo en Adobe Dynamic Media Classic.

## Instrucciones para obtener imágenes para conjuntos de giros {#guidelines-for-shooting-spin-set-images}

En general, cuantas más imágenes tenga en un conjunto de giros, mejor será el efecto de giro de la imagen. Sin embargo, si se incluyen muchas imágenes en el conjunto también se aumentará el tiempo que tardan en cargarse las imágenes. Adobe Dynamic Media Classic recomienda estas directrices para grabar imágenes para utilizarlas en conjuntos de giros:

* Como mínimo, utilice 8-12 imágenes en un conjunto de giros unidimensional y 16-24 imágenes en un conjunto de giros bidimensional.
* Utilice un formato sin pérdida; se recomiendan TIFF y PNG.
* Aplique máscara a todas las imágenes para que el elemento aparezca en un fondo blanco puro o con otro color de alto contraste. Si lo desea, agregue sombras.
* Asegúrese de que los detalles del producto están bien iluminados y enfocados.
* Tome las imágenes de giro para las prendas de ropa con un maniquí o una persona. A menudo, el maniquí está enmascarado (usando un maniquí de vidrio) o se muestra un maniquí estilizado/dressform en la imagen. Se puede crear un conjunto de giros en modelo definiendo el número de ángulos. Marque cada ángulo con cinta en el suelo para que pueda guiar al modelo para que avance y mire en la dirección de cada disparo.

## Creación de un conjunto de giros {#create}

El orden en que se crea o crea el conjunto de giros en Adobe Dynamic Media Classic es importante. Según la forma en que ordene los recursos al arrastrar y soltar imágenes en la cuadrícula de la página Conjunto de giros, el conjunto de giros girará en una dirección determinada. Por lo tanto, el orden en el que se muestra visualmente en el generador es el giro del recurso cuando un usuario mueve el puntero del mouse o el dedo, de izquierda a derecha.

Cuando crea un conjunto, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| **[!UICONTROL Publicar después de seleccionar la opción Guardar]** antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

Al crear un conjunto de giros, Adobe recomienda la siguiente práctica recomendada y aplica el siguiente límite:

| Tipo de límite de conjunto de giros | Práctica recomendada | Límite impuesto |
| --- | --- | --- |
| Número máximo de filas/columnas por conjunto 2D | 12 a 18 imágenes por conjunto | 1.000 |

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

Después de guardar un conjunto de giros, use la opción Vista previa de la página Generar: Conjunto de giros para comprobar el aspecto del conjunto de giros en el visor predeterminado.

**Para crear un conjunto de giros:**

1. En el menú desplegable **[!UICONTROL Generar]**, seleccione **[!UICONTROL Conjuntos de giros]**.
1. En el cuadro de diálogo Tamaño del conjunto de giros, defina el número de filas y celdas que desee.

   Para crear un conjunto de giros unidimensional, seleccione solo una fila.

   Para crear un conjunto de giros de dos dimensiones, seleccione dos filas o más.

1. Seleccione **[!UICONTROL Aceptar]**.
1. Arrastre las imágenes y suéltelas en la cuadrícula de la pantalla Conjunto de giros.
1. Cuando termine, cerca de la esquina inferior derecha de la página, asegúrese de que **Publicar después de guardar** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**.
1. En el cuadro de diálogo Guardar, seleccione una carpeta para almacenar el conjunto de giros. En el campo Nombre de archivo, introduzca el nombre del conjunto de giros.
1. Seleccione **[!UICONTROL Guardar]**.

## Edición de un conjunto de giros {#editing-a-spin-set}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publicar después de seleccionar la opción Guardar]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para editar un conjunto de giros:**

1. Seleccione el botón de rollover **[!UICONTROL Editar]** del conjunto de giros.
1. Realice una de las siguientes acciones:

   * **Eliminando imágenes**: Seleccione la imagen y, a continuación, seleccione **[!UICONTROL Eliminar]**.

   * **Agregando imágenes**: arrastre la imagen a una celda.

   * **Reordenación de filas (conjuntos de giros bidimensionales)**: seleccione un cuadro de selector de fila (a la izquierda de la fila) y, a continuación, seleccione **[!UICONTROL Bajar fila]** o **[!UICONTROL Subir fila]**.

   * **Agregar filas y celdas**: Escriba un número en el cuadro Filas y en el cuadro Celdas para determinar el número de filas y el número de celdas de cada fila.

1. Cuando termine de editar, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminación de un conjunto de giros

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para eliminar un conjunto de giros:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de giros.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **[!UICONTROL Eliminar]**.
