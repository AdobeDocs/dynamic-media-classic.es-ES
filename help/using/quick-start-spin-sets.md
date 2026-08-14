---
title: 'Inicio rápido: Conjuntos de giros'
description: Introducción y Inicio rápido del conjunto de giros para ayudarle a ponerse en marcha rápidamente con Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:10:31.990Z'
TQID: 'https://experienceleague.adobe.com/dYjjsyvPAPOS5icw4Yi6Kpo93Nh2qvnCiW5-ih2hmDk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 1c15d2395e62ce41a298d25b973920963eef3a7a
workflow-type: tm+mt
source-wordcount: 820
ht-degree: 11%

---

# Inicio rápido: Conjuntos de giros{#quick-start-spin-sets}

Un conjunto de giros proporciona una vista de 360 grados de un objeto. Los conjuntos de giros permiten ver elementos desde cualquier ángulo, obteniendo detalles visuales desde cualquier perspectiva. Un conjunto de giros simula una visualización de 360 grados. Adobe Dynamic Media Classic ofrece conjuntos de giros unidimensionales en los que los visualizadores pueden rotar un elemento y conjuntos de giros bidimensionales en los que los visualizadores pueden rotar y voltear el elemento. Además, los usuarios pueden hacer zoom y recorrer cualquiera de las vistas. Los usuarios pueden examinar un elemento más de cerca desde un punto de vista particular.

![Imágenes de un conjunto de giros](/help/using/assets/spin_set.png)

Los conjuntos de giros también aceptan mapas de imagen. Un mapa de imagen es una región de una imagen dentro del conjunto de giros que muestra un panel de rollover con texto. Cuando el usuario selecciona un mapa de imagen, se activa una acción. Por ejemplo, se abre una página web para que el usuario pueda obtener más información sobre un producto. Para indicar un mapa de imagen en un conjunto de giros, aparece un contorno alrededor del propio mapa de imagen cuando el usuario mueve el puntero sobre él.

Consulte [Crear mapas de imagen](creating-image-maps.md).

Ver el vídeo de aprendizaje [Conjuntos de giros e imágenes: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS).

Al crear un conjunto de giros, Adobe recomienda las siguientes directrices y aplica los límites siguientes:

| Tipo de límite de conjunto de giros | Práctica recomendada | Límite impuesto |
| --- | --- | --- |
| Número máximo de filas/columnas por conjunto 2D | 12 a 18 imágenes por conjunto | 1000 |

Consulte también [Limitaciones de Dynamic Media](/help/using/limitations.md).

Esta guía se ha diseñado para ayudarle a empezar a utilizar rápidamente las técnicas de conjuntos de giros en Adobe Dynamic Media Classic. Siga los pasos del 1 al 7. Al final de cada paso, puede seleccionar un vínculo de tema para obtener más información.

## &#x200B;1. Creación y carga de imágenes

Como mínimo, necesita 8-12 tomas de un artículo para un conjunto de giros unidimensional y 16-24 para un conjunto de giros bidimensional. Las tomas deben realizarse a intervalos regulares para mostrar el elemento girando y volteando. Por ejemplo, si un conjunto de giros unidimensional incluye 12 disparos, gire el elemento 30° (360/12) para cada disparo.

En la barra de navegación global, selecciona **[!UICONTROL Cargar]** para cargar imágenes de giros desde tu equipo o red a Adobe Dynamic Media Classic.

Consulte [Instrucciones para obtener imágenes para conjuntos de giros](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## &#x200B;2. Creación de un conjunto de giros

Para crear un conjunto de giros, en la barra de navegación global, ve a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de giros]**. En el cuadro de diálogo Tamaño del conjunto de giros, elija cuántas filas y celdas desea y seleccione **[!UICONTROL Aceptar]**. A continuación, arrastre las imágenes a la cuadrícula de la página Conjunto de giros.

Consulte [Crear un conjunto de giros](creating-spin-set.md#creating-a-spin-set).

## &#x200B;3. Edición de un conjunto de giros

Para editar un conjunto de giros, en la barra de navegación global, ve a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visor]**. Seleccione un conjunto de giros y, a continuación, seleccione **[!UICONTROL Editar]**. Agregue y quite las imágenes y cambie su posición. Puede cambiar la posición de las filas en conjuntos de giros bidimensionales.

Consulte [Editar un conjunto de giros](creating-spin-set.md#editing-a-spin-set).

## &#x200B;4. Configurar ajustes preestablecidos del visor de conjuntos de giros

Los administradores pueden crear ajustes preestablecidos de visor de conjuntos de giros. Estos ajustes preestablecidos determinan el aspecto del visor de conjuntos de giros. Para configurar un nuevo ajuste preestablecido de visualizador de conjuntos de giros, en la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de visualizador]**.

En la página Ajustes preestablecidos de visor, haga clic en **[!UICONTROL Agregar]**, seleccione **[!UICONTROL Visor de conjuntos de giros]** en la lista desplegable y, a continuación, seleccione **[!UICONTROL Agregar]**. Elija opciones en la página `Configure Viewer` y luego haga clic en **[!UICONTROL Guardar]**.

Consulte [Configurar ajustes preestablecidos del visor de conjuntos de giros](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## &#x200B;5. Previsualización de un conjunto de giros

Seleccione el conjunto de giros en el panel Examinar y, a continuación, haga clic en **[!UICONTROL Vista previa]**. En la página Vista previa, mantenga presionado el botón y arrastre el puntero a izquierda o derecha para girar el elemento visualmente.

Ver [Vista previa de un conjunto de giros](previewing-spin-set.md#previewing-a-spin-set).

## &#x200B;6. Publicación de un conjunto de giros

Al publicar un conjunto de giros, se coloca en servidores de Adobe Dynamic Media Classic para que se pueda enviar de forma dinámica a su sitio web o aplicación. También activa la cadena URL que llama al conjunto de giros desde los servidores de imágenes de Dynamic Media al sitio web o la aplicación.

Para publicar un conjunto de giros, márquelo para su publicación seleccionando el icono **[!UICONTROL Marcar para publicación]** junto a su nombre en el panel Examinar. En la barra de navegación global, haga clic en **[!UICONTROL Publicar]** para iniciar la publicación. En la página Publicación, haga clic en **[!UICONTROL Enviar publicación]**.

Ver [Publicar un conjunto de giros](publishing-spin-set.md#publishing-a-spin-set).

## &#x200B;7. Vinculación de un conjunto de giros a una página web

Adobe Dynamic Media Classic crea cadenas de llamada de URL para conjuntos de giros y las activa después de publicarlas. Puede copiar estas direcciones URL desde la página de vista previa.

Seleccione el conjunto de giros y, a continuación, haga clic en **[!UICONTROL Vista previa]**. Seleccione un ajuste preestablecido de visor de conjuntos de giros. Luego haga clic en **[!UICONTROL Copiar URL]**.

Ver [Vincular un conjunto de giros a una página web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
