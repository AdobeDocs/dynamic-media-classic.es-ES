---
title: Creación de un conjunto de ofertas
description: Obtenga información sobre cómo crear un conjunto de ofertas.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 52%

---

# Creación de un conjunto de ofertas{#creating-an-offer-set}

Se puede crear cualquiera de los siguientes tipos de conjuntos de ofertas:

* Vídeo
* Plantilla parametrizada
* Imagen

Para las plantillas, haga clic en **[!UICONTROL Agregar y previsualizar]** y, a continuación, establezca los parámetros que elija. Los otros tipos de conjuntos de ofertas no incluyen parámetros pero, aun así, se pueden personalizar haciendo clic en **[!UICONTROL Vista previa]** y cambiando los ajustes preestablecidos disponibles.

Dynamic Media Classic ofrece herramientas para editar y crear conjuntos de ofertas.

>[!NOTE]
>
>Antes de crear un conjunto de ofertas, asegúrese de publicar en Dynamic Media Classic todos los recursos que desee utilizar para el conjunto. Consulte [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Se puede crear un conjunto de ofertas de cualquiera de los siguientes tipos:

* **Imágenes** : puede ensamblar imágenes para un conjunto de ofertas. Cada imagen incluye una oferta diferente en el conjunto.

* **Plantilla de imagen** : puede parametrizar las plantillas de imagen en Dynamic Media Classic con el comando Generar > Conceptos básicos de plantilla. Mediante parámetros, se pueden intercambiar y personalizar los componentes de la plantilla como el texto de los cuadros de texto y las distintas imágenes. Para un conjunto de ofertas, puede utilizar parámetros de plantilla para crear variaciones de la misma imagen en el conjunto de ofertas, por ejemplo. Para obtener más información sobre la creación y la parametrización de plantillas de imagen, consulte Creación de parámetros de plantilla.

* **Vídeo** : puede ensamblar vídeo para un conjunto de ofertas. Cada vídeo conforma una oferta distinta en el conjunto.

## Creación de un conjunto de ofertas con una plantilla parametrizada {#creating-an-offer-set-with-a-parameterized-template}

Al crear un conjunto de ofertas, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con una plantilla parametrizada:**

1. Seleccione la plantilla o el banner.
1. Haga clic en **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de ofertas de Test&amp;Target]**. 

   La página Conjunto de ofertas de Test&amp;Target enumera las ofertas del conjunto de ofertas. El primer elemento de la lista es el objeto.

1. Seleccione el objeto y haga clic en **[!UICONTROL Agregar y previsualizar]**.

   En la parte izquierda de esta página, se muestran los parámetros de la plantilla y sus valores.

1. Cambie los valores de los parámetros para crear la oferta. Por ejemplo, introduzca otro texto en el campo de texto, cambie el tamaño de una capa, intercambie una imagen por otra, o bien seleccione otro ajuste preestablecido de visor.
1. Haga clic en **[!UICONTROL **Guardar]** o **[!UICONTROL Guardar como**]** para guardar la oferta como parte del conjunto de ofertas.

   La página Conjunto de ofertas de Test&amp;Target enumera las ofertas que ha creado.

1. Repita los pasos del 3 al 5 para crear más ofertas para el conjunto.
1. Cuando termine, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publish after save*]** esté seleccionado (predeterminado).
1. Haga clic en **[!UICONTROL Cerrar]**, introduzca un nombre para el conjunto de ofertas y, a continuación, haga clic en **[!UICONTROL Guardar]**.

