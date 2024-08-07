---
title: Especificación de opciones de exportación disponibles para los usuarios de Media Portal
description: Obtenga información sobre cómo especificar las opciones de exportación disponibles para los usuarios de Media Portal en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 42%

---

# Especificación de opciones de exportación disponibles para los usuarios de Media Portal {#specifying-export-options-available-to-media-portal-users}

Si el administrador les otorga permiso para hacerlo, los usuarios de Media Portal pueden cambiar el formato de las imágenes al exportarlas. Por ejemplo, pueden cambiar el tamaño, el formato de archivo y la calidad de la imagen. Al cambiar el formato de las imágenes automáticamente a medida que se exportan, se ahorra tiempo, ya que no tiene que formatearlas por separado. Además, los administradores pueden crear un ajuste preestablecido, es decir, una selección preestablecida de configuraciones de formato de imagen. Puede usar un ajuste preestablecido al exportar imágenes para cambiarles el formato conforme a las especificaciones de la empresa.

Si exporta recursos de imagen mediante una conversión definida por el usuario o si exporta imágenes principales originales, se aplican las dos restricciones siguientes:

* El archivo ZIP comprimido de exportación tiene un tamaño máximo de 1 GB para el trabajo de exportación.
* Puede tener un máximo de 500 recursos en total por trabajo de exportación.

Consulte también [Exportar recursos desde Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Para especificar las opciones de exportación disponibles para los usuarios de Media Portal:**

1. En la barra de navegación global, vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.
1. En la ventana Ajustes preestablecidos de imagen, seleccione una de las siguientes opciones:

   * **Habilitar conversión definida por el usuario**: cuando se selecciona, esta opción permite a los usuarios elegir otras opciones de la lista desplegable **[!UICONTROL Tamaño]** en la ventana Exportar Assets seleccionado. Los usuarios pueden elegir una unidad de medida, como píxeles o centímetros, y especificar la anchura y la altura deseadas. Al exportar o descargar estos archivos, se cambia el formato de los archivos de imagen.

     Si se eligen **[!UICONTROL píxeles]** de la lista desplegable **[!UICONTROL Tamaño]**, el ancho × alto de la imagen resultante no puede superar los 100 millones de píxeles. Este tamaño equivale a 10.000 × 10.000 píxeles para una imagen cuadrada, o aproximadamente 8.000 × 12.000 píxeles para una imagen con una relación de aspecto 2x3. Esta limitación de tamaño no se aplica si exporta imágenes principales originales.

     Anule la selección de esta opción para que los usuarios descarguen los archivos sin volver a aplicarles formato a medida que se descargan.

   * **Habilitar la exportación del original**: permite exportar las imágenes principales originales. En el panel **[!UICONTROL Exportar Assets seleccionado]**, los usuarios pueden abrir el menú desplegable **[!UICONTROL Conversión]** y elegir **[!UICONTROL Exportar original]** para exportar los archivos originales. Anule la selección de esta opción si desea obligar a los usuarios a seleccionar un ajuste preestablecido de imagen o sus propias opciones de conversión al exportar imágenes.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de imagen](application-setup.md#image_presets)
>* [Elegir permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
