---
title: Vinculación de un conjunto de giros a una página web
description: Aprenda a vincular un conjunto de giros a una página web.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Visualizadores,Conjuntos de giros
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 87%

---

# Vinculación de un conjunto de giros a una página web{#linking-a-spin-set-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server, incluidos los conjuntos de giros, mediante cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar la cadena URL o el código incrustado del conjunto de giros en las páginas web y aplicaciones, debe copiarlo desde Dynamic Media Classic.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copia de una URL de conjunto de giros {#copying-a-spin-set-url}

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **[!UICONTROL Conjunto de giros]**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el conjunto de giros cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **[!UICONTROL Copiar URL]** a la derecha del visor que desee.
   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

   * Haga clic en **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Copiar URL]**.

## Adición de direcciones URL de conjuntos de giros a una página web {#adding-spin-set-urls-to-your-web-page}

Los conjuntos de giros se distribuyen como todos los visores de zoom, a través de una página dinámica (ASP o JSP) que muestra el conjunto de giros en una ventana de zoom. La llamada de URL a la plataforma Dynamic Media Classic sigue el mismo protocolo en el visor de zoom. Sin embargo, el nombre del ajuste preestablecido de visor depende del ajuste preestablecido que el administrador haya definido como ajuste preestablecido de visor de conjuntos de giros predeterminado. Por ejemplo, el siguiente ejemplo de sintaxis de URL desactivada incluye un nombre de ajuste preestablecido denominado `viewer.jsp` y el parámetro de SKU es ahora el nombre de conjunto de giros:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

En este ejemplo de sintaxis de URL (el vínculo no está activado), fíjese en que hay un número de SKU ( `sku=backpack_spin`). La cadena que sigue a `sku=` es el nombre del conjunto de giros ( `backpack spin`).

## Copia del código incrustado de un visor de conjuntos de giros {#copying-the-embed-code-of-a-spin-set-viewer}

El uso de la función de código incrustado permite revisar el código del visor del conjunto de giros seleccionado. También puede copiar el código en el portapapeles para pegarlo en sus páginas web para la implementación del visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código incrustado de un visor de conjuntos de giros:**

1. En la lista desplegable Mostrar del panel de exploración de recursos, haga clic en **[!UICONTROL Conjunto de giros]**.
1. En el panel Biblioteca de recursos del lado izquierdo, navegue a la carpeta de recursos que contenga el conjunto de giros cuyo código incrustado desee copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL y código incrustado de la derecha, haga clic en **[!UICONTROL Código incrustado]** a la derecha del visor que desee.
   * Haga clic en **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** debajo de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

   * Haga clic en **[!UICONTROL Vista de lista]**. En el panel de exploración de recursos, seleccione un único recurso y, a continuación, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]** a la derecha de la imagen en miniatura.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

   * Haga clic en **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]** o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, haga clic en **[!UICONTROL Vista previa]** > **[!UICONTROL Lista del visor]**.

      En la página Lista del visor, en la columna Acciones de la tabla, haga clic en **[!UICONTROL Código incrustado]**.

1. En el cuadro de diálogo Código incrustado, haga clic en **[!UICONTROL Copiar al portapapeles]**.

   No se permite la edición del código en el cuadro de diálogo Código incrustado.

1. Haga clic en **[!UICONTROL Cerrar]**.
