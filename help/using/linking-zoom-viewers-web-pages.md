---
title: Vinculación de visores de zoom a sus páginas web
description: Aprenda a vincular visores de zoom a sus páginas web en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 23%

---

# Vinculación de visores de zoom a sus páginas web{#linking-zoom-viewers-to-your-web-pages}

Sus sitios web y aplicaciones acceden al contenido del servidor de imágenes de Dynamic Media mediante cadenas URL o código incrustado. Ese acceso incluye imágenes principales y destinos de zoom asociados. También incluye ajustes preestablecidos del visor de zoom. Estas cadenas URL se activan durante el proceso de publicación. Para colocar estas cadenas URL o el código incrustado en las páginas Web y aplicaciones, cópielas desde Adobe Dynamic Media Classic.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copiar una URL de visor de zoom {#copying-a-zoom-viewer-url}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el visor de zoom cuya URL desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado que se encuentra a la derecha, seleccione **[!UICONTROL Copiar dirección URL]** a la derecha del visor que desee.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

## Añadir URL del visor de zoom a la página web {#adding-zoom-viewer-urls-to-your-web-page}

Normalmente, los visitantes hacen zoom de las imágenes de un sitio web seleccionando primero un icono de Zoom (a menudo el icono muestra la imagen de una lupa). Al seleccionar este icono, se inicia una página Web dinámica (ASP o JSP) que muestra la imagen en una ventana emergente. Es en esta ventana emergente donde los visitantes aplican zoom en la imagen.

Para obtener más detalles y ejemplos de código, consulte [Incrustar visor de zoom básico de HTML5 en la Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/es/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiar la copia incrustada de un visor de zoom {#copying-the-embed-copy-of-a-zoom-viewer}

El uso de la función de código incrustado permite revisar el código del visor de zoom seleccionado. También puede copiar el código en el portapapeles para pegarlo en las páginas web y así poder implementar el visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de zoom:**

1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el visor de zoom cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel Direcciones URL e Código incrustado que se encuentra a la derecha, seleccione **[!UICONTROL Código incrustado]** a la derecha del visor que desee.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccionar **[!UICONTROL vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista de visualizadores]**.

     En la página Lista de visores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al Portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Seleccione **[!UICONTROL Cerrar]**.
