---
title: Vincular visualizadores de zoom a las páginas web
description: Aprenda a vincular visores de zoom a sus páginas web en Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# Vincular visualizadores de zoom a las páginas web{#linking-zoom-viewers-to-your-web-pages}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server, incluidas las imágenes principales y los destinos de zoom asociados, y los ajustes preestablecidos de visor de zoom, mediante cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar estas cadenas URL o el código incrustado en sus páginas web y aplicaciones, debe copiarlas desde Adobe Dynamic Media Classic.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copiar una URL del visor de zoom {#copying-a-zoom-viewer-url}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el visor de zoom cuya URL desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]** o **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, seleccione **[!UICONTROL Copiar URL]** a la derecha del visor que desee.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un único recurso y, a continuación, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccione **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un único recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

## Añadir direcciones URL del visor de zoom a la página web {#adding-zoom-viewer-urls-to-your-web-page}

Normalmente, los visitantes hacen zoom de las imágenes en un sitio web seleccionando primero un icono de Zoom (a menudo, el icono muestra la imagen de una lupa). Si se selecciona este icono, se inicia una página web dinámica (ASP o JSP) que muestra la imagen en una ventana emergente. Es en esta ventana emergente donde los visitantes aplican zoom en la imagen.

Para obtener más información y ejemplos de código, consulte [Embed HTML5 Basic Zoom Viewer in the Adobe Viewers Reference Guide](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copiar la copia incrustada de un visor de zoom {#copying-the-embed-copy-of-a-zoom-viewer}

El uso de la función de código incrustado permite revisar el código del visor de zoom seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de zoom:**

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el visor de zoom cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, seleccione **[!UICONTROL Código incrustado]** a la derecha del visor que desee.
   * Seleccione **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un único recurso y, a continuación, debajo de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccione **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un único recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

   * Seleccione **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      En la página Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, seleccione **[!UICONTROL Copiar al portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Seleccione **[!UICONTROL Cerrar]**.
