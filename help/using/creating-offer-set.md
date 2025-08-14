---
title: Crear un conjunto de ofertas
description: Obtenga información sobre cómo crear un conjunto de ofertas en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# Crear un conjunto de ofertas {#creating-an-offer-set}

Puede crear cualquiera de los siguientes tipos de conjuntos de ofertas:

* Vídeo
* Plantilla parametrizada
* Imagen

Para las plantillas, seleccione **[!UICONTROL Agregar y previsualizar]** y, a continuación, establezca los parámetros que elija. Otros tipos de conjuntos de ofertas no incluyen parámetros, pero puedes personalizarlos seleccionando **[!UICONTROL Vista previa]** y cambiando los ajustes preestablecidos disponibles.

Adobe Dynamic Media Classic ofrece herramientas para editar y crear conjuntos de ofertas.

>[!NOTE]
>
>Antes de crear un conjunto de ofertas, asegúrese de publicar en Adobe Dynamic Media Classic todos los recursos que pretenda utilizar para el conjunto. Consulte [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

## Tipos de conjuntos de ofertas {#types-of-offer-sets}

Cree un conjunto de ofertas a partir de los siguientes tipos de conjuntos de ofertas:

* **Imágenes**: puede combinar imágenes para un conjunto de ofertas. Cada imagen incluye una oferta diferente en el conjunto.

* **Plantilla de imagen**: puede parametrizar plantillas de imagen en Adobe Dynamic Media Classic con el comando **[!UICONTROL Generar]** > Conceptos básicos de plantilla. Mediante parámetros, componentes de la plantilla, el texto en marcos de texto, las diferentes imágenes, se pueden intercambiar y personalizar. Para un conjunto de ofertas, puede utilizar parámetros de plantilla para crear variaciones en la misma imagen del conjunto de ofertas, por ejemplo. Para obtener información sobre cómo crear y parametrizar plantillas de imagen, consulte [Crear parámetros de plantilla](creating-template-parameters.md#creating_template_parameters).

Vea también [Fundamentos de la plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de formación.

* **Vídeo**: puede combinar vídeo para un conjunto de ofertas. Cada vídeo conforma una oferta distinta en el conjunto.

## Creación de un conjunto de ofertas con una plantilla con parámetros {#creating-an-offer-set-with-a-parameterized-template}

Cuando crea un conjunto de ofertas, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| **[!UICONTROL Publicar después de seleccionar la opción Guardar]** antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con una plantilla con parámetros:**

1. Seleccione la plantilla o el banner.
1. Vaya a **[!UICONTROL Compilación]** > **[!UICONTROL Conjunto de ofertas de Test&amp;Target]**.

   La página Conjunto de ofertas de Test&amp;Target enumera las ofertas del conjunto de ofertas. El primer elemento de la lista es el objeto.

1. Seleccione el objeto y seleccione **[!UICONTROL Agregar y previsualizar]**.

   En la parte izquierda de esta página, se muestran los parámetros de la plantilla y sus valores.

1. Cambie los valores de los parámetros para crear la oferta. Por ejemplo, introduzca un texto diferente en un campo de texto, cambie el tamaño de una capa, cambie una imagen por otra o elija un ajuste preestablecido de visor diferente.
1. Seleccione **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como**]** para guardar la oferta como parte del conjunto de ofertas.

   La página Conjunto de ofertas de Test&amp;Target enumera las ofertas que ha creado.

1. Repita los pasos del 3 al 5 para crear más ofertas para el conjunto.
1. Cuando termine, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar*]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Cerrar]**, escriba un nombre para el conjunto de ofertas y, a continuación, seleccione **[!UICONTROL Guardar]**.

