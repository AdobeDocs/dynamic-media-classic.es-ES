---
title: Creación de un conjunto de ofertas
seo-title: Creación de un conjunto de ofertas
description: nulo
seo-description: Descubra cómo crear un conjunto de ofertas.
uuid: 6 d 6 a 4 af 9-70 c 0-4 cfa -9 a 8 f -855 d 6 adfcc 8 f
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 59 b 6437 d-c 21 e -4929-9291-3032 dbb 34565
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Creación de un conjunto de ofertas{#creating-an-offer-set}

Se puede crear cualquiera de los siguientes tipos de conjuntos de ofertas:

* Vídeo
* Plantilla parametrizada
* Imagen

For templates, click **Add and Preview**, then set the parameters you choose. Los otros tipos de conjuntos de ofertas no incluyen parámetros pero, aun así, se pueden personalizar haciendo clic en **Vista previa** y cambiando los ajustes preestablecidos disponibles.

Dynamic Media Classic ofrece herramientas para editarlas y crear conjuntos de ofertas.

>[!NOTE]
>
>Antes de crear un conjunto de ofertas, asegúrese de publicar todos los recursos que vaya a utilizar para el conjunto en Scene 7 Publishing System. Consulte [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Se puede crear un conjunto de ofertas de cualquiera de los siguientes tipos:

**Imágenes** Puede montar imágenes para un conjunto de ofertas. Cada imagen incluye una oferta distinta en el conjunto.

**Plantilla** Imagen Puede parametrizar plantillas de imagen en Dynamic Media Classic con el comando Generar &gt; Funciones básicas de plantilla. Mediante parámetros, se pueden intercambiar y personalizar los componentes de la plantilla como el texto de los cuadros de texto y las distintas imágenes. Para un conjunto de ofertas, puede utilizar parámetros de plantilla para crear variaciones de la misma imagen en el conjunto de ofertas, por ejemplo. Para obtener más información sobre la creación y la parametrización de plantillas de imagen, consulte Creación de parámetros de plantilla.

**Vídeo** Puede montar vídeo para un conjunto de ofertas. Cada vídeo conforma una oferta distinta en el conjunto.

## Creación de conjuntos de ofertas con una plantilla parametrizada {#creating-an-offer-set-with-a-parameterized-template}

Al crear un conjunto de ofertas, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con una plantilla parametrizada**

1. Seleccione la plantilla o la pancarta.
1. Click **Build** &gt; **Target Classic Offer Set**.

   La página Conjuntos de ofertas de Target Classic enumera las ofertas del conjunto de ofertas. El primer elemento de la lista es el objeto.

1. Seleccione el objeto y haga clic en **Agregar y previsualizar**.

   En la parte izquierda de esta página, se muestran los parámetros de la plantilla y sus valores.

1. Cambie los valores de los parámetros para crear la oferta. Por ejemplo, introduzca otro texto en el campo de texto, cambie el tamaño de una capa, intercambie una imagen por otra, o bien seleccione otro ajuste preestablecido de visor.
1. Haga clic en **Guardar** o en **Guardar como** para guardar la oferta como parte del conjunto de ofertas.

   La página Conjunto de ofertas de Target Classic enumera las ofertas creadas.

1. Repita los pasos del 3 al 5 para crear más ofertas para el conjunto.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Antes de cerrar la página Conjunto de ofertas de Target Classic, inserte el conjunto de ofertas en Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Al crear un conjunto de ofertas, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Se ha seleccionado la opción “Publicar después de guardar” antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con imágenes o vídeos**

1. Monte imágenes o vídeos para el conjunto de ofertas. Comience en la pantalla Conjunto de ofertas de Target Classic o en la Vista de cuadrícula o de Lista y utilice uno de los métodos siguientes:

   **Pantalla Conjunto de ofertas de Target Classic** Haga clic en Generar &gt; Conjunto de ofertas de Target Classic. Arrastre las imágenes o los vídeos a la pantalla. Para crear vídeos o imágenes de distintos tamaños, arrastre varias copias de la imagen o del vídeo y defina cada tamaño de manera individual.

   **Vista de cuadrícula o de lista** Seleccione las imágenes o los vídeos y haga clic en Generar &gt; Conjunto de ofertas de Target Classic.

1. Si lo desea, seleccione una imagen o un vídeo y haga clic en **Vista previa**. En la página Vista previa de ofertas, puede cambiar el tamaño y el aspecto de la imagen o del vídeo seleccionado. O bien, puede cambiar todas las imágenes o los vídeos del conjunto de ofertas.

   * Elija un valor preestablecido para cambiar el aspecto y el tamaño de la imagen o del vídeo.
   * Haga clic en la casilla de verificación de selección de ajustes preestablecidos para todas con el fin de aplicar los ajustes que elija a todas las ofertas del conjunto de ofertas.
   Haga clic en **Guardar** para guardar los cambios en la oferta de imagen o vídeo. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Haga clic en **Guardar**, especifique un nombre para el conjunto de ofertas y haga clic en **Guardar**.

Antes de cerrar la página Conjunto de ofertas de Target Classic, inserte el conjunto de ofertas en Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Edición de un conjunto de ofertas {#editing-an-offer-set}

Según si edita un conjunto publicado o sin publicar, la opción **Publicar después de guardar** afecta al conjunto y a los miembros del conjunto de las siguientes formas:

| ¿Ya se ha publicado el conjunto? | ¿Se ha seleccionado la opción “Publicar después de Guardar” antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
|--- |--- |--- |--- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros existentes del conjunto conservan su estado publicado. Todos los miembros nuevos que agregue durante la edición conservarán su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de ofertas**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. En la página Conjunto de ofertas de Target Classic, realice una de las siguientes acciones:

   **Eliminación de una oferta**

   Select the offer, and then click **Delete** to remove an offer from the set.

   **Adición de una oferta**

   El modo de agregar una oferta depende del tipo de conjunto de ofertas con el que trabaje:

   * Templates: Click **Add &amp; Preview**, and on the Add &amp; Preview Offers page, create another offer.
   * Imágenes y vídeos: Arrastre una imagen o un vídeo a la página Conjuntos de ofertas de Target Classic.
   ***Nota**: No puede eliminar un conjunto de ofertas asociado a una campaña. Para eliminar un conjunto de ofertas asociado a una campaña, inicie sesión en Target Classic y elimine primero las asociaciones de campañas. Even after un-associating from a campaign, the asset can only be deleted from Scene7 Publishing System, requiring a login to Target Classic, and not from within Target Classic.*

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Haga clic en **Guardar**, seleccione una carpeta de almacenamiento, especifique un nombre para el conjunto y haga clic en **Guardar**.

## Eliminación de un conjunto de ofertas {#deleting-an-offer-set}

Cuando se elimina un conjunto de ofertas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o “elementos secundarios”) dentro de dicho conjunto no se verán afectados; cada uno mantendrá su estado existente de publicación o no.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de ofertas**

1. En la vista de cuadrícula, la vista de lista o la vista de detalles, seleccione uno o varios conjuntos de ofertas.
1. En la barra de navegación global, haga clic en **Archivo** &gt; **Eliminar** &gt; **Eliminar**.

>[!MORELIKETHIS]
>
>* [Creación de parámetros de plantilla](creating-template-parameters.md#creating_template_parameters)

