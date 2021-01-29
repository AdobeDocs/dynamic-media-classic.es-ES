---
title: Vinculación de visores de zoom a páginas web
description: Descubra cómo vincular los visores de zoom a sus páginas web.
uuid: cd350ea4-267e-4a8a-aed8-7553df86b438
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: df5471c1-ccda-4dd4-a7f1-5b9193b41f98
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 86%

---


# Vinculación de visores de zoom a páginas web{#linking-zoom-viewers-to-your-web-pages}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server, incluidas las imágenes principales y los destinatarios de zoom asociados, así como a los ajustes preestablecidos de visor de zoom, a través de cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar estas cadenas URL o el código incrustado en las páginas web y las aplicaciones, debe copiarlas desde Dynamic Media Classic.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copia de una URL de visor de zoom  {#copying-a-zoom-viewer-url}

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el visor de zoom cuya URL desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula** o **Vista de lista**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **Copiar URL** a la derecha del visor que desee.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** > **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

## Adición de direcciones URL de visores de zoom a una página web  {#adding-zoom-viewer-urls-to-your-web-page}

Normalmente, los visitantes de un sitio web aplican zoom en las imágenes seleccionando primero un icono de zoom (representado por un icono de lupa, por lo general). Si se selecciona este icono, se inicia una página web dinámica (ASP o JSP) que muestra la imagen en una ventana emergente. Es en esta ventana emergente donde los visitantes aplican zoom en la imagen.

Para obtener más información y ejemplos de código, consulte [Incrustación del visor de zoom básico HTML5 en la Guía de referencia de visores de Adobe](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html).

## Copia de la copia incrustada de un visor de zoom {#copying-the-embed-copy-of-a-zoom-viewer}

El uso de la función de código incrustado permite revisar el código del visor de zoom seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de zoom**

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el visor de zoom cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **Código incrustado** a la derecha del visor que desee.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** > **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** > **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

1. En el cuadro de diálogo Código incrustado, haga clic en **Copiar al portapapeles**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Haga clic en Cerrar.

