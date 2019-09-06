---
title: Especificación de opciones de exportación disponibles para usuarios de Media Portal
seo-title: Especificación de opciones de exportación disponibles para usuarios de Media Portal
description: nulo
seo-description: Aprenda a especificar las opciones de exportación disponibles para los usuarios de Media Portal.
uuid: 5258 b 8 a 4-0704-43 cd -97 d 1-c 9 af 2 e 4 e 298 b
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 9 bfd 95 da -3714-4 e 38-98 af -331 a 04 c 685 f 5
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Especificación de opciones de exportación disponibles para los usuarios de Media Portal {#specifying-export-options-available-to-media-portal-users}

Si el administrador les otorga permiso para hacerlo, los usuarios de Media Portal pueden cambiar el formato de las imágenes al exportarlas. Por ejemplo, pueden cambiar el tamaño, el formato de archivo y la calidad de la imagen. Al cambiar el formato de las imágenes automáticamente a medida que se exportan, se ahorra tiempo, ya que no tiene que formatearlas por separado. Además, los administradores pueden crear un ajuste preestablecido, es decir, una selección preestablecida de configuraciones de formato de imagen. Puede usar un ajuste preestablecido al exportar imágenes para cambiarles el formato conforme a las especificaciones de la empresa.

Las dos restricciones siguientes se aplican si exporta recursos de imagen por medio de una conversión definida por el usuario o si exporta imágenes principales originales:

* El archivo ZIP comprimido de exportación tiene un tamaño máximo de 1 GB para el trabajo de exportación.
* Puede tener un máximo de 500 recursos en total por trabajo de exportación.

Consulte también [Exportación de recursos de Scene7 Publishing System](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system).

**Para especificar las opciones de exportación disponibles para los usuarios de Media Portal**

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de imagen**.
1. En la ventana Ajustes preestablecidos de imagen, seleccione una de las siguientes opciones:

   **Activar conversión definida por el usuario** Cuando se selecciona, esta opción permite a los usuarios elegir otro en la lista desplegable Tamaño de la ventana Exportar recursos seleccionados. A continuación, los usuarios pueden elegir una unidad de medida como, por ejemplo, píxeles o centímetros, y especificar la anchura y la altura deseadas. Al exportar o descargar estos archivos, se cambia el formato de los archivos de imagen.

   Cuando se eligen **píxeles** de la lista desplegable **Tamaño**, la anchura x la altura de la imagen resultante no puede superar los 100 millones de píxeles. Este tamaño equivale a 10.000 x 10.000 píxeles para una imagen cuadrada, o aproximadamente 8.000 x 12.000 píxeles para una imagen con una proporción de aspecto 2x3. Esta restricción de tamaño no se aplica si exporta imágenes principales originales.

   Anule la selección de esta opción si desea que los usuarios descarguen archivos sin cambiar el formato al descargarlos.

   **Activar exportación original** Permite exportar imágenes principales originales. En el cuadro de diálogo Exportar recursos seleccionados, los usuarios pueden abrir el menú desplegable Conversión y elegir Exportar original para exportar los archivos originales. Anule la selección de esta opción si desea obligar a los usuarios a seleccionar un ajuste preestablecido de imagen o sus propias opciones de conversión al exportar imágenes.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de imagen](application-setup.md#image_presets)
>* [Elección de permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

