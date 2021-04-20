---
title: Vinculación de visores de zoom a páginas web
description: Aprenda a vincular visores de zoom a sus páginas web.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 84%

---


# Vinculación de visores de zoom a páginas web{#linking-zoom-viewers-to-your-web-pages}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server, incluidas las imágenes principales y los destinos de zoom asociados, y los ajustes preestablecidos de visor de zoom, mediante cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar estas cadenas URL o el código incrustado en sus páginas web y aplicaciones, debe copiarlas desde Dynamic Media Classic.

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

Para obtener más información y ejemplos de código, consulte [Incrustación del visor de zoom básico HTML5 en la Guía de referencia de visores de Adobe](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

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

1. Haga clic en **Cerrar**.
