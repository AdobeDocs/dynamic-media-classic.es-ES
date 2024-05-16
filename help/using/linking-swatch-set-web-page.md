---
title: Vinculación de un conjunto de muestras a una página web
description: Obtenga información sobre cómo vincular un conjunto de muestras a una página web en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 16%

---

# Vinculación de un conjunto de muestras a una página web{#linking-a-swatch-set-to-a-web-page}

Después de publicar un conjunto de muestras, puede utilizar su dirección URL asociada o código incrustado en el sitio web o la aplicación. A continuación, puede implementar la dirección URL o el código incrustado según sea necesario para que los usuarios puedan ver el conjunto de muestras en el sitio web o la aplicación.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copiar una URL de conjunto de muestras {#copying-a-swatch-set-url}

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de muestras]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de muestras cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL e Código incrustado de la derecha, seleccione **[!UICONTROL Copiar URL]** a la derecha del visor que desee.
   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]**, o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

## Añadir URL del conjunto de muestras a la página web {#adding-swatch-set-urls-to-your-web-page}

La forma más común de implementar Conjuntos de muestras es colocar un vínculo (mediante un icono de navegación) en la página web. Cuando se selecciona, el vínculo inicia una página dinámica (ASP o JSP) que muestra el conjunto de muestras en una ventana de zoom emergente. El vínculo de zoom abre una ventana emergente que contiene la función de zoom real.

Para obtener más información y ejemplos de código, consulte [Incrustación del visor de zoom HTML5 en la Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copia del código de incrustación de un visor de conjuntos de muestras {#copying-the-embed-code-of-a-swatch-set-viewer}

El uso de la función de código incrustado permite revisar el código del visor del conjunto de muestras seleccionado. También puede copiar el código en el portapapeles para pegarlo en las páginas web y así poder implementar el visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código de incrustación de un visor de conjuntos de muestras:**

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de muestras]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de muestras cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL e Código incrustado de la derecha, seleccione **[!UICONTROL Código incrustado]** a la derecha del visor que desee.
   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccionar **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]**, o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Seleccionar **[!UICONTROL Cerrar]**.

>[!MORELIKETHIS]
>
>* [Publish](publishing-files.md#publishing_files)
