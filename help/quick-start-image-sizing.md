---
title: '"Inicio rápido: Cambio de tamaño de imagen"'
seo-title: '"Inicio rápido: Cambio de tamaño de imagen"'
description: nulo
seo-description: Introducción y Inicio rápido al cambio de tamaño de imagen para ayudarle en el uso inicial de las técnicas de cambio de tamaño de imagen.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 56%

---


# Inicio rápido: Cambio de tamaño de imagen{#quick-start-image-sizing}

El cambio de tamaño de imagen hace referencia a la capacidad de Dynamic Media Classic para crear varias imágenes derivadas basadas en una sola imagen de alta resolución. En lugar de crear manualmente varias imágenes (por ejemplo, una miniatura y una imagen de vista ampliada) para la aplicación o el sitio Web, se proporciona una sola imagen principal. Dynamic Media Classic genera todas las imágenes modificadas tal y como las solicita. La creación dinámica de imágenes a partir de una imagen principal aporta diversas ventajas:

* Se elimina la necesidad de crear manualmente varias copias de la misma imagen en diferentes tamaños. Proporciona una imagen principal a Dynamic Media Classic y Dynamic Media Classic genera derivados de diferente tamaño a partir de la imagen principal.
* Se puede cambiar rápidamente el tamaño de un tipo de imagen en toda una aplicación o un sitio web. Por ejemplo, para cambiar todas las miniaturas, puede modificar el ajuste preestablecido de imagen para miniatura. Un ajuste preestablecido de imagen, similar a una macro, se compone de una serie de atributos de formato y tamaño. Puede modificar el ajuste preestablecido de imagen para miniatura para cambiar en una sola operación el tamaño de todas las miniaturas que haya en su aplicación o sitio web.
* Se elimina la necesidad de gestionar las imágenes principales y todas sus derivadas en los sistemas de gestión de recursos o contenido, tanto interna como externamente.

![Puede crear varias imágenes derivadas con un tamaño diferente del mismo archivo maestro de alta resolución.](/help/assets/is_derivative_sizes_popup.png)

**Inicio rápido**

Este Inicio rápido de cambio de tamaño de imagen se ha diseñado para ayudarle en el uso inicial de las técnicas de cambio de tamaño de imagen en Dynamic Media Classic. Siga los pasos del 1 al 5. Después de cada paso hay una referencia cruzada que proporciona más información relevante.

**1. Carga de imágenes principales**

Inicio cargando las imágenes principales en Dynamic Media Classic. En cuanto al tamaño, Dynamic Media Classic recomienda el uso de imágenes que tengan el tamaño más grande que se espera usar en el sitio web o la aplicación. Por ejemplo, si quiere que los visores apliquen zoom, cargue imágenes cuya dimensión superior sea al menos 2000 píxeles. Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan las imágenes TIFF y PNG sin pérdida.

Seleccione el botón Cargar en la barra de navegación global para cargar archivos del equipo en una carpeta de Dynamic Media Classic. Consulte [Carga de imágenes principales](uploading-master-images.md#uploading_master_images).

**2. Configuración de ajustes preestablecidos de imagen**

Un ajuste preestablecido de imagen se compone de una serie de comandos de formato y tamaño predefinidos, que se guarda con un nombre exclusivo; es similar a una macro. Un ajuste preestablecido de imagen determina el tamaño y el formato con los que se entregan las imágenes desde los servidores de imágenes de Dynamic Media. Los administradores pueden crear ajustes preestablecidos de imagen. Dynamic Media Classic también incluye ajustes preestablecidos de imagen predeterminados y puede utilizarlos para distribuir imágenes de forma dinámica.

Para crear un ajuste preestablecido de imagen (si es administrador), elija Ajustes > Ajustes de aplicación. En la pantalla Ajustes, seleccione Ajustes de aplicación y luego Ajustes preestablecidos de imagen. A continuación, haga clic en **Añadir** o en **Editar** para crear un ajuste preestablecido de imagen.

El ajuste creado se incluye en el menú Ajustes preestablecidos de imagen de la pantalla Vista previa. Podrá utilizar el nuevo ajuste preestablecido para mostrar dinámicamente imágenes en sus sitios web o aplicaciones. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

**3. Vista previa de ajustes preestablecidos de imagen**

El siguiente paso consiste en obtener una vista previa de los ajustes preestablecidos creados por el administrador en diferentes tamaños. 

To explore Image Presets, click **Setup** > **Image Presets**, and then browse to an Image Preset.

Experimente con los diversos ajustes. Compruebe el aspecto que tendrá la imagen al distribuirse dinámicamente, con distintos tamaños, a su aplicación o sitio web. 

Consulte [Vista previa de un recurso de imagen en su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicación de imágenes principales**

La publicación de archivos de imágenes principales tiene dos finalidades:

* Publicación de imágenes principales en servidores de imágenes de Dynamic Media para que las imágenes se puedan distribuir dinámicamente en el sitio web y la aplicación.
* La publicación activa las cadenas URL para llamar a imágenes desde los servidores de imágenes de Dynamic Media a su sitio web o aplicación. Después de la publicación, puede copiar y colocar las URL generadas por Dynamic Media Classic cuando sea necesario en su sitio web o aplicación.

Seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. En la pantalla Publicar, seleccione el botón Iniciar publicación. Consulte [Publicación de imágenes principales](publishing-master-images.md#publishing_master_images).

**5. Vinculación de direcciones URL al sitio web**

Dynamic Media Classic crea cadenas de llamada mediante URL para imágenes. Al publicar imágenes en los servidores de imágenes de Dynamic Media, las direcciones URL se activan. Puede copiar estas cadenas URL desde el panel Examinar (en vista de detalles) o desde la pantalla Vista previa. Cuando haya copiado las cadenas URL, podrá usarlas en sus sitios web y en sus aplicaciones. La URL de cambio de tamaño de imagen sustituye a la referencia a un nombre de imagen estática en el código de página web dinámico. La URL hace referencia al nombre de una imagen principal, que la base de datos sustituye por cada nueva imagen que mostrar.

Las cadenas URL generadas con ajustes preestablecidos de imagen contienen el nombre de un ajuste preestablecido de imagen. Este nombre se indica entre signos de dólar (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Consulte [Vinculación de direcciones URL al sitio web](linking-urls-web-application.md#linking_urls_to_your_web_application).