Antes de cerrar la página Conjunto de ofertas de Test&amp;Target, inserte el conjunto de ofertas en Adobe Target Standard/Premium. Consulte [Insertar conjuntos de ofertas en Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creación de un conjunto de ofertas con imágenes o vídeos {#creating-an-offer-set-with-images-or-videos}

Cuando crea un conjunto de ofertas, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| **[!UICONTROL Publicar después de seleccionar la opción Guardar]** antes de guardar? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- |
| Sí | Publicado | Publicado |
| No | Sin publicar | Los miembros del conjunto conservan su estado publicado o no. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para crear un conjunto de ofertas con imágenes o vídeos:**

1. Organice imágenes o vídeos para el conjunto de ofertas. Comience en la pantalla del conjunto de ofertas de Test&amp;Target o en la vista de cuadrícula o la vista de lista y utilice uno de los siguientes métodos:

   * **Pantalla del conjunto de ofertas de Test&amp;Target**: Ir a **[!UICONTROL Generar]** > **[!UICONTROL Conjunto de ofertas de Test&amp;Target]**. Arrastre las imágenes o los vídeos a la pantalla. Para crear vídeos o imágenes de distintos tamaños, arrastre varias copias de la imagen o del vídeo y defina cada tamaño de manera individual.

   * **Vista de cuadrícula o Vista de lista**: selecciona las imágenes o los vídeos y, a continuación, ve a **[!UICONTROL Generar]** > **[!UICONTROL Conjunto de ofertas de Test&amp;Target]**.

1. Si lo desea, seleccione una imagen o un vídeo y seleccione **[!UICONTROL Vista previa]**. En la página Vista previa de ofertas, puede cambiar el tamaño y el aspecto de la imagen o el vídeo que ha seleccionado. O bien, puede cambiar todas las imágenes o vídeos del conjunto de ofertas.

   * Elija un valor preestablecido para cambiar el aspecto y el tamaño de la imagen o del vídeo.
   * Para aplicar el ajuste preestablecido que eligió a todas las ofertas del conjunto de ofertas, active la casilla de verificación **[!UICONTROL Seleccionar ajustes preestablecidos para todos]**.

   Seleccione **[!UICONTROL Guardar]** para guardar los cambios en la oferta de imagen o vídeo. A continuación, seleccione **[!UICONTROL Cerrar]** para volver a la página del conjunto de ofertas de Test&amp;Target.

1. Cuando termine de crear ofertas para el conjunto de ofertas y de elegir ajustes preestablecidos de imagen para distintas imágenes, asegúrese de que la opción **[!UICONTROL Publicar después de guardar]** esté seleccionada (opción predeterminada).
1. Seleccione **[!UICONTROL Guardar]**, escriba un nombre para el conjunto de ofertas y seleccione **[!UICONTROL Guardar]**.

Antes de cerrar la página de conjuntos de ofertas de Test&amp;Target, inserte el conjunto de ofertas en Adobe Target Standard/Premium. Consulte [Insertar conjuntos de ofertas en Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Editar un conjunto de ofertas {#editing-an-offer-set}

Tanto si edita un conjunto publicado como un conjunto sin publicar, la opción **[!UICONTROL Publicar después de guardar]** afecta a los miembros del conjunto y del conjunto de las siguientes maneras:

| ¿Ya se ha publicado el conjunto? | **[!UICONTROL Publicar después de seleccionar la opción Guardar]** antes de guardar la edición? | Estado del conjunto después de guardar | Estado de los miembros del conjunto después de guardar |
| --- | --- | --- | --- |
| Sí | Sí | Publicado | Publicado |
| Sí | No | Publicado | Los miembros del conjunto existentes conservan su estado publicado. Cualquier nuevo miembro que añada al conjunto durante la edición conservará su estado publicado o no publicado. |
| No | Sí | Publicado | Publicado |
| No | No | Sin publicar | Los miembros existentes del conjunto y cualquier nuevo miembro que añada al conjunto durante la edición conservarán su estado publicado o no publicado. |

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para editar un conjunto de ofertas:**

1. Para editar un conjunto de ofertas, muéstrelo en la vista de cuadrícula o de lista y, a continuación, seleccione el botón de rollover **[!UICONTROL Editar]**.
1. En la página Conjunto de ofertas de Test&amp;Target, realice una de las acciones siguientes:

   * **Eliminando una oferta**: Seleccione la oferta y, a continuación, seleccione **[!UICONTROL Eliminar]** para eliminar una oferta del conjunto.
   * **Agregar una oferta**: La forma de agregar una oferta depende del tipo de conjunto de ofertas con el que esté trabajando:
      * **Plantillas**: selecciona **[!UICONTROL Agregar y previsualizar]** y en la página Agregar y previsualizar ofertas crea otra oferta.
      * **Imágenes y vídeos**: arrastre una imagen o un vídeo a la página Conjunto de ofertas de Test&amp;Target.

   >[!NOTE]
   >
   >No puede eliminar un conjunto de ofertas asociado a una campaña. Para eliminar un conjunto de ofertas asociado a una campaña, inicie sesión en Adobe Target Standard/Premium y elimine primero las asociaciones de campañas. Incluso después de desasociarse de una campaña, el recurso solo se puede eliminar de Adobe Dynamic Media Classic, por lo que se requiere un inicio de sesión en Adobe Target Standard/Premium y no desde Adobe Target Standard/Premium.

1. Cuando termine de editar, cerca de la esquina inferior derecha de la página, asegúrese de que **[!UICONTROL Publicar después de guardar]** está seleccionado (predeterminado).
1. Seleccione **[!UICONTROL Guardar]**, seleccione una carpeta de almacenamiento, escriba un nombre para el conjunto y, a continuación, seleccione **[!UICONTROL Guardar]**.

## Eliminar un conjunto de ofertas {#delet-an-offer-set}

Cuando se elimina un conjunto de ofertas, el conjunto en sí se mueve a la papelera. Sin embargo, los miembros (o &quot;hijos&quot;) de ese conjunto no se ven afectados, sino que cada uno de ellos conserva su estado publicado o no publicado.

Consulte también [Publicación manual de recursos](publishing-files.md#manually_publishing_assets) y [Cancelación manual de la publicación de recursos](publishing-files.md#manually_unpublishing_assets).

**Para eliminar un conjunto de ofertas:**

1. En la vista de cuadrícula, vista de lista o vista de detalles, seleccione un conjunto de ofertas o más.
1. En la barra de navegación global, ve a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]** > **Eliminar**.

>[!MORELIKETHIS]
>
>* [Creando parámetros de plantilla](creating-template-parameters.md#creating_template_parameters)
