---
title: 'Inicio rápido: Cambio de tamaño de imagen'
description: Introducción y Inicio rápido del tamaño de la imagen para ayudarle a ponerse en marcha rápidamente con las técnicas de tamaño de imagen en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
autotag-review: '2026-05-13T20:09:57.533Z'
TQID: 'https://experienceleague.adobe.com/VGp4OQ03iRiobXKWuUERNtFwUMQ4z7a19wyOgHWuv3w'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 202f477d78272c66d0ac490e3a5041839b3e4f4d
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 6%

---

# Inicio rápido: Cambio de tamaño de imagen{#quick-start-image-sizing}

El tamaño de imagen hace referencia a la capacidad de Adobe Dynamic Media Classic para crear varias imágenes derivadas basadas en una sola imagen de alta resolución. En lugar de crear manualmente varias imágenes para el sitio web o la aplicación, se proporciona una sola imagen principal. Adobe Dynamic Media Classic genera todas las imágenes modificadas a medida que se solicitan. La entrega dinámica de imágenes a partir de una sola imagen principal tiene muchas ventajas:

* No es necesario crear manualmente varias copias de la imagen en diferentes tamaños. Suministra una imagen principal a Adobe Dynamic Media Classic y genera derivados de diferente tamaño a partir de la imagen principal.
* Puede cambiar rápidamente el tamaño de una imagen en el sitio web o la aplicación. Por ejemplo, para cambiar todas las imágenes de miniaturas, puede modificar el ajuste preestablecido de imagen &quot;thumbnail&quot;. Un ajuste preestablecido de imagen es una colección de atributos de tamaño y formato. Para cambiar el tamaño de todas las imágenes en miniatura en el sitio web o la aplicación, puede modificar el ajuste preestablecido de imagen en &quot;miniatura&quot;.
* No tiene que administrar los archivos principales ni todos los derivados en ninguno de los sistemas de administración de recursos o contenido.

![Puede crear varias imágenes derivadas con un tamaño diferente a partir del mismo archivo principal de alta resolución](/help/using/assets/is_derivative_sizes_popup.png).

Ver [Tamaño de imagen: Vídeo de formación de Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS).

El siguiente Inicio rápido de ajuste de tamaño de imagen se ha diseñado para ayudarle a empezar a utilizar las técnicas de ajuste de tamaño de imagen en Adobe Dynamic Media Classic. Complete los pasos del 1 al 5. Después de cada paso, hay una referencia cruzada donde puede encontrar más información si la necesita.

## &#x200B;1. Cargar imágenes principales

Cargue las imágenes principales en Adobe Dynamic Media Classic. Adobe Dynamic Media Classic recomienda utilizar imágenes que sean del tamaño máximo que espera utilizar en su sitio web o aplicación. Por ejemplo, si desea que los visualizadores hagan zoom en las imágenes, cargue imágenes que tengan el tamaño más grande al menos 2000 píxeles. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan imágenes TIFF y PNG sin pérdidas.

En la barra de navegación global, selecciona **[!UICONTROL Cargar]** para cargar archivos de tu equipo a una carpeta en Adobe Dynamic Media Classic. Ver [Cargar imágenes principales](uploading-master-images.md#uploading_master_images).

## &#x200B;2. Configurar ajustes preestablecidos de imagen

Un ajuste preestablecido de imagen es un conjunto de comandos predefinidos de tamaño y formato guardados con un nombre. Un ajuste preestablecido de imagen determina el tamaño y el formato con que se envían las imágenes desde los servidores de imágenes de Dynamic Media. Puede configurar ajustes preestablecidos de imagen de forma independiente si tiene el estado de administrador de la empresa. Puede enviar imágenes de forma dinámica utilizando los ajustes preestablecidos de imagen predeterminados incluidos con Adobe Dynamic Media Classic.

Para crear un ajuste preestablecido de imagen (si es administrador), en la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Ajustes preestablecidos de imagen]**. A continuación, seleccione **[!UICONTROL Agregar]** para crear un ajuste preestablecido de imagen o seleccione **[!UICONTROL Editar]** para cambiar un ajuste preestablecido de imagen existente.

El ajuste preestablecido de imagen que cree se añadirá al menú Ajuste preestablecido de imagen de la página Vista previa. Puede utilizarlo para mostrar dinámicamente imágenes en sus sitios Web o aplicaciones. Consulte [Configurar ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

## &#x200B;3. Previsualizar ajustes preestablecidos de imagen

El siguiente paso consiste en obtener una vista previa de los ajustes preestablecidos creados por el administrador en diferentes tamaños.

Para explorar los ajustes preestablecidos de imagen, en la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de imagen]** y, a continuación, busque un ajuste preestablecido de imagen.

Pruebe los diferentes ajustes preestablecidos de imagen. Determine cómo aparece la imagen cuando se envía dinámicamente al sitio web o a la aplicación en diferentes tamaños.

Consulte [Previsualizar un recurso de imagen en función de su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## &#x200B;4. Publicación de las imágenes principales

La publicación de los archivos de imagen principales tiene dos propósitos esenciales:

* Publique las imágenes principales en los servidores de imágenes de Dynamic Media para que las imágenes se puedan enviar de forma dinámica al sitio web y a la aplicación.
* La publicación activa las cadenas URL para llamar a imágenes desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación. Después de la publicación, puede copiar y colocar las direcciones URL generadas por Adobe Dynamic Media Classic donde sea necesario en su sitio web o aplicación.

En la barra de navegación global, seleccione **[!UICONTROL Publicar]** para iniciar un trabajo de publicación. En el cuadro de diálogo Publicación, seleccione **[!UICONTROL Enviar publicación]**. Ver [Publicar imágenes principales](publishing-master-images.md#publishing_master_images).

## &#x200B;5. Vinculación de URL en la aplicación web

Adobe Dynamic Media Classic crea cadenas de llamada de URL para las imágenes. Cuando publica imágenes en servidores de imágenes de Dynamic Media, las direcciones URL se activan. Puede copiar estas cadenas de URL desde el panel Examinar (en la vista de detalles) o la pantalla Vista previa. Después de copiar las cadenas URL, puede utilizarlas en su sitio web o aplicación. La URL para el tamaño de la imagen reemplaza la referencia a un nombre de imagen estático en el código de la página web. La dirección URL hace referencia a un nombre de imagen principal que la base de datos sustituye para cada nueva imagen mostrada.

Las cadenas URL generadas con ajustes preestablecidos de imagen contienen el nombre de un ajuste preestablecido de imagen. Este nombre se incluye entre símbolos de dólar (`$`). Por ejemplo, `$thumbnail$` puede ser el ajuste preestablecido de imagen diseñado para mostrar imágenes principales en tamaño de miniatura. Ver [URL de vínculo a su aplicación web](linking-urls-web-application.md#linking_urls_to_your_web_application).
