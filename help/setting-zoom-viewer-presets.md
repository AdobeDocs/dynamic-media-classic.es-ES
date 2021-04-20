---
title: Configuración de ajustes preestablecidos de visor de zoom
description: Aprenda a configurar los ajustes preestablecidos del visor de zoom.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 68%

---


# Configuración de ajustes preestablecidos de visor de zoom{#setting-up-zoom-viewer-presets}

Los ajustes preestablecidos de visor de zoom determinan el estilo, el comportamiento y el aspecto de los visores de zoom. Dynamic Media Classic ofrece muchas opciones para personalizar y desollar visualizadores. Dynamic Media Classic incluye ajustes preestablecidos básicos (rápidos), flotantes y de visor de zoom personalizado. Si es administrador, puede crear nuevos ajustes preestablecidos de visor de zoom para su empresa o editar un ajuste preestablecido de visor de zoom predeterminado y guardarlo con un nombre nuevo.

Todos los visores de zoom tienen botones para acercar, alejar, desplazar y restablecer la imagen a su estado original tras la aplicación de zoom. El aspecto de estos botones y el de la ventana depende de la selección de ajustes preestablecidos de visor de zoom. Los ajustes preestablecidos de visor de zoom se pueden configurar con diferentes colores, bordes, fuentes y parámetros de imagen. Al configurar un visor de zoom guiado, también puede elegir dónde colocar los destinos de zoom. Los destinos de zoom son miniaturas en las que hacen clic los usuarios para aplicar zoom en áreas que se hayan especificado.

## Acerca de los ajustes preestablecidos de visor de zoom {#about-zoom-viewer-presets}

Dynamic Media Classic ofrece estos ajustes preestablecidos de visor de zoom:

* **Visor de zoom:**
BásicoProporciona un zoom básico en la imagen original.

* **Visor de zoom: Salida**
Muestra una segunda imagen del área ampliada junto a la imagen original. No hay controles, los usuarios simplemente mueven la selección sobre la zona que desean ver.

Al determinar el uso del ancho de banda completo para este visor, tenga en cuenta que tanto la imagen principal como la imagen flotante se muestran en el visor. El tamaño de la imagen flotante viene determinado por el tamaño de la imagen principal (anchura y altura de escenario) y el factor de zoom. Para evitar que el tamaño del archivo flotante sea demasiado grande, equilibre estos dos valores: si el tamaño de la imagen principal es muy grande, reduzca el valor de Factor de zoom. (Los valores de Anchura flotante y Altura flotante determinan el tamaño de la ventana flotante, pero no el tamaño de la imagen que se muestra en el visor).

Por ejemplo, si el tamaño de la imagen principal es 350 x 350 píxeles, con un factor de zoom de 3, el tamaño de la imagen flotante que resultará será de 1050 x 1050 píxeles. Si el tamaño de la imagen principal es de 300 x 300 píxeles, con un factor de zoom de 4, el tamaño de la imagen flotante será de 1200 x 1200 píxeles. Según el ajuste de calidad JPEG (el recomendado es entre 80 y 90), podrá reducir el tamaño del archivo en gran medida. Los factores de zoom recomendados son de 2,5 a 4, según el tamaño de la imagen principal.

Dynamic Media Classic recomienda estos parámetros para los ajustes preestablecidos del visor de zoom flotante:

* **Tamaño de imagen**
ampliadoAproximadamente 1500 por 1500 píxeles, sin superar los 2000 por 2000 píxeles.

* **Tamaño de la imagen**
100 KB o menos, no superior a 150 KB (comprima el archivo para mantenerlo por debajo de 150 KB).

* **Visor de zoom:**
PersonalizadoProporciona zoom guiado o no guiado con imágenes, conjuntos de imágenes con varias vistas o conjuntos de muestras de color.

## Creación y edición de ajustes preestablecidos de visor de zoom {#creating-and-editing-zoom-viewer-presets}

Siga estos pasos para crear o editar un ajuste preestablecido de visor de zoom:

1. Haga clic en **Ajustes** > **Ajustes preestablecidos de visor**.
1. Realice una de las siguientes acciones:

   * **Creación de un**
ajuste preestablecidoHaga clic en Agregar. En el cuadro de diálogo Agregar ajuste preestablecido de visualizador, seleccione una plataforma, elija un visualizador de zoom y, a continuación, haga clic en Agregar. Introduzca un nombre para el ajuste preestablecido en el cuadro Nombre del ajuste preestablecido.

   * **Edición de un**
ajuste preestablecidoSeleccione un ajuste preestablecido de visor de zoom y haga clic en 
**Editar**.

1. Especifique los ajustes que desee.

   Para ver una descripción de una opción, haga clic en el icono de información  que aparece junto a ella.

   La pantalla Vista previa muestra el visor mientras actualiza y cambia la configuración.

1. Haga clic en **Guardar** o **Guardar como**.
1. En la pantalla Ajustes preestablecidos de visor, examine el ajuste preestablecido de visor de zoom o el ajuste preestablecido de visor de zoom guiado que haya creado. Si es necesario realizar ajustes, haga clic en **Editar**, cambie la configuración en la pantalla Configurar visor y haga clic en **Guardar**.

Para obtener más información sobre la gestión de valores preestablecidos de visor en la pantalla Ajustes preestablecidos de visor, consulte [Ajustes preestablecidos de visor](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Creación y edición de ajustes preestablecidos de visor](application-setup.md#adding_and_editing_viewer_presets)

