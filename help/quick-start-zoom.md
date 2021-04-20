---
title: '"Inicio rápido: Zoom"'
description: Introducción y acceso rápido al zoom para ayudarle a poner en marcha rápidamente.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 64%

---


# Inicio rápido: Zoom{#quick-start-zoom}

Zoom le permite ver de forma interactiva detalles de alta resolución en imágenes. Por ejemplo, se pueden ver colores, opciones, ángulos y detalles de una imagen en un visor integrado, dinámico y completamente configurable. Este visor puede ser parte de una página web o aparecer en una ventana emergente. Puede analizar las imágenes de cerca y desplazarlas con resoluciones altas. La aplicación de zoom ofrece a los clientes una visualización interactiva, informativa y atractiva.

Dynamic Media Classic también ofrece zoom guiado, un medio para resaltar las funciones importantes de una imagen. Por ejemplo, para centrar la atención en un logotipo, puede crear un destino de zoom para el mismo. Cuando un usuario haga clic en este destino de zoom, se aplicará zoom al logotipo.

Todas las imágenes de zoom se crean y ofrecen a partir de imágenes principales, gráficos y atributos controlados por base de datos. El zoom de Dynamic Media Classic reduce en gran medida el tiempo y el coste de producción y entrega de imágenes. Puede usar Visualizadores de zoom para acercar y alejar imágenes. El visor de zoom tiene botones en los que se puede hacer clic para aplicar zoom y desplazamiento; también se pueden realizar desplazamientos arrastrando a la pantalla. Mediante ajustes preestablecidos de visor de zoom se puede configurar el visor de zoom dentro del cual se aplicará zoom en las imágenes.

**Inicio rápido**

Este inicio rápido de zoom está diseñado para ponerse en marcha rápidamente con las técnicas de zoom en Dynamic Media Classic. Siga los pasos del 1 al 6. Después de cada paso hay una referencia cruzada a un encabezado de tema en el que podrá encontrar más información.

**1. Carga de imágenes de zoom**

Comience por cargar las imágenes de zoom en Dynamic Media Classic. Para lograr un zoom óptimo, Dynamic Media Classic recomienda que las imágenes tengan al menos 2000 píxeles en la dimensión más larga.

Seleccione el botón Cargar en la barra de navegación global para cargar imágenes de su equipo o red a una carpeta de Dynamic Media Classic. Consulte [Carga de imágenes de zoom](uploading-zoom-images.md#uploading_zoom_images).

**2. Creación de destinos de zoom para zoom guiado**

Los destinos de zoom permiten resaltar partes específicas de una imagen. Por ejemplo, puede hacer destacar las partes de una imagen que la hacen exclusiva. En la ventana del visor de zoom, los destinos de zoom aparecen como miniaturas al lado de la imagen. Si se selecciona una de estas miniaturas de destino de zoom, se aplica zoom automáticamente en una parte de la imagen que se especifique.

Para crear un objetivo de zoom, haga clic en el botón de rollover Editar y seleccione Destinos de zoom o abra una imagen en el panel Examinar de la vista de detalles y haga clic en Destinos de zoom. A continuación, use las herramientas de zoom en la pantalla del editor de destinos de zoom para aislar parte de la imagen como destino. Consulte [Creación de destinos de zoom para zoom guiado](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

**3. Configuración de ajustes preestablecidos de visor de zoom**

Los ajustes preestablecidos de visor de zoom determinan el estilo y comportamiento de los visores de zoom. Puede configurar ajustes preestablecidos de visor de zoom si es un administrador; Dynamic Media Classic también incluye ajustes preestablecidos de visor de zoom &quot;prácticas recomendadas&quot; predeterminados.

Para crear un ajuste preestablecido del visor de zoom, haga clic en el botón Ajustes en la barra de navegación global y seleccione Ajustes preestablecidos de visor. A continuación, haga clic en el botón Agregar en la pantalla Ajustes preestablecidos de visor, seleccione una plataforma, elija Visor de zoom y haga clic en Agregar. A continuación elija las opciones deseadas en la pantalla Configurar visor. 

Dynamic Media Classic ofrece opciones de ajustes preestablecidos de visor de zoom que permiten seleccionar el estilo del botón y el aspecto general del visor. También puede personalizar la configuración de zoom para el sitio web. Consulte [Configuración de ajustes preestablecidos de visor de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

**4. Vista previa de imágenes con el visor de zoom**

Puede obtener una vista previa de imágenes en un visor de zoom para ver lo que sucede al aplicar zoom en las imágenes.

Para explorar varios ajustes preestablecidos de visor de zoom y cómo presentan el efecto de zoom, elija una imagen en el panel Examinar y haga clic en el botón Vista previa. Se abre la pantalla Vista previa. Elija Ajustes preestablecidos > Zoom y seleccione un ajuste preestablecido en el menú Zoom.

Aparecerán los botones Zoom. Puede ver el aspecto de las imágenes de zoom en el sitio web. Seleccione los botones (y destinos) de zoom para probar la configuración del ajuste preestablecido de visor de zoom que elija. Consulte [Vista previa de imágenes con distintos visores zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

**5. Publicación de imágenes de zoom**

Al publicar las imágenes de zoom, estas se colocan en los servidores de imágenes de Dynamic Media para que se puedan enviar al sitio web y a la aplicación. Como parte del proceso de publicación, Dynamic Media Classic activa las cadenas URL. Estas cadenas URL llaman a hacer zoom de imágenes desde servidores de imágenes de Dynamic Media a su sitio web o aplicación.

Seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. En la pantalla Publicar, seleccione el botón Iniciar publicación. Consulte [Publicación de imágenes de zoom](publishing-zoom-images.md#publishing_zoom_images).

**6. Vinculación de visores de zoom al sitio web**

Dynamic Media Classic crea las cadenas de llamada de URL necesarias para acercar imágenes y las activa al publicar imágenes en servidores de imágenes de Dynamic Media. Puede copiar estas cadenas URL de la pantalla Vista previa. Cuando haya copiado las cadenas URL, estarán disponibles para su página web y sus aplicaciones. Consulte [Vinculación de visores de zoom al sitio web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
