---
title: Vinculación de un conjunto de giros a una página web
description: Obtenga información sobre cómo vincular un conjunto de giros a una página web en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 23%

---

# Vinculación de un conjunto de giros a una página web{#linking-a-spin-set-to-a-web-page}

Los sitios web y las aplicaciones acceden al contenido de Dynamic Media Image Server, incluidos los conjuntos de giros, mediante cadenas URL o código incrustado. Estas cadenas URL se activan durante el proceso de publicación. Para colocar la cadena URL o el código incrustado del conjunto de giros en las páginas web y aplicaciones, cópielo desde Adobe Dynamic Media Classic.

>[!NOTE]
>
>La URL no se activa hasta que publique el recurso.

## Copiar una URL de conjunto de giros {#copying-a-spin-set-url}

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de giros]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de giros cuyo código incrustado desea copiar.
1. Encima del panel de exploración de recursos, en la parte derecha de la barra de herramientas, realice una de las siguientes acciones:

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel de exploración de recursos, haga doble clic en un único recurso para abrirlo en la vista de detalles. En el panel URL e Código incrustado de la derecha, seleccione **[!UICONTROL Copiar URL]** a la derecha del visor que desee.
   * Seleccionar **[!UICONTROL Vista de cuadrícula]**. En el panel Examinar recursos, seleccione un solo recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL Vista de lista]**. En el panel Examinar recursos, seleccione un solo recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

   * Seleccionar **[!UICONTROL Vista de cuadrícula]**, **[!UICONTROL Vista de lista]**, o **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

     En la página Lista de visualizadores, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]**.

## Añadir URL de conjuntos de giros a la página web {#adding-spin-set-urls-to-your-web-page}

Los conjuntos de giros se distribuyen como todos los visores de zoom, a través de una página dinámica (ASP o JSP) que muestra el conjunto de giros en una ventana de zoom. La llamada URL a la plataforma de Adobe Dynamic Media Classic sigue el mismo protocolo en el visor de zoom. Sin embargo, el nombre del ajuste preestablecido de visor depende del ajuste preestablecido que el administrador haya definido como ajuste preestablecido de visor de conjuntos de giros predeterminado. Por ejemplo, el siguiente ejemplo de sintaxis de URL no activa incluye un nombre de ajuste preestablecido denominado `viewer.jsp` y el parámetro SKU es ahora el nombre del conjunto de giros:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

En este ejemplo de sintaxis de URL (el vínculo no está activo), observe un número SKU ( `sku=backpack_spin`). La cadena después de `sku=` es el nombre del conjunto de giros ( `backpack spin`).

## Copiar el código de incrustación de un visor de conjuntos de giros {#copying-the-embed-code-of-a-spin-set-viewer}

El uso de la función de código incrustado permite revisar el código del visor del conjunto de giros seleccionado. También puede copiar el código en el portapapeles para pegarlo en las páginas web y así poder implementar el visor. No se permite la edición del código en el cuadro de diálogo Código incrustado.

**Para copiar el código de incrustación de un visor de conjuntos de giros:**

1. En el panel Examen de recursos, en la lista desplegable Mostrar, seleccione **[!UICONTROL Conjunto de giros]**.
1. en el panel Biblioteca de recursos de la izquierda, vaya a la carpeta de recursos que contiene el conjunto de giros cuyo código incrustado desea copiar.
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
