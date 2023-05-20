---
title: "Inicio rápido: Conjuntos de imágenes"
description: Introducción y Inicio rápido a los conjuntos de imágenes para ayudarle a ponerse en marcha rápidamente con las técnicas de conjuntos de imágenes en Adobe Dynamic Media Classic.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# Inicio rápido: Conjuntos de imágenes{#quick-start-image-sets}

Los conjuntos de imágenes de Adobe Dynamic Media Classic proporcionan a los usuarios una experiencia de visualización integrada. En el visor de conjuntos de imágenes dinámico los usuarios pueden acceder a diversas vistas de un elemento haciendo clic en una imagen de miniatura. Los conjuntos de imágenes permiten presentar vistas alternativas de alta resolución de un elemento.

El visor de conjuntos de imágenes ofrece herramientas de zoom para examinar las imágenes de cerca. Si lo desea, puede crear destinos de zoom guiado y mapas de imagen para que formen parte del conjunto de imágenes. Los conjuntos de imágenes permiten una visualización completa y coordinada.

Consulte [Conjuntos de imágenes y giros: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de formación.

Al crear un conjunto de imágenes, Adobe recomienda las siguientes prácticas recomendadas y aplica los límites siguientes:

| Tipo de límite | Práctica recomendada | Límite impuesto |
| --- | --- | --- |
| Número de recursos duplicados por conjunto | No hay duplicados | 20 |
| Número máximo de imágenes por conjunto | 5-10 imágenes por conjunto | 1.000 |

Consulte también [Limitaciones de Dynamic Media](/help/limitations.md).

El siguiente Inicio rápido de conjuntos de imágenes está diseñado para ayudarle a ponerse en marcha rápidamente con las técnicas de conjuntos de imágenes en Adobe Dynamic Media Classic.

## 1. Cargue las imágenes principales para varias vistas y muestras

Comience el proceso cargando las imágenes para los conjuntos de imágenes. Dado que los usuarios pueden aplicar zoom a las imágenes en el Visor de conjuntos de imágenes, asegúrese de tener en cuenta esta capacidad al elegir imágenes. Asegúrese de que las imágenes tengan al menos 2000 píxeles del tamaño más grande. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan imágenes de TIFF, PNG y EPS sin pérdidas.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar archivos desde el equipo a una carpeta de Adobe Dynamic Media Classic.

Consulte [Preparar recursos del conjunto de imágenes para cargar](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) y [Cargar los archivos](uploading-files.md#uploading-your-files).

## 2. Crear un conjunto de imágenes

En los conjuntos de imágenes, los usuarios seleccionan imágenes en miniatura en el Visor de conjuntos de imágenes para ver una imagen desde un lado o ángulo diferente.

Para crear un conjunto de imágenes, en la barra de navegación global, seleccione **[!UICONTROL Generar]**, luego elija **[!UICONTROL Conjuntos de imágenes]**. En la ventana Conjunto de imágenes, arrastre las imágenes a la página para componer el conjunto de imágenes. Organice, agregue y elimine imágenes según sea necesario.

Consulte [Crear un conjunto de imágenes](creating-image-set.md#creating-an-image-set).

Consulte también [Incluir destinos de zoom y mapas de imagen en conjuntos de imágenes](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Prepare los ajustes preestablecidos del visualizador de conjuntos de imágenes según sea necesario

Los administradores pueden crear o modificar los ajustes preestablecidos de visor de conjuntos de imágenes. Adobe Dynamic Media Classic incluye ajustes preestablecidos de visor predeterminados para cada tipo de medio enriquecido. Uso del Visor de zoom: **[!UICONTROL Personalizado]** > **[!UICONTROL Imágenes]** o **[!UICONTROL Conjuntos de imágenes]**/**[!UICONTROL Vistas múltiples]** para ver los conjuntos de imágenes.

Puede añadir o editar los ajustes preestablecidos del visor desde la pantalla Ajustes de aplicación.

Consulte [Crear y editar ajustes preestablecidos de visor](application-setup.md#adding-and-editing-viewer-presets).

## 4. Previsualizar un conjunto de imágenes

Seleccione el conjunto de imágenes en el panel Examinar y, a continuación, seleccione **[!UICONTROL Previsualizar]**. En la página Vista previa, seleccione los iconos de miniatura para examinar el conjunto de imágenes en el visor seleccionado. Puede elegir distintos visores en el menú Ajustes preestablecidos.

Consulte [Previsualización de un recurso](previewing-asset.md#previewing-an-asset).

## 5. Publicar un conjunto de imágenes

Al publicar un conjunto de imágenes, se coloca en los servidores de Adobe Dynamic Media Classic y se activa la cadena URL.

>[!NOTE]
>
>Este paso no es necesario si seleccionó la opción **[!UICONTROL Publicar después de guardar]** (predeterminada) al crear y guardar el conjunto de imágenes.

Seleccionar **[!UICONTROL Marcar para publicación]** a la izquierda de su nombre en el panel Examinar. A continuación, seleccione **[!UICONTROL Publish]**. En la página Publicar, seleccione **[!UICONTROL Enviar publicación]**.

Consulte [Publicar archivos](publishing-files.md#publishing-files).

## 6. Vincular un conjunto de imágenes a su sitio web

Adobe Dynamic Media Classic crea llamadas de URL para conjuntos de imágenes y las activa después de la publicación. Puede copiar estas direcciones URL desde la pantalla Vista previa.

Seleccione el conjunto de imágenes y, a continuación, seleccione **[!UICONTROL Previsualizar]**. A continuación, seleccione un ajuste preestablecido del visualizador de conjuntos de imágenes y seleccione **[!UICONTROL Copiar URL]**.

Consulte [Vinculación de un conjunto de imágenes a una página web](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
