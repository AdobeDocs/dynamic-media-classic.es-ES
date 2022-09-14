---
title: "Inicio rápido: Conjunto de medios mixtos"
description: Introducción y inicio rápido a los conjuntos de medios mixtos para ayudarle a poner en marcha Adobe Dynamic Media Classic rápidamente.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 34%

---

# Inicio rápido: Conjuntos de medios mixtos{#quick-start-mixed-media-sets}

Los conjuntos de medios mixtos de ofrecen a los usuarios una visualización integrada. Los conjuntos de medios mixtos pueden incluir imágenes, conjuntos de imágenes, conjuntos de muestras, conjuntos de giros y vídeos. Los usuarios pueden seleccionar distintas pestañas dentro del visualizador de medios mixtos para ver los elementos en los distintos visualizadores. Si no se especifica ninguna ficha, todos los recursos se muestran juntos en la fila de muestras.

Los ajustes preestablecidos del visor de conjuntos de medios mixtos incluyen opciones de comunidad para los usuarios finales para incrustar código, copiar URL y crear un vínculo al sitio web principal. Los usuarios pueden utilizar estas opciones para compartir información sobre los productos en sus sitios web personales o en los sitios de redes sociales.

Este inicio rápido de conjuntos de medios mixtos está diseñado para ayudarle a poner en marcha rápidamente las técnicas de conjuntos de medios mixtos en Adobe Dynamic Media Classic.

## 1. Cargue las imágenes, los archivos de muestra y los vídeos

Comience por cargar las imágenes, los archivos de muestras, y los vídeos para sus conjuntos de medios mixtos. Dado que los usuarios pueden hacer zoom en las imágenes en el visualizador de conjuntos de medios mixtos, asegúrese de tener en cuenta esta capacidad al elegir imágenes. Asegúrese de que las imágenes tengan al menos 2000 píxeles en el tamaño más grande.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar archivos desde el equipo a una carpeta de Adobe Dynamic Media Classic.

Consulte [Cargar los archivos](uploading-files.md#uploading-your-files).

## 2. Crear conjuntos de medios para utilizarlos en el conjunto de medios mixtos

Puede agregar imágenes, conjuntos de imágenes, conjuntos de muestras, conjuntos de giros y vídeos a su conjunto de medios mixtos. Prepare los conjuntos de medios antes de agregarlos al conjunto de medios mixtos.

Consulte [Crear un conjunto de imágenes](creating-image-set.md#creating-an-image-set), [Creación de un conjunto de muestras](creating-swatch-set.md#creating-a-swatch-set)y [Crear un conjunto de giros](creating-spin-set.md#creating-a-spin-set).

## 3. Crear un conjunto de medios mixtos

En la barra de navegación global, vaya a **[!UICONTROL Generar]** > **[!UICONTROL Conjuntos de medios mixtos]**. Arrastre las imágenes, los conjuntos de muestras, los conjuntos de imágenes y los vídeos a la página Conjunto de medios mixtos . Para añadir una pista de sonido, arrastre un archivo de audio al cuadro Pista de sonido.

Consulte [Crear un conjunto de medios mixtos](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Configurar ajustes preestablecidos del visualizador de medios mixtos

Adobe Dynamic Media Classic incluye ajustes preestablecidos de visor predeterminados para conjuntos de medios mixtos. Los administradores pueden crear o modificar los ajustes preestablecidos de visor de conjuntos de medios mixtos.

Al configurar un ajuste preestablecido de visualizador de conjuntos de medios mixtos, agregue los ajustes preestablecidos de visualizador para todos los demás recursos del conjunto. Por ejemplo, si su conjunto de medios mixtos incluye vídeos, será necesario agregar un ajuste preestablecido de visor de vídeo al ajuste preestablecido de visor de conjuntos de medios mixtos. También puede agregar una pista de audio al visor. Esta pista de audio se reproduce mientras el visor está abierto, pero no cuando un vídeo está activo.

Consulte [Configuración de un ajuste preestablecido de visualizador de conjuntos de medios mixtos](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) y [Crear y editar ajustes preestablecidos de visor](application-setup.md#adding-and-editing-viewer-presets).

Consulte también [Ajustes preestablecidos de visor](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vídeo de formación.

## 5. Obtener una vista previa de un conjunto de medios mixtos

Seleccione el conjunto de medios mixtos **[!UICONTROL Vista previa]** botón. Puede seleccionar los iconos de miniatura y muestra para examinar el conjunto de medios mixtos en el visor de conjuntos de medios mixtos. Puede elegir distintos visores en el menú Ajustes preestablecidos.

Consulte [Vista previa de un recurso](previewing-asset.md#previewing-an-asset).

## 6. Publicar un conjunto de medios mixtos

Al publicar un conjunto de medios mixtos, se coloca en servidores de Adobe Dynamic Media Classic y se activa la cadena URL.

Los conjuntos de vídeo adaptables requieren que se publique en el **Servidor de vídeo** y también en el **Servidor de imágenes**. El **Servidor de vídeo** se utiliza para publicar los vídeos reales que se han marcado para publicación. Y usted usa **Servidor de imágenes** para publicar recursos relacionados, como miniaturas de vídeo, y establecer información para cualquier conjunto de vídeos adaptables.

Consulte [Publicar un conjunto de medios mixtos](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Vincular un conjunto de medios mixtos a una página web

Adobe Dynamic Media Classic activa las llamadas URL para conjuntos de medios mixtos después de publicarlos. Puede copiar estas direcciones URL desde la página Vista previa .

Seleccione el conjunto de medios mixtos y, a continuación, seleccione **[!UICONTROL Vista previa]**. En la página Vista previa, seleccione un ajuste preestablecido de visualizador de conjuntos de medios mixtos y, a continuación, seleccione **[!UICONTROL Copiar URL]**. Consulte [Vinculación de conjuntos de medios mixtos a páginas web](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
