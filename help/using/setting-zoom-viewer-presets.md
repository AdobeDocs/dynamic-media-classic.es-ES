---
title: Configurar ajustes preestablecidos del visor de zoom
description: Obtenga información sobre cómo configurar ajustes preestablecidos del visor de zoom en Adobe Dynamic Media Classic.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 47%

---

# Configurar ajustes preestablecidos del visor de zoom{#setting-up-zoom-viewer-presets}

Los ajustes preestablecidos de visor de zoom determinan el estilo, el comportamiento y el aspecto de los visores de zoom. Adobe Dynamic Media Classic ofrece muchas opciones para personalizar y desollar visores. Adobe Dynamic Media Classic incluye ajustes preestablecidos básicos (rápidos), desplegables y personalizados del visor de zoom predeterminados. Si es administrador, puede crear ajustes preestablecidos del visor de zoom de la empresa o editar un ajuste preestablecido predeterminado y guardarlo con un nombre nuevo.

Todos los visores de zoom tienen botones para acercar, alejar, desplazar y restablecer la imagen a su estado original tras la aplicación de zoom. El aspecto de estos botones y el modo en que aparece la ventana dependen de la selección de los ajustes preestablecidos del visor de zoom. Los ajustes preestablecidos de visor de zoom se pueden configurar con diferentes colores, bordes, fuentes y parámetros de imagen. Al configurar un visor de zoom guiado, también puede elegir dónde colocar los destinos de zoom. Los destinos de zoom son miniaturas en las que hacen clic los usuarios para aplicar zoom en áreas que se hayan especificado.

## Acerca de los ajustes preestablecidos de visor de zoom {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic ofrece los siguientes ajustes preestablecidos de visor de zoom:

* **Visor de zoom: Básico** - Proporciona un zoom básico sobre la imagen original.

* **Visor de zoom: Flotante** - Muestra una segunda imagen del área ampliada junto a la imagen original. No hay controles, los usuarios simplemente mueven la selección sobre la zona que desean ver.

Al determinar el uso del ancho de banda completo para este visor, tenga en cuenta que tanto la imagen principal como la imagen flotante se muestran en el visor. El tamaño de la imagen flotante viene determinado por el tamaño de la imagen principal (anchura y altura de escenario) y el factor de zoom. Para evitar que el tamaño del archivo flotante sea demasiado grande, equilibre estos dos valores: si el tamaño de la imagen principal es muy grande, reduzca el valor de Factor de zoom. (Los valores de Anchura flotante y Altura flotante determinan el tamaño de la ventana flotante, pero no el tamaño de la imagen que se muestra en el visor).

Por ejemplo, si el tamaño de la imagen principal es 350 x 350 píxeles, con un factor de zoom de 3, el tamaño de la imagen flotante que resultará será de 1050 x 1050 píxeles. Si el tamaño de la imagen principal es de 300 x 300 píxeles, con un factor de zoom de 4, el tamaño de la imagen flotante será de 1200 x 1200 píxeles. Según el ajuste de calidad JPEG (el recomendado es entre 80 y 90), podrá reducir el tamaño del archivo en gran medida. Los factores de zoom recomendados son de 2,5 a 4, según el tamaño de la imagen principal.

Adobe Dynamic Media Classic recomienda los siguientes parámetros para ajustes preestablecidos del visor de zoom flotantes:

* **Tamaño de imagen ampliado** - Aproximadamente 1500 por 1500 píxeles, sin superar los 2000 por 2000 píxeles.

* **Tamaño de imagen** - 100 KB o menos, no debe superar los 150 KB (comprima el archivo para mantenerlo por debajo de 150 KB).

* **Visor de zoom: Personalizado** - Proporciona zoom guiado o no guiado con imágenes, conjuntos de imágenes con varias vistas o conjuntos de muestras de color.

## Crear y editar ajustes preestablecidos del visor de zoom {#creating-and-editing-zoom-viewer-presets}

1. En la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes preestablecidos de visor]**.
1. Realice una de las siguientes acciones:

   * **Crear un ajuste preestablecido** - Seleccionar **[!UICONTROL Añadir]**. En el cuadro de diálogo Agregar ajuste preestablecido de visor, elija una plataforma, elija un visor de zoom y, a continuación, seleccione **[!UICONTROL Añadir]**. Introduzca un nombre para el ajuste preestablecido en el cuadro Nombre del ajuste preestablecido.

   * **Editar un ajuste preestablecido** - Seleccione un ajuste preestablecido de visor de zoom y, a continuación, seleccione **[!UICONTROL Editar]**.

1. Especifique los ajustes que desee.

   Para ver la descripción de una opción, seleccione la **[!UICONTROL Sugerencia de información]** junto a la opción.

   La página Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. Seleccionar **[!UICONTROL Guardar]** o **[!UICONTROL Guardar como]**.
1. En la página Ajustes preestablecidos del visor, examine los ajustes preestablecidos del visor de zoom o del visor de zoom guiado que ha creado. Si es necesario ajustarlo, seleccione **[!UICONTROL Editar]**, cambie la configuración en la página Configurar visor y seleccione **[!UICONTROL Guardar]**.

Para obtener más información sobre la gestión de valores preestablecidos de visor en la pantalla Ajustes preestablecidos de visor, consulte [Ajustes preestablecidos de visor](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Crear y editar ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets)
