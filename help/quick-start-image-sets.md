---
title: '"Inicio rápido: Conjuntos de imágenes"'
description: Introducción y inicio rápido a los conjuntos de imágenes para ayudarle a poner en marcha rápidamente las técnicas de conjuntos de imágenes en Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: 5040b1916794d3b54f952a1df5f060be2f31006a
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 21%

---

# Inicio rápido: Conjuntos de imágenes{#quick-start-image-sets}

Los conjuntos de imágenes de Adobe Dynamic Media Classic proporcionan a los usuarios una experiencia de visualización integrada. En el visor de conjuntos de imágenes dinámico los usuarios pueden acceder a diversas vistas de un elemento haciendo clic en una imagen de miniatura. Conjuntos de imágenes permite presentar vistas de alta resolución alternativas de un elemento.

El visor de conjuntos de imágenes ofrece herramientas de zoom para examinar las imágenes de cerca. Si lo desea, puede crear destinos de zoom guiado y mapas de imagen para que formen parte del conjunto de imágenes. Los conjuntos de imágenes permiten una visualización completa y coordinada.

Consulte [Conjuntos de giros e imágenes: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de formación.

>[!NOTE]
>
>Al crear un conjunto de imágenes, Adobe recomienda las siguientes directrices de prácticas recomendadas y límites obligatorios.
>
>* Número de recursos duplicados por conjunto de imágenes
   >   * Práctica recomendada: 20
   >   * Límite obligatorio: 20
>* Número máximo de páginas por conjunto de imágenes
   >   * Práctica recomendada: 1000
   >   * Límite ampliado: 1000


El siguiente Inicio rápido de conjuntos de imágenes está diseñado para ayudarle a poner en marcha rápidamente las técnicas de conjuntos de imágenes en Adobe Dynamic Media Classic.

## 1. Cargue las imágenes principales para varias vistas y muestras

Comience el proceso cargando las imágenes para los conjuntos de imágenes. Dado que los usuarios pueden hacer zoom en las imágenes en el visualizador de conjuntos de imágenes, asegúrese de tener en cuenta esta capacidad al elegir imágenes. Asegúrese de que las imágenes tengan al menos 2000 píxeles en el tamaño más grande. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan las imágenes TIFF, PNG y EPS sin pérdida.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar archivos desde el equipo a una carpeta de Adobe Dynamic Media Classic.

Consulte [Preparación de recursos de conjuntos de imágenes para su carga](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) y [Cargar los archivos](uploading-files.md#uploading-your-files).

## 2. Crear un conjunto de imágenes

En los conjuntos de imágenes, los usuarios seleccionan las imágenes en miniatura en el visor de conjuntos de imágenes para ver una imagen desde un lado o ángulo diferente.

Para crear un conjunto de imágenes, en la barra de navegación global, seleccione **[!UICONTROL Generar]** y, a continuación, elija **[!UICONTROL Conjuntos de imágenes]**. En la ventana Conjunto de imágenes, arrastre las imágenes a la página para componer el conjunto de imágenes. Organice, agregue y elimine imágenes según sea necesario.

Consulte [Crear un conjunto de imágenes](creating-image-set.md#creating-an-image-set).

Consulte también [Incluir destinos de zoom y mapas de imagen en conjuntos de imágenes](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Prepare ajustes preestablecidos del visualizador de conjuntos de imágenes, según sea necesario

Los administradores pueden crear o modificar los ajustes preestablecidos de visor de conjuntos de imágenes. Adobe Dynamic Media Classic incluye ajustes preestablecidos de visor predeterminados para cada tipo de medios enriquecidos. Utilice el visor de zoom: **[!UICONTROL Personalizado]** > **[!UICONTROL Imágenes]** o **[!UICONTROL Conjuntos de imágenes]**/**[!UICONTROL Varias vistas]** ajustes preestablecidos para ver los conjuntos de imágenes.

Puede añadir o editar los ajustes preestablecidos del visor desde la pantalla Ajustes de aplicación.

Consulte [Crear y editar ajustes preestablecidos de visor](application-setup.md#adding-and-editing-viewer-presets).

## 4. Obtener una vista previa de un conjunto de imágenes

Seleccione el conjunto de imágenes en el panel Examinar y, a continuación, seleccione **[!UICONTROL Vista previa]**. En la página Vista previa, seleccione los iconos de miniaturas para examinar el conjunto de imágenes en el visor seleccionado. Puede elegir distintos visores en el menú Ajustes preestablecidos.

Consulte [Vista previa de un recurso](previewing-asset.md#previewing-an-asset).

## 5. Publicar un conjunto de imágenes

Al publicar un conjunto de imágenes, este se coloca en los servidores de Adobe Dynamic Media Classic y se activa la cadena URL.

>[!NOTE]
>
>Este paso no es necesario si seleccionó la opción **[!UICONTROL Publicar después de guardar]** (predeterminada) al crear y guardar el conjunto de imágenes.

Select **[!UICONTROL Marcar para publicación]** a la izquierda de su nombre en el panel Examinar. A continuación, seleccione **[!UICONTROL Publicación]**. En la página Publicar , seleccione **[!UICONTROL Enviar publicación]**.

Consulte [Publicar archivos](publishing-files.md#publishing-files).

## 6. Vincular un conjunto de imágenes a su sitio web

Adobe Dynamic Media Classic crea llamadas de URL para conjuntos de imágenes y los activa después de publicar. Puede copiar estas direcciones URL desde la pantalla Vista previa.

Seleccione el conjunto de imágenes y, a continuación, seleccione **[!UICONTROL Vista previa]**. A continuación, seleccione un ajuste preestablecido de visualizador de conjuntos de imágenes y, a continuación, seleccione **[!UICONTROL Copiar URL]**.

Consulte [Vinculación de un conjunto de imágenes a una página web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
