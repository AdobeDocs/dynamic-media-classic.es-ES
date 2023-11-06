---
title: "Inicio rápido: Conjuntos de giros"
description: Introducción y Inicio rápido del conjunto de giros para ayudarle a ponerse en marcha rápidamente con Adobe Dynamic Media Classic.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: faa1784e1d19b1167cad5749dc04227e3ff388e5
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 22%

---

# Inicio rápido: Conjuntos de giros{#quick-start-spin-sets}

Un conjunto de giros simula la acción física de girar un objeto para examinarlo. Los conjuntos de giros permiten ver elementos desde cualquier ángulo, por lo que se pueden obtener los detalles visuales clave de los mismos desde cualquier ángulo. Un conjunto de giros simula una visualización de 360 grados. Adobe Dynamic Media Classic ofrece conjuntos de giros unidimensionales en los que los visualizadores pueden rotar un elemento y conjuntos de giros bidimensionales en los que los visualizadores pueden rotar y voltear el elemento. Además, los usuarios pueden hacer zoom de forma libre y recorrer cualquiera de las vistas con unos pocos clics de ratón. De esta forma, los usuarios pueden examinar un elemento de cerca desde un punto de vista determinado.

![Imágenes para un conjunto de giros.](/help/using/assets/spin_set.png)

Los conjuntos de giros también aceptan mapas de imagen. Un mapa de imagen es una región de una imagen dentro de un conjunto de giros que muestra un panel de rollover con texto. Cuando el usuario selecciona un mapa de imagen, se activa un tipo de acción. Por ejemplo, se abre una página web para que el usuario pueda obtener más información sobre un producto. Para señalar un mapa de imagen en un conjunto de giros, aparece un contorno alrededor del propio mapa de imagen cuando el usuario mueve el puntero del ratón sobre él.

Consulte [Crear mapas de imagen](creating-image-maps.md).

Consulte [Conjuntos de imágenes y giros: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de formación.

Al crear un conjunto de giros, Adobe recomienda la siguiente práctica recomendada y aplica los límites siguientes:

| Tipo de límite de conjunto de giros | Práctica recomendada | Límite impuesto |
| --- | --- | --- |
| Número máximo de filas/columnas por conjunto 2D | 12 a 18 imágenes por conjunto | 1.000 |

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

Este Inicio rápido de conjuntos de giros está diseñado para ayudarle a ponerse en marcha rápidamente con las técnicas de conjuntos de giros en Adobe Dynamic Media Classic. Siga los pasos del 1 al 7. Al final de cada paso, puede seleccionar un vínculo de tema para obtener más información.

## 1. Crear y cargar las imágenes

Como mínimo, necesita 8-12 tomas de un artículo para un conjunto de giros unidimensional y 16-24 para un conjunto de giros bidimensional. Las tomas deben realizarse siguiendo intervalos regulares para dar la impresión de que se está rotando y volteando el elemento. Por ejemplo, si un conjunto de giros unidimensional incluye 12 disparos, gire el elemento 30° (360/12) para cada disparo.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar imágenes de giros desde el equipo o la red a Adobe Dynamic Media Classic.

Consulte [Instrucciones para obtener imágenes para conjuntos de giros](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Crear un conjunto de giros

Para crear un conjunto de giros, en la barra de navegación global, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de giros]**. En el cuadro de diálogo Tamaño del conjunto de giros, elija cuántas filas y celdas desea y seleccione **[!UICONTROL OK]**. A continuación, arrastre imágenes a la cuadrícula de la página Conjunto de giros.

Consulte [Creación de un conjunto de giros](creating-spin-set.md#creating-a-spin-set).

## 3. Edición de un conjunto de giros

Para editar un conjunto de giros, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de visor]**. Seleccione un conjunto de giros y, a continuación, seleccione **[!UICONTROL Editar]**. Agregue y quite las imágenes y cambie su posición. Puede cambiar la posición de las filas en los conjuntos de giros bidimensionales.

Consulte [Edición de un conjunto de giros](creating-spin-set.md#editing-a-spin-set).

## 4. Configurar ajustes preestablecidos del visor de conjuntos de giros

Los administradores pueden crear ajustes preestablecidos de visor de conjuntos de giros. Estos ajustes preestablecidos determinan el aspecto del visor de conjuntos de giros. Para configurar un nuevo ajuste preestablecido de visualizador de conjuntos de giros, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de visor]**.

En la página Ajustes preestablecidos de visor, seleccione **[!UICONTROL Añadir]**, luego seleccione **[!UICONTROL Visor de conjuntos de giros]** en la lista desplegable, y luego seleccione **[!UICONTROL Añadir]**. Elija opciones en la página Configurar visor y, a continuación, seleccione **[!UICONTROL Guardar]**.

Consulte [Configurar ajustes preestablecidos del visor de conjuntos de giros](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Previsualización de un conjunto de giros

Seleccione el conjunto de giros en el panel de exploración y, a continuación, seleccione **[!UICONTROL Previsualizar]**. En la página Vista previa, mantenga presionado el botón del mouse y arrastre el puntero a izquierda o derecha para &quot;girar&quot; visualmente el elemento.

Consulte [Previsualización de un conjunto de giros](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publicación de un conjunto de giros

Al publicar un conjunto de giros, se coloca en servidores de Adobe Dynamic Media Classic para que se pueda enviar de forma dinámica a su sitio web o aplicación. También activa la cadena URL que llama al conjunto de giros desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Para publicar un conjunto de giros, márquelo para su publicación seleccionando la variable **[!UICONTROL Marcar para publicación]** junto a su nombre en el panel Examinar. En la barra de navegación global, seleccione **[!UICONTROL Publish]** para iniciar una publicación. En la pantalla Publicar, seleccione **[!UICONTROL Enviar publicación]**.

Consulte [Publicación de un conjunto de giros](publishing-spin-set.md#publishing-a-spin-set).

## 7. Vinculación de un juego de giros a una página web

Adobe Dynamic Media Classic crea cadenas de llamada de URL para conjuntos de giros y las activa después de publicarlas. Puede copiar estas direcciones URL desde la página de vista previa.

Seleccione el conjunto de giros y, a continuación, seleccione **[!UICONTROL Previsualizar]**. Seleccione un ajuste preestablecido de visor de conjuntos de giros. A continuación seleccione **[!UICONTROL Copiar URL]**.

Consulte [Vinculación de un conjunto de giros a una página web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
