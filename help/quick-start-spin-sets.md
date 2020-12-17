---
title: '"Inicio rápido: Conjuntos de giros"'
seo-title: '"Inicio rápido: Conjuntos de giros"'
description: nulo
seo-description: Introducción y Inicio rápido del conjunto de giros para ayudarle en el uso inicial.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 68%

---


# Inicio rápido: Conjuntos de giros{#quick-start-spin-sets}

Un conjunto de giros simula la acción física de girar un objeto para examinarlo. Los conjuntos de giros permiten ver elementos desde cualquier ángulo, por lo que se pueden obtener los detalles visuales clave de los mismos desde cualquier ángulo. Un conjunto de giros simula una visualización de 360 grados. Dynamic Media Classic oferta conjuntos de giros unidimensionales en los que los visores pueden rotar un elemento y conjuntos de giros bidimensionales en los que los visores pueden rotar y voltear el elemento. Además, los usuarios pueden aplicar zoom &quot;de forma libre&quot; y desplazarse por cualquiera de las vistas con unos pocos clics simples del ratón. De esta forma, los usuarios pueden examinar un elemento de cerca desde un punto de vista determinado.

![Imágenes para un conjunto de giros.](/help/assets/spin_set.png)

Los conjuntos de giros también aceptan mapas de imagen. Un mapa de imagen es una región de una imagen dentro de un conjunto de giros que muestra un panel de rollover con texto. Cuando el usuario hace clic en un mapa de imagen, se activa una acción de cierto tipo. Por ejemplo, se abre una página web para que el usuario pueda obtener más información sobre un producto. Para llamar la atención sobre el uso de un mapa de imagen en un conjunto de giros, cuando el usuario mueve el puntero del ratón por encima del mapa de imagen se visualiza un contorno alrededor del mismo.

Consulte [Creación de mapas de imagen](creating-image-maps.md).

**Inicio rápido**

Este Inicio rápido sobre los conjuntos de giros se ha diseñado para ayudarle en el uso inicial de las técnicas de conjuntos de giros en Dynamic Media Classic. Siga los pasos del 1 al 7. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información si la necesita.

**1. Creación y carga de las imágenes**

Como mínimo, necesitará entre 8 y 12 tomas de un elemento para un conjunto de giros unidimensional y entre 16 y 24 para un conjunto de giros bidimensional. Las tomas deben realizarse siguiendo intervalos regulares para dar la impresión de que se está rotando y volteando el elemento. Por ejemplo, si el conjunto de giros unidimensional incluye 12 tomas, gire el elemento 30 grados (360 entre 12) cada vez que realice una toma.

Seleccione el botón Cargar en la barra de navegación global para cargar imágenes de giro desde el equipo o la red en Dynamic Media Classic.

Consulte [Instrucciones para obtener imágenes para conjuntos de giros](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

**2. Creación de un conjunto de giros**

Para crear un conjunto de giros, haga clic en el botón Generar y elija Conjuntos de giros. En el cuadro de diálogo Tamaño del conjunto de giros, seleccione el número de columnas y celdas que desee incluir y haga clic en Aceptar. A continuación, arrastre las imágenes hasta la cuadrícula de la pantalla Conjunto de giros.

Consulte [Creación de un conjunto de giros](creating-spin-set.md#creating-a-spin-set).

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06-245331fc135ab744793-8000">Including Image Maps in Spin Sets</a> to add clickable, hotspot regions, known as Image Maps, to images in a Spin Set. </p>

 -->

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See also <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06229f600f135ab7cc461-8000">Managing InfoPanel content</a>.</p>

 -->

**3. Edición de un conjunto de giros**

Para editar un conjunto de giros, seleccione el botón de rollover de edición correspondiente. Aparecerá la pantalla Conjunto de giros. Agregue y quite las imágenes y cambie su posición. Puede cambiar la posición de las filas en los conjuntos de giros bidimensionales.

Consulte [Edición de un conjunto de giros](creating-spin-set.md#editing-a-spin-set).

**4. Configuración de ajustes preestablecidos del visor de conjunto de giros**

Los administradores pueden crear ajustes preestablecidos de visor de conjuntos de giros. Estos ajustes preestablecidos determinan el aspecto del visor de conjuntos de giros. Para crear un nuevo ajuste preestablecido de visor de conjuntos de giros, seleccione el botón Ajustes en la barra de navegación global. En la pantalla Ajustes, seleccione Ajustes de aplicación y luego Ajustes preestablecidos de visor.

En la pantalla Ajustes preestablecidos de visor, seleccione el menú Agregar y elija la opción Visor de conjuntos de giros en el cuadro de diálogo que aparece. A continuación elija las opciones deseadas en la pantalla Configurar visor. 

Consulte [Configuración de ajustes preestablecidos del visor de conjunto de giros](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

**5. Vista previa de un conjunto de giros**

Seleccione su conjunto de giros en el panel Examinar y haga clic en el botón de rollover Vista previa. En la pantalla Vista previa, mantenga presionado el botón del ratón y arrastre el puntero hacia la izquierda o la derecha para “girar” el elemento visualmente.

Consulte [Vista previa de un conjunto de giros](previewing-spin-set.md#previewing-a-spin-set).

**6. Publicación de un conjunto de giros**

Al publicar un conjunto de giros, éste se coloca en los servidores de Dynamic Media Classic para que se pueda distribuir dinámicamente en el sitio web o la aplicación. También activa la cadena URL que llama al conjunto de giros desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Para publicar un conjunto de giros, márquelo para la publicación seleccionando el icono **Marcar para publicación** junto a su nombre en el panel Examinar. Haga clic en **Publicar** en la barra de navegación global para iniciar una publicación. En la pantalla Publicar, haga clic en **Publicación de Inicio**.

Consulte [Publicación de un conjunto de giros](publishing-spin-set.md#publishing-a-spin-set).

**7. Vinculación de un conjunto de giros a una página web**

Dynamic Media Classic crea cadenas de llamada mediante URL para conjuntos de giros y las activa después de publicarlos. Puede copiar estas direcciones URL desde la pantalla Vista previa.

Seleccione el conjunto de giros y, a continuación, haga clic en **Previsualización**. Se abre la pantalla Vista previa. Seleccione un ajuste preestablecido de visor de conjuntos de giros. A continuación, haga clic en **Copiar URL**.

Consulte [Vinculación de un conjunto de giros a una página web](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
