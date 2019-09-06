---
title: Vinculación de un conjunto de giros a una página web
seo-title: Vinculación de un conjunto de giros a una página web
description: nulo
seo-description: Descubra cómo vincular un conjunto de giros a una página web.
uuid: d 3 c 5773 e -60 c 4-4 e 8 b -9 c 48-e 1 e 3 eb 8028 d 0
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/spin_ sets
discoiquuid: 651 b 21 ef-e 322-4 e 6 d -8 e 37-45 ffd 56 f 7 a 58
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Vinculación de un conjunto de giros a una página web{#linking-a-spin-set-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido del servidor de imágenes de Dynamic Media, incluidos los conjuntos de giros, a través de cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar la cadena URL o código incrustado del conjunto de giros en las páginas web y las aplicaciones, debe copiar esta cadena desde Scene7 Publishing System.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copia de una URL de conjunto de giros {#copying-a-spin-set-url}

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **Conjunto de giros**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el conjunto de giros cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **Copiar URL** a la derecha del visor que desee.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** &gt; **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Copiar URL**.

## Adición de direcciones URL de conjuntos de giros a una página web {#adding-spin-set-urls-to-your-web-page}

Los conjuntos de giros se distribuyen como todos los visores de zoom, a través de una página dinámica (ASP o JSP) que muestra el conjunto de giros en una ventana de zoom. La llamada mediante URL a la plataforma Dynamic Media Classic sigue el mismo protocolo en el visor de zoom. Sin embargo, el nombre del ajuste preestablecido de visor depende del ajuste preestablecido que el administrador haya definido como ajuste preestablecido de visor de conjuntos de giros predeterminado. Por ejemplo, el siguiente ejemplo de sintaxis de URL desactivada incluye un nombre de ajuste preestablecido denominado `viewer.jsp` y el parámetro de SKU es ahora el nombre de conjunto de giros:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

En este ejemplo de sintaxis de URL (el vínculo no está activado), fíjese en que hay un número de SKU ( `sku=backpack_spin`). The string after `sku=` is the Spin Set name ( `backpack spin`).

## Copia del código incrustado de un visor de conjuntos de giros {#copying-the-embed-code-of-a-spin-set-viewer}

El uso de la función de código incrustado permite revisar el código del visor del conjunto de giros seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de conjuntos de giros**

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **Conjunto de giros**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el conjunto de giros cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **Código incrustado** a la derecha del visor que desee.
   * Haga clic en **Vista de cuadrícula**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de lista**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **Vista previa** &gt; **Lista del visor** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

   * Haga clic en **Vista de cuadrícula**, **Vista de lista** o **Vista de detalles**. En la misma barra de herramientas, haga clic en **Vista previa** &gt; **Lista del visor**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **Código incrustado**.

1. En el cuadro de diálogo Código incrustado, haga clic en **Copiar al portapapeles**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Haga clic en Cerrar.

