---
title: Vinculación de un conjunto de imágenes a una página web
description: Obtenga información sobre cómo vincular un conjunto de imágenes a una página web en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 17%

---

# Vinculación de un conjunto de imágenes a una página web{#linking-an-image-set-to-a-web-page}

Después de publicar un conjunto de imágenes, puede copiar su dirección URL asociada o su código incrustado para utilizarlos en el sitio web o la aplicación. A continuación, puede implementar la dirección URL o pegar el código incrustado según sea necesario para que los usuarios puedan ver el conjunto de imágenes en el sitio web o la aplicación.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copiar una URL de conjunto de imágenes {#copying-an-image-set-url}

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de imágenes]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de imágenes cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado que se encuentra a la derecha, seleccione **[!UICONTROL Copiar dirección URL]** a la derecha del visor que desee.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

## Adición de direcciones URL de conjuntos de imágenes a la página web {#adding-image-set-urls-to-your-web-page}

La forma más común de implementar conjuntos de imágenes es colocar un vínculo (mediante un icono de navegación) en la página web. Cuando se selecciona, el vínculo inicia una página dinámica (JSP) que muestra el conjunto de imágenes en una ventana de zoom emergente. El vínculo de zoom abre una ventana emergente que contiene la función de zoom real.

Para obtener más detalles y ejemplos de código, consulte [Incrustar visor de zoom HTML5 en la Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/es/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiar el código de incrustación de un visor de conjuntos de imágenes {#copying-the-embed-code-of-an-image-set-viewer}

El uso de la función de código incrustado permite revisar el código del visor del conjunto de imágenes seleccionado. También puede copiar el código en el portapapeles para pegarlo en las páginas web y así poder implementar el visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de conjunto de imágenes:**

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de imágenes]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de imágenes cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL de la derecha, seleccione **[!UICONTROL Código incrustado]**.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al Portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Seleccione **[!UICONTROL Cerrar]**.

>[!MORELIKETHIS]
>
>* [Publicar](publishing-files.md#publishing_files)
