---
title: '"Inicio rápido: Cambio de tamaño de imagen"'
seo-title: '"Inicio rápido: Cambio de tamaño de imagen"'
description: nulo
seo-description: Introducción e Inicio rápido a Tamaño de imagen para ayudarle en el uso inicial de las técnicas de cambio de tamaño de imagen.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: dcaa 9 b 21-b 925-4 dbb -865 e -7918 cdbda 50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Inicio rápido: Cambio de tamaño de imagen{#quick-start-image-sizing}

El tamaño de imagen hace referencia a la capacidad de Dynamic Media Classic para crear varias imágenes derivadas en función de una sola imagen de alta resolución. En lugar de crear manualmente varias imágenes (por ejemplo, una miniatura y una imagen de vista ampliada) para su sitio Web o aplicación, debe proporcionar una sola imagen principal. Dynamic Media Classic genera todas las imágenes modificadas al mismo medida que las solicita. La creación dinámica de imágenes a partir de una imagen principal aporta diversas ventajas:

* Se elimina la necesidad de crear manualmente varias copias de la misma imagen en diferentes tamaños. Puede proporcionar una imagen principal a Dynamic Media Classic y Dynamic Media Classic genera derivados de distintos tamaños a partir de la imagen principal.
* Se puede cambiar rápidamente el tamaño de un tipo de imagen en toda una aplicación o un sitio web. Por ejemplo, para cambiar todas las miniaturas, puede modificar el ajuste preestablecido de imagen para miniatura. Un ajuste preestablecido de imagen, similar a una macro, se compone de una serie de atributos de formato y tamaño. Puede modificar el ajuste preestablecido de imagen para miniatura para cambiar en una sola operación el tamaño de todas las miniaturas que haya en su aplicación o sitio web.
* Se elimina la necesidad de gestionar las imágenes principales y todas sus derivadas en los sistemas de gestión de recursos o contenido, tanto interna como externamente.

![Puede crear varias imágenes derivadas a partir de un tamaño distinto a partir del mismo archivo principal de alta resolución.](/help/assets/is_derivative_sizes_popup.png)

**Inicio rápido**

Estas instrucciones de inicio rápido se han diseñado para agilizar el aprendizaje de las técnicas de cambio de tamaño de imagen en Scene7 Publishing System. Siga los pasos 1-5. Después de cada paso hay una referencia cruzada que proporciona más información relevante.

**1. Carga de imágenes principales**

Comience por cargar las imágenes principales en Scene7 Publishing System. En cuanto a tamaño, Dynamic Media Classic recomienda utilizar imágenes con el tamaño máximo que se piense utilizar en el sitio web o en la aplicación. Por ejemplo, si quiere que los visores apliquen zoom, cargue imágenes cuya dimensión superior sea al menos 2000 píxeles. Dynamic Media Classic admite muchos formatos de archivo de imagen, pero se recomiendan las imágenes TIFF y PNG sin pérdida.

Seleccione el botón Cargar en la barra de navegación global para cargar archivos del ordenador en una carpeta de Scene7 Publishing System. Consulte [Carga de imágenes principales](uploading-master-images.md#uploading_master_images).

**2. Configuración de ajustes preestablecidos de imagen**

Un ajuste preestablecido de imagen se compone de una serie de comandos de formato y tamaño predefinidos, que se guarda con un nombre exclusivo; es similar a una macro. Un ajuste preestablecido de imagen rige el tamaño y el formato con el que se envían las imágenes desde los servidores de imágenes de Dynamic Media. Los administradores pueden crear ajustes preestablecidos de imagen. Dynamic Media Classic también incluye ajustes preestablecidos de imagen predeterminados y puede utilizarlos para distribuir imágenes dinámicamente.

Para crear un ajuste preestablecido de imagen (si es administrador), elija Ajustes &gt; Ajustes de aplicación. En la pantalla Ajustes, seleccione Ajustes de aplicación y luego Ajustes preestablecidos de imagen. A continuación, haga clic **en Agregar** o **Editar** para crear un ajuste preestablecido de imagen.

El ajuste creado se incluye en el menú Ajustes preestablecidos de imagen de la pantalla Vista previa. Podrá utilizar el nuevo ajuste preestablecido para mostrar dinámicamente imágenes en sus sitios web o aplicaciones. Consulte [Configuración de ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

**3. Vista previa de ajustes preestablecidos de imagen**

El siguiente paso consiste en obtener una vista previa de los ajustes preestablecidos creados por el administrador en diferentes tamaños. 

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

Experimente con los diversos ajustes. Compruebe el aspecto que tendrá la imagen al distribuirse dinámicamente, con distintos tamaños, a su aplicación o sitio web. 

Consulte [Vista previa de un recurso de imagen en su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Publicación de imágenes principales**

La publicación de archivos de imágenes principales tiene dos finalidades:

* Publicar las imágenes principales en servidores de imágenes de Dynamic Media para que las imágenes se puedan distribuir de forma dinámica al sitio web y a la aplicación.
* La publicación activa las cadenas URL para llamar a imágenes desde servidores de imágenes de Dynamic Media hasta su sitio web o aplicación. Después de la publicación, puede copiar y colocar las URL generadas por Dynamic Media Classic en las que sea necesario en su sitio web o aplicación.

Seleccione el botón Publicar en la barra de navegación global para iniciar una publicación. En la pantalla Publicar, seleccione el botón Iniciar publicación. Consulte [Publicación de imágenes principales](publishing-master-images.md#publishing_master_images).

**5. Vinculación de direcciones URL al sitio web**

Dynamic Media Classic crea cadenas de llamada URL para imágenes. Cuando publica imágenes en servidores de imágenes de Dynamic Media, las URL pasan a estar activas. Puede copiar estas cadenas URL desde el panel Examinar (en vista de detalles) o desde la pantalla Vista previa. Cuando haya copiado las cadenas URL, podrá usarlas en sus sitios web y en sus aplicaciones. La URL de cambio de tamaño de imagen sustituye a la referencia a un nombre de imagen estática en el código de página web dinámico. La URL hace referencia al nombre de una imagen principal, que la base de datos sustituye por cada nueva imagen que mostrar.

Las cadenas URL generadas con ajustes preestablecidos de imagen contienen el nombre de un ajuste preestablecido de imagen. Este nombre se indica entre signos de dólar (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Consulte [Vinculación de direcciones URL al sitio web](linking-urls-web-application.md#linking_urls_to_your_web_application).
