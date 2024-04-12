---
title: "Inicio rápido: Tamaño de la imagen"
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
source-git-commit: 3dbab811a92363150cf465cd02d31a9e82b62d14
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 17%

---

# Inicio rápido: Cambio de tamaño de imagen{#quick-start-image-sizing}

El tamaño de imagen hace referencia a la capacidad de Adobe Dynamic Media Classic para crear varias imágenes derivadas basadas en una sola imagen de alta resolución. En lugar de crear manualmente varias imágenes (por ejemplo, una miniatura y una imagen de vista ampliada) para el sitio web o la aplicación, se proporciona una sola imagen principal. Adobe Dynamic Media Classic genera todas las imágenes modificadas tal como se solicitan. Poder entregar imágenes dinámicamente desde una sola imagen principal tiene muchas ventajas:

* Se elimina la necesidad de crear manualmente varias copias de la misma imagen en diferentes tamaños. Se proporciona una imagen principal a Adobe Dynamic Media Classic y Adobe Dynamic Media Classic genera derivados de diferente tamaño a partir de la imagen principal.
* Se puede cambiar rápidamente el tamaño de un tipo de imagen en toda una aplicación o un sitio web. Por ejemplo, para cambiar todas las imágenes de miniaturas, puede modificar el ajuste preestablecido de imagen &quot;thumbnail&quot;. Un ajuste preestablecido de imagen (similar a una macro) es un conjunto de atributos de tamaño y formato. Puede modificar el ajuste preestablecido de imagen en &quot;miniatura&quot; para cambiar el tamaño de todas las imágenes en miniatura en el sitio web o la aplicación.
* No tiene que administrar los archivos principales y todos los derivados en ninguno de los sistemas de administración de recursos o contenido de forma interna o externa.

![Puede crear varias imágenes derivadas con un tamaño diferente desde el mismo archivo principal de alta resolución.](/help/using/assets/is_derivative_sizes_popup.png)

Consulte [Tamaño de la imagen: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) vídeo de formación.

La siguiente Guía de inicio rápido para el tamaño de imágenes está diseñada para ayudarle a ponerse en marcha rápidamente con las técnicas de tamaño de imágenes de Adobe Dynamic Media Classic. Siga los pasos del 1 al 5. Después de cada paso, hay una referencia cruzada donde puede encontrar más información si la necesita.

## 1. Cargar imágenes principales

Comience por cargar las imágenes principales en Adobe Dynamic Media Classic. En cuanto al tamaño, Adobe Dynamic Media Classic recomienda utilizar imágenes que tengan el tamaño más grande esperado en el sitio web o la aplicación. Por ejemplo, si desea que los visualizadores hagan zoom en las imágenes, cargue imágenes que tengan el tamaño más grande al menos 2000 píxeles. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan imágenes de TIFF y PNG sin pérdidas.

En la barra de navegación global, seleccione **[!UICONTROL Cargar]** para cargar archivos desde el equipo a una carpeta de Adobe Dynamic Media Classic. Consulte [Cargar imágenes principales](uploading-master-images.md#uploading_master_images).

## 2. Configurar ajustes preestablecidos de imagen

Un ajuste preestablecido de imagen se compone de una serie de comandos de formato y tamaño predefinidos, que se guarda con un nombre exclusivo; es similar a una macro. Un ajuste preestablecido de imagen determina el tamaño y el formato con el que se envían las imágenes desde los servidores de imágenes de Dynamic Media. Los administradores pueden crear ajustes preestablecidos de imagen. Adobe Dynamic Media Classic también incluye ajustes preestablecidos de imagen predeterminados y puede utilizarlos para entregar imágenes de forma dinámica.

Para crear un ajuste preestablecido de imagen (si es administrador), en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de imagen]**. A continuación seleccione **[!UICONTROL Añadir]** para crear un ajuste preestablecido de imagen, o seleccione **[!UICONTROL Editar]** para cambiar un ajuste preestablecido de imagen existente.

El ajuste preestablecido de imagen que cree se añadirá al menú Ajuste preestablecido de imagen de la página Vista previa. Podrá utilizar el nuevo ajuste preestablecido para mostrar dinámicamente imágenes en sus sitios web o aplicaciones. Consulte [Configurar ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

## 3. Previsualizar ajustes preestablecidos de imagen

El siguiente paso consiste en obtener una vista previa de los ajustes preestablecidos creados por el administrador en diferentes tamaños. 

Para explorar los ajustes preestablecidos de imagen, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de imagen]** y, a continuación, vaya a un ajuste preestablecido de imagen.

Experimente con los diversos ajustes. Descubra cómo aparece la imagen cuando se envía dinámicamente al sitio web o a la aplicación en diferentes tamaños.

Consulte [Previsualizar un recurso de imagen en función de su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publicar las imágenes principales

La publicación de los archivos de imagen principales tiene dos propósitos esenciales:

* Publicación de las imágenes principales en los servidores de imágenes de Dynamic Media para que las imágenes se puedan enviar de forma dinámica al sitio web y a la aplicación.
* La publicación activa las cadenas URL para llamar a las imágenes de los servidores de imágenes de Dynamic Media en el sitio web o la aplicación. Después de la publicación, puede copiar y colocar las direcciones URL generadas por Adobe Dynamic Media Classic donde sea necesario en su sitio web o aplicación.

En la barra de navegación global, seleccione **[!UICONTROL Publish]** para iniciar un trabajo de publicación. En el cuadro de diálogo Publicación, seleccione **[!UICONTROL Enviar publicación]**. Consulte [Publicación de imágenes principales](publishing-master-images.md#publishing_master_images).

## 5. Vincular URL en la aplicación web

Adobe Dynamic Media Classic crea cadenas de llamada de URL para las imágenes. Al publicar imágenes en los servidores de imágenes de Dynamic Media, las direcciones URL se activan. Puede copiar estas cadenas de URL desde el panel de exploración (en la vista de detalles) o la pantalla de vista previa. Cuando haya copiado las cadenas URL, podrá usarlas en sus sitios web y en sus aplicaciones. La URL de cambio de tamaño de imagen sustituye a la referencia a un nombre de imagen estática en el código de página web dinámico. La dirección URL hace referencia a un nombre de imagen principal, que se sustituye por la base de datos para que se muestre cada imagen nueva.

Las cadenas URL generadas con ajustes preestablecidos de imagen contienen el nombre de un ajuste preestablecido de imagen. Este nombre se incluye entre símbolos de dólar (`$`). Por ejemplo, `$thumbnail$` puede ser el ajuste preestablecido de imagen diseñado para mostrar imágenes principales en tamaño de miniatura. Consulte [Vinculación de URL en la aplicación web](linking-urls-web-application.md#linking_urls_to_your_web_application).
