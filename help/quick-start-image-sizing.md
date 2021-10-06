---
title: '"Inicio rápido: Cambio de tamaño de imagen"'
description: Introducción y tamaño rápido de la imagen para ayudarle a poner en marcha rápidamente las técnicas de cambio de tamaño de la imagen en Adobe Dynamic Media Classic.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 29%

---

# Inicio rápido: Cambio de tamaño de imagen{#quick-start-image-sizing}

El tamaño de la imagen se refiere a la capacidad de Adobe Dynamic Media Classic para crear varias imágenes derivadas basadas en una sola imagen de alta resolución. En lugar de crear manualmente varias imágenes (por ejemplo, una miniatura y una imagen de vista ampliada) para el sitio web o la aplicación, proporciona una sola imagen maestra. Adobe Dynamic Media Classic genera todas las imágenes modificadas tal como las solicita. La creación dinámica de imágenes a partir de una imagen principal aporta diversas ventajas:

* Se elimina la necesidad de crear manualmente varias copias de la misma imagen en diferentes tamaños. Se proporciona una imagen maestra a Adobe Dynamic Media Classic y Adobe Dynamic Media Classic genera derivados de diferente tamaño a partir de la imagen maestra.
* Se puede cambiar rápidamente el tamaño de un tipo de imagen en toda una aplicación o un sitio web. Por ejemplo, para cambiar todas las miniaturas, puede modificar el ajuste preestablecido de imagen para miniatura. Un ajuste preestablecido de imagen, similar a una macro, se compone de una serie de atributos de formato y tamaño. Puede modificar el ajuste preestablecido de imagen para miniatura para cambiar en una sola operación el tamaño de todas las miniaturas que haya en su aplicación o sitio web.
* No es necesario que administre los maestros y todos los derivados en ninguno de los sistemas de gestión de recursos o contenido interna o externamente.

![Puede crear varias imágenes derivadas a un tamaño diferente del mismo archivo maestro de alta resolución.](/help/assets/is_derivative_sizes_popup.png)

Consulte [Tamaño de imagen: Vídeo de formación del Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS).

El siguiente inicio rápido sobre el tamaño de la imagen está diseñado para ayudarle a poner en marcha rápidamente las técnicas de cambio de tamaño de la imagen en Adobe Dynamic Media Classic. Siga los pasos del 1 al 5. Después de cada paso hay una referencia cruzada que proporciona más información relevante.

## 1. Cargar imágenes principales

Comience por cargar las imágenes principales a Adobe Dynamic Media Classic. En cuanto al tamaño, Adobe Dynamic Media Classic recomienda utilizar imágenes que tengan el tamaño más grande previsto para su sitio web o aplicación. Por ejemplo, si desea que los espectadores amplíen las imágenes, cargue imágenes que tengan al menos 2000 píxeles de tamaño mayor. Adobe Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan TIFF sin pérdida e imágenes PNG.

En la barra de navegación global, seleccione **[!UICONTROL Upload]** para cargar archivos del equipo a una carpeta de Adobe Dynamic Media Classic. Consulte [Cargar imágenes maestras](uploading-master-images.md#uploading_master_images).

## 2. Configurar ajustes preestablecidos de imagen

Un ajuste preestablecido de imagen se compone de una serie de comandos de formato y tamaño predefinidos, que se guarda con un nombre exclusivo; es similar a una macro. Los ajustes preestablecidos de imagen rigen el tamaño y el formato con que se entregan las imágenes desde los servidores de imágenes de Dynamic Media. Los administradores pueden crear ajustes preestablecidos de imagen. Adobe Dynamic Media Classic también incluye ajustes preestablecidos de imagen predeterminados y puede utilizarlos para distribuir imágenes de forma dinámica.

Para crear un ajuste preestablecido de imagen (si es un administrador), en la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Ajustes preestablecidos de imagen]**. A continuación, seleccione **[!UICONTROL Agregar]** para crear un ajuste preestablecido de imagen o seleccione **[!UICONTROL Editar]** para cambiar un ajuste preestablecido de imagen existente.

El ajuste preestablecido de imagen que cree se agregará al menú Ajuste preestablecido de imagen de la página Vista previa. Podrá utilizar el nuevo ajuste preestablecido para mostrar dinámicamente imágenes en sus sitios web o aplicaciones. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

## 3. Previsualizar ajustes Preestablecidos De Imagen

El siguiente paso consiste en obtener una vista previa de los ajustes preestablecidos creados por el administrador en diferentes tamaños. 

Para explorar los ajustes preestablecidos de imagen, en la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de imagen]** y, a continuación, busque un ajuste preestablecido de imagen.

Experimente con los diversos ajustes. Descubra cómo aparece la imagen cuando se entrega de forma dinámica a su sitio web o aplicación a diferentes tamaños.

Consulte [Vista previa de un recurso de imagen en función de su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Publicar las imágenes principales

La publicación de archivos de imágenes principales tiene dos finalidades:

* Publicación de las imágenes principales en los servidores de imágenes de Dynamic Media para que las imágenes se puedan enviar de forma dinámica al sitio web y a la aplicación.
* La publicación activa las cadenas URL para llamar a imágenes desde servidores de imágenes de Dynamic Media a su sitio web o aplicación. Después de la publicación, puede copiar y colocar las URL generadas por Adobe Dynamic Media Classic donde sea necesario en su sitio web o aplicación.

En la barra de navegación global, seleccione **[!UICONTROL Publicar]** para iniciar un trabajo de publicación. En el cuadro de diálogo Publicar, seleccione **[!UICONTROL Enviar publicación]**. Consulte [Publicar imágenes maestras](publishing-master-images.md#publishing_master_images).

## 5. Vincular URL a la aplicación web

Adobe Dynamic Media Classic crea cadenas de llamada URL para imágenes. Cuando publica imágenes en los servidores de imágenes de Dynamic Media, las direcciones URL se activan. Puede copiar estas cadenas URL desde el panel Examinar (en la Vista de detalles) o la pantalla Vista previa. Cuando haya copiado las cadenas URL, podrá usarlas en sus sitios web y en sus aplicaciones. La URL de cambio de tamaño de imagen sustituye a la referencia a un nombre de imagen estática en el código de página web dinámico. La URL hace referencia al nombre de una imagen principal, que la base de datos sustituye por cada nueva imagen que mostrar.

Las cadenas URL generadas con ajustes preestablecidos de imagen contienen el nombre de un ajuste preestablecido de imagen. Este nombre se indica entre signos de dólar (`$`). Por ejemplo, `$thumbnail$` puede ser el ajuste preestablecido de imagen diseñado para mostrar imágenes principales con tamaño de miniatura. Consulte [Vincular URL a su aplicación web](linking-urls-web-application.md#linking_urls_to_your_web_application).
