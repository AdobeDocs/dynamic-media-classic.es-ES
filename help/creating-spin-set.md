---
title: Creación de un conjunto de giros
description: Obtenga información sobre cómo crear un conjunto de giros.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 74%

---


# Creación de un conjunto de giros{#creating-a-spin-set}

Si desea crear un conjunto de giros eficaz, asegúrese de tomar las imágenes correctamente. Para crear un conjunto de giros en Dynamic Media Classic, seleccione el botón Generar y elija Conjuntos de giros. Edite los conjuntos de giros en la pantalla Conjunto de giros.

>[!NOTE]
>
>Las versiones anteriores de Dynamic Media Classic no hacían ofertas de conjuntos de giros bidimensionales. Si ha creado un conjunto de giros en una versión anterior de Dynamic Media Classic, no podrá guardar el conjunto de giros unidimensional sin guardarlo primero con otro nombre. Haga clic en Guardar como en la pantalla Conjunto de giros e introduzca un nuevo nombre para poder editarlo en Dynamic Media Classic.

## Instrucciones para obtener imágenes para conjuntos de giros {#guidelines-for-shooting-spin-set-images}

Por normal general, cuantas más imágenes tenga un conjunto de giros, mejor será el efecto de giro. Sin embargo, si se incluyen muchas imágenes en el conjunto también se aumentará el tiempo que tardan en cargarse las imágenes. Dynamic Media Classic recomienda estas pautas para la toma de imágenes para su uso en conjuntos de giros:

* Como mínimo, utilice entre 8 y 12 imágenes en un conjunto de giros unidimensional y entre 16 y 24 imágenes en un conjunto de giros bidimensional.
* Utilice un formato sin pérdida; se recomiendan TIFF y PNG.
* Aplique máscara a todas las imágenes para que el elemento aparezca en un fondo blanco puro o con otro color de alto contraste. Si lo desea, agregue sombras.
* Asegúrese de que los detalles del producto están bien iluminados y enfocados.
* Tome las imágenes de giro para las prendas de ropa con un maniquí o una persona. El maniquí suele ocultarse por completo (mediante el uso de un maniquí de cristal); también se puede mostrar un maniquí o busto estilizado en la imagen. Puede crear un conjunto de giros con persona definiendo el número de ángulos. Marque cada ángulo en el suelo con cinta adhesiva para indicar a la persona dónde debe colocarse y hacia dónde debe mirar en cada toma. 

## Creación de un conjunto de giros  {#create}

Tenga en cuenta que es importante el orden en que se crea o se crea el conjunto de giros en Dynamic Media Classic. Dependiendo del orden de los recursos al arrastrar y colocar imágenes en la cuadrícula de la pantalla Conjunto de giros, el conjunto girará en una dirección determinada. Por consiguiente, el orden en que se ve en el generador es la forma en que el recurso gira cuando un usuario mueve el puntero del ratón o mueve el dedo, de izquierda a derecha.

Al crear un conjunto, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

Después de guardar un conjunto de giros, use la opción Vista previa de la página Generar: Conjunto de giros para comprobar el aspecto del conjunto de giros en el visor predeterminado.

**Para crear un conjunto de giros**

1. En el menú desplegable **Generar**, haga clic en **Conjuntos de giros**.
1. En el cuadro de diálogo Tamaño del conjunto de giros, defina el número de filas y celdas que desee.

   Para crear un conjunto de giros de una dimensión, seleccione solo una fila.

   Para crear un conjunto de giros de dos dimensiones, seleccione dos filas o más.

1. Haga clic en **Aceptar**.
1. Arrastre las imágenes y suéltelas en la cuadrícula de la pantalla Conjunto de giros.
1. Cuando haya terminado, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**.
1. En el cuadro de diálogo Guardar, seleccione la carpeta en la que desee almacenar el conjunto de giros. En el campo Nombre de archivo, escriba el nombre del conjunto de giros.
1. Haga clic en **Guardar**.

## Edición de un conjunto de giros  {#editing-a-spin-set}

Según si edita un conjunto publicado o sin publicar, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservan su estado publicado.Los nuevos miembros del conjunto que haya agregado durante la edición conservarán su estado publicado o sin publicar. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para editar un conjunto de giros**

1. Haga clic en el botón de rollover **Editar** del conjunto de giros.
1. Realice una de las siguientes acciones:

   * **Eliminación de**
imágenesSeleccione la imagen y, a continuación, haga clic en 
**Eliminar**.

   * **Añadir**
imágenesArrastre la imagen a una celda.

   * **Reordenación de filas (conjuntos de giros bidimensionales)**
Haga clic en un cuadro de selección de filas (a la izquierda de la fila) y, a continuación, haga clic en 
**Mover fila** abajo  **Subir fila**.

   * **Añadir filas y**
celdasIntroduzca un número en el cuadro Filas y el cuadro Celdas para determinar el número de filas y el número de celdas en cada fila.

1. Cuando haya terminado con su edición, asegúrese de que esté seleccionada la opción **Publicar después de guardar** (predeterminada), cerca de la esquina inferior derecha de la página.
1. Haga clic en **Guardar**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **Guardar**.

## Eliminación de un conjunto de giros  {#deleting-a-spin-set}

Cuando se elimina un conjunto, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually-publishing-assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually-unpublishing-assets).

**Para eliminar un conjunto de giros**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de giros.
1. En la barra de navegación global, haga clic en **Archivo** > **Eliminar** > **Eliminar**.

