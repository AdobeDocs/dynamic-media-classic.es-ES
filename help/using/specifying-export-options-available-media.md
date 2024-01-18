---
title: Especificación de opciones de exportación disponibles para los usuarios de Media Portal
description: Obtenga información sobre cómo especificar las opciones de exportación disponibles para los usuarios de Media Portal en Adobe Dynamic Media Classic.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 41%

---

# Especificación de opciones de exportación disponibles para los usuarios de Media Portal {#specifying-export-options-available-to-media-portal-users}

Si el administrador les otorga permiso para hacerlo, los usuarios de Media Portal pueden cambiar el formato de las imágenes al exportarlas. Por ejemplo, pueden cambiar el tamaño, el formato de archivo y la calidad de la imagen. Al cambiar el formato de las imágenes automáticamente a medida que se exportan, se ahorra tiempo, ya que no tiene que formatearlas por separado. Además, los administradores pueden crear un ajuste preestablecido, es decir, una selección preestablecida de configuraciones de formato de imagen. Puede usar un ajuste preestablecido al exportar imágenes para cambiarles el formato conforme a las especificaciones de la empresa.

Si exporta recursos de imagen mediante una conversión definida por el usuario o si exporta imágenes principales originales, se aplican las dos restricciones siguientes:

* El archivo ZIP comprimido de exportación tiene un tamaño máximo de 1 GB para el trabajo de exportación.
* Puede tener un máximo de 500 recursos en total por trabajo de exportación.

Consulte también [Exportación de recursos desde Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Para especificar las opciones de exportación disponibles para los usuarios de Media Portal:**

1. En la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.
1. En la ventana Ajustes preestablecidos de imagen, seleccione una de las siguientes opciones:

   * **Habilitar conversión definida por el usuario** : cuando se selecciona, esta opción permite a los usuarios elegir otras opciones del **[!UICONTROL Tamaño]** en la ventana Exportar recursos seleccionados. Los usuarios pueden elegir una unidad de medida, como píxeles o centímetros, y especificar la anchura y la altura deseadas. Al exportar o descargar estos archivos, se cambia el formato de los archivos de imagen.

     Cuándo **[!UICONTROL píxeles]** se eligen de la **[!UICONTROL Tamaño]** , la anchura × altura de la imagen resultante no puede superar los 100 millones de píxeles. Este tamaño equivale a 10.000 × 10.000 píxeles para una imagen cuadrada, o aproximadamente 8.000 × 12.000 píxeles para una imagen con una relación de aspecto 2x3. Esta limitación de tamaño no se aplica si exporta imágenes principales originales.

     Anule la selección de esta opción si desea que los usuarios descarguen archivos sin cambiar el formato al descargarlos.

   * **Habilitar la exportación del original** : permite exportar imágenes principales originales. En el **[!UICONTROL Exportar recursos seleccionados]** , los usuarios pueden abrir el panel **[!UICONTROL Conversión]** menú desplegable y elija **[!UICONTROL Exportar original]** para exportar archivos originales. Anule la selección de esta opción si desea obligar a los usuarios a elegir un ajuste preestablecido de imagen o a elegir opciones de conversión al exportar imágenes.

>[!MORELIKETHIS]
>
>* [Ajustes preestablecidos de imagen](application-setup.md#image_presets)
>* [Elija permisos de acceso a ajustes preestablecidos de imagen para un grupo](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