Antes de cerrar la página de conjunto de ofertas de Test&amp;Target , inserte el conjunto de ofertas en Adobe Target Standard/Premium. Consulte [Transferencia de conjuntos de ofertas a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creación de un conjunto de ofertas con imágenes o vídeos {#creating-an-offer-set-with-images-or-videos}

Al crear un conjunto de ofertas, la opción **[!UICONTROL Publicar después de guardar]** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| **[!UICONTROL ¿Publicar después de]** guardar está seleccionada la opción antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con imágenes o vídeos:**

1. Ensamble imágenes o vídeos para el conjunto de ofertas. Comience en la pantalla Conjunto de ofertas de Test&amp;Target o en la vista de cuadrícula o de lista y utilice uno de los métodos siguientes:

   * **Pantalla**  del conjunto de ofertas de Test&amp;Target: haga clic en  **[!UICONTROL Generar]**  > Conjunto de ofertas de  **[!UICONTROL Test&amp;Target]**. Arrastre las imágenes o los vídeos a la pantalla. Para crear vídeos o imágenes de distintos tamaños, arrastre varias copias de la imagen o del vídeo y defina cada tamaño de manera individual.

   * **Vista de cuadrícula o vista**  de lista: seleccione las imágenes o los vídeos y, a continuación, haga clic en  **[!UICONTROL Generar]**  > Conjunto de ofertas de  **[!UICONTROL Test&amp;Target]**.

1. Si lo desea, seleccione una imagen o un vídeo y haga clic en **[!UICONTROL Vista previa]**. En la página Ofertas de vista previa , puede cambiar el tamaño y el aspecto de la imagen o del vídeo que ha seleccionado. O bien, puede cambiar todas las imágenes o vídeos del conjunto de ofertas.

   * Elija un valor preestablecido para cambiar el aspecto y el tamaño de la imagen o del vídeo.
   * Para aplicar el ajuste preestablecido que ha elegido a todas las ofertas del conjunto de ofertas, haga clic en la casilla de verificación **[!UICONTROL Seleccionar ajustes preestablecidos a todos]**.

   Haga clic en **[!UICONTROL Guardar]** para guardar los cambios en la oferta de imagen o vídeo. A continuación, haga clic en **[!UICONTROL Cerrar]** para volver a la pantalla Conjuntos de ofertas de Test&amp;Target.

1. Cuando termine de crear ofertas para el conjunto de ofertas y de elegir Ajustes preestablecidos de imagen para diferentes imágenes, asegúrese de que **[!UICONTROL Publish after save]** esté seleccionado (predeterminado).
1. Haga clic en **[!UICONTROL Guardar]**, especifique un nombre para el conjunto de ofertas y haga clic en **[!UICONTROL Guardar]**.

Antes de cerrar la página de conjunto de ofertas de Test&amp;Target, inserte el conjunto de ofertas en Adobe Target Standard/Premium. Consulte [Transferencia de conjuntos de ofertas a Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Edición de un conjunto de ofertas {#editing-an-offer-set}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL ¿Publicar después de]** guardar una opción seleccionada antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservarán su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de ofertas:**

1. Para editar un conjunto de ofertas, muestre el conjunto de ofertas en la vista de cuadrícula o de lista y, a continuación, haga clic en su botón de sustitución **[!UICONTROL Edit]**.
1. En la página Conjunto de ofertas de Test&amp;Target , realice una de las acciones siguientes:

   * **Eliminación de una oferta** : seleccione la oferta y, a continuación, haga clic en  **** Eliminar para eliminar una oferta del conjunto.
   * **Adición de una oferta** : la forma de añadir una oferta depende del tipo de conjunto de ofertas con el que esté trabajando:
      * **Plantillas** : haga clic en  **[!UICONTROL Agregar y previsualizar]** y, en la página Agregar y previsualizar ofertas, cree otra oferta.
      * **Imágenes y vídeos** : arrastre una imagen o un vídeo a la página Conjunto de ofertas de Test&amp;Target.

   >[!NOTE]
   >
   >No puede eliminar un conjunto de ofertas que esté asociado a una campaña. Para eliminar un conjunto de ofertas asociado a una campaña, inicie sesión en Adobe Target Standard/Premium y elimine primero las asociaciones de campañas. Incluso después de desasociar de una campaña, el recurso solo se puede eliminar de Dynamic Media Classic, lo que requiere iniciar sesión en Adobe Target Standard/Premium, y no desde Adobe Target Standard/Premium.

1. Cuando termine de editar, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar]** esté seleccionado (predeterminado).
1. Haga clic en **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **[!UICONTROL Guardar]**.

## Eliminación de un conjunto de ofertas {#deleting-an-offer-set}

Cuando se elimina un conjunto de ofertas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de ofertas:**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de ofertas.
1. En la barra de navegación global, haga clic en **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **Eliminar**.

>[!MORELIKETHIS]
>
>* [Creación de parámetros de plantilla](creating-template-parameters.md#creating_template_parameters)

