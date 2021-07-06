---
title: '"Inicio rápido: Conjunto de medios mixtos"'
description: Introducción y inicio rápido a los conjuntos de medios mixtos para ayudarle a empezar a utilizarlos rápidamente.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Visualizadores,Conjunto de medios mixtos
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: f99832bc9660a16b06e63b19f9ead1267dab0f35
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 52%

---

# Inicio rápido: Conjuntos de medios mixtos{#quick-start-mixed-media-sets}

Los conjuntos de medios mixtos de ofrecen a los usuarios una visualización integrada. Los conjuntos de medios mixtos pueden incluir imágenes, conjuntos de imágenes, conjuntos de muestras, conjuntos de giros y vídeos. Los usuarios pueden hacer clic en diferentes fichas del visor de medios mixtos para ver los elementos en los distintos visores. Si no se especifica ninguna ficha, todos los recursos se muestran juntos en la fila de muestras.

Los ajustes preestablecidos del visor de conjuntos de medios mixtos incluyen opciones de comunidad para los usuarios finales para incrustar código, copiar URL y crear un vínculo al sitio web principal. Los usuarios pueden utilizar estas opciones para compartir información sobre los productos en sus sitios web personales o en los sitios de redes sociales.

Este inicio rápido de conjuntos de medios mixtos está diseñado para ponerse en marcha rápidamente con las técnicas de conjuntos de medios mixtos en Dynamic Media Classic.

## 1. Carga de imágenes, archivos de muestra y vídeos

Comience por cargar las imágenes, los archivos de muestras, y los vídeos para sus conjuntos de medios mixtos. Dado que los usuarios pueden hacer zoom en las imágenes en el visualizador de conjuntos de medios mixtos, asegúrese de tener en cuenta esta capacidad al elegir imágenes. Asegúrese de que las imágenes tengan al menos 2000 píxeles en el tamaño más grande.

En la barra de navegación global, haga clic en **[!UICONTROL Cargar]** para cargar archivos del equipo a una carpeta de Dynamic Media Classic.

Consulte [Carga de los archivos](uploading-files.md#uploading-your-files).

## 2. Creación de conjuntos de medios para su uso en el conjunto de medios mixtos

Puede agregar imágenes, conjuntos de imágenes, conjuntos de muestras, conjuntos de giros y vídeos a su conjunto de medios mixtos. Prepare los conjuntos de medios antes de agregarlos al conjunto de medios mixtos.

Consulte [Creación de un conjunto de imágenes](creating-image-set.md#creating-an-image-set), [Creación de un conjunto de muestras](creating-swatch-set.md#creating-a-swatch-set) y [Creación de un conjunto de giros](creating-spin-set.md#creating-a-spin-set).

## 3. Creación de un conjunto de medios mixtos

En la barra de navegación global, haga clic en **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de medios mixtos]**. Arrastre las imágenes, los conjuntos de muestras, los conjuntos de imágenes y los vídeos a la página Conjunto de medios mixtos . Para añadir una pista de sonido, arrastre un archivo de audio al cuadro Pista de sonido.

Consulte [Creación de un conjunto de medios mixtos](creating-mixed-media-set.md#creating-a-mixed-media-set)

## 4. Configuración de los ajustes preestablecidos del visualizador de medios mixtos

Dynamic Media Classic incluye ajustes preestablecidos de visor predeterminados para conjuntos de medios mixtos. Los administradores pueden crear o modificar los ajustes preestablecidos de visor de conjuntos de medios mixtos.

Al configurar un ajuste preestablecido de visualizador de conjuntos de medios mixtos, agregue los ajustes preestablecidos de visualizador para todos los demás recursos del conjunto. Por ejemplo, si su conjunto de medios mixtos incluye vídeos, será necesario agregar un ajuste preestablecido de visor de vídeo al ajuste preestablecido de visor de conjuntos de medios mixtos. También puede agregar una pista de audio al visor. Esta pista de audio se reproduce mientras el visor está abierto, pero no cuando un vídeo está activo.

Consulte [Configuración de un ajuste preestablecido de visor de conjuntos de medios mixtos](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) y [Creación y edición de valores preestablecidos de visor](application-setup.md#adding-and-editing-viewer-presets).

## 5. Vista previa de un conjunto de medios mixtos

Haga clic en el botón **[!UICONTROL Preview]** del conjunto de medios mixtos. Si desea examinar el conjunto de medios mixtos en el visor de conjuntos de medios mixtos, puede hacer clic en los iconos de miniaturas y muestras. Puede elegir distintos visores en el menú Ajustes preestablecidos.

Consulte [Previsualización de un recurso](previewing-asset.md#previewing-an-asset).

## 6. Publicación de un conjunto de medios mixtos

Al publicar un conjunto de medios mixtos, este se coloca en los servidores de Dynamic Media Classic y se activa la cadena URL.

Los conjuntos de vídeo adaptables requieren que se publique en el **Servidor de vídeo** y también en el **Servidor de imágenes**. El **Servidor de vídeo** se utiliza para publicar los vídeos reales que se han marcado para publicación. Además, utiliza **Image Server** para publicar recursos relacionados, como miniaturas de vídeo, y establecer información para cualquier conjunto de vídeos adaptables.

Consulte [Publicación de un conjunto de medios mixtos](publishing-mixed-media-set.md#publishing-a-mixed-media-set)

## 7. Vinculación de un conjunto de medios mixtos a una página web

Dynamic Media Classic activa las llamadas URL para conjuntos de medios mixtos después de publicarlos. Puede copiar estas direcciones URL desde la página Vista previa .

Seleccione el conjunto de medios mixtos y, a continuación, haga clic en **[!UICONTROL Vista previa]**. En la página Vista previa, seleccione un ajuste preestablecido de visualizador de conjuntos de medios mixtos y haga clic en **[!UICONTROL Copiar URL]**. Consulte [Vinculación de conjuntos de medios mixtos a páginas web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
