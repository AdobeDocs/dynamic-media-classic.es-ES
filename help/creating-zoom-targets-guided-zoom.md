---
title: Creación de destinos de zoom para zoom guiado
description: Aprenda a crear destinos de zoom para zoom guiado.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Visualizadores,Zoom
role: Profesional empresarial
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 68%

---


# Creación de destinos de zoom para zoom guiado{#creating-zoom-targets-for-guided-zoom}

Los destinos de zoom guían a ciertas partes de una imagen. Además de aplicar zoom de forma libre, es posible aplicar zoom en la parte deseada de la imagen al hacer clic en la miniatura de destino de zoom correspondiente. Los destinos de zoom permiten resaltar las partes atractivas o interesantes de una imagen.

![Creación de destinos de zoom para zoom guiado](/help/assets/zo_guided_zoom.png)

## Acerca de los destinos de zoom {#about-zoom-targets}

El valor máximo de zoom en los destinos de zoom es 100%. El porcentaje mínimo de zoom varía según la combinación de los tamaños del visor y la imagen, como se muestra en esta tabla:

| Tamaño de imagen | Tamaño de visor | Porcentaje de zoom |
|--- |--- |--- |
| Grande | Menor | Mínimo más pequeño |
| Pequeño | Mayor | Mínimo más grande |

Puede cambiar el tamaño del visor de zoom para que corresponda al que se usa en la página web. Para modificar este valor de forma definitiva, puede cambiar el tamaño del visor en la pantalla Ajustes (si es administrador). Consulte [Configuración de ajustes preestablecidos de visor de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creación y edición de destinos de zoom  {#creating-and-editing-zoom-targets}

Cree y edite destinos de zoom en la pantalla Editor de destinos de zoom. Para abrir esta pantalla, seleccione una imagen y realice una de las acciones siguientes:

* Haga clic en el botón **[!UICONTROL Edit]** y seleccione Destinos de zoom.
* En el panel Examinar, muestre la imagen en **[!UICONTROL Vista de detalles]** y haga clic en **[!UICONTROL Destinos de zoom]**.

En la pantalla Editor de destinos de zoom, haga clic en el botón **[!UICONTROL Seleccionar destino]** (flecha) para seleccionar un objetivo antes de cambiar su tamaño o posición. Haga clic en **[!UICONTROL Add Targets]** (rectángulo) para crear un objetivo de zoom en la imagen. La pantalla Editor de destinos de zoom también proporciona herramientas para eliminar, copiar y asignar nombre a los destinos de zoom.

### Creación de un destino de zoom  {#creating-a-zoom-target}

Abra la pantalla Editor de destinos de zoom y siga estos pasos para crear un destino de zoom:

1. Haga clic en **[!UICONTROL Add Targets]** (rectángulo), mueva el puntero sobre la imagen y haga clic donde desee que se muestre el objetivo de zoom.

   Aparece una imagen de miniatura del destino de zoom en el panel de la derecha de la pantalla.

1. Haga clic en **[!UICONTROL Seleccionar destino]** (flecha), haga clic en para seleccionar el objetivo de zoom que ha creado y ajuste el tamaño y la posición del objetivo.

   * ****
Cambiar tamañoMueva el puntero sobre una esquina del destino de zoom y arrástrelo para ampliar o reducir el destino.

   * ****
ColocaciónMueva el puntero sobre el destino de zoom y arrástrelo a una ubicación diferente.

1. Escriba un nombre para el destino de zoom en el cuadro Nombre. 

   >[!NOTE]
   >
   >lo que introduzca en el cuadro Nombre es mucho más que un nombre. Cuando los usuarios mueven el puntero por el destino de zoom, ven lo que se ha introducido en el cuadro Nombre. Introduzca una breve descripción del destino de zoom en el cuadro Nombre para que los usuarios sepan en qué pueden hacer zoom.

1. También puede introducir datos de usuario en el campo Datos de usuario. Este campo permite que los diseñadores de sitios web agreguen información en el destino de zoom.
1. Haga clic en **[!UICONTROL Guardar]**.

   Se guardarán las coordenadas y el nivel de zoom correspondientes al destino de zoom. A la derecha de la pantalla aparece una imagen de miniatura del destino de zoom con el nombre introducido.

>[!NOTE]
>
>Para ver el aspecto de los destinos de zoom en un visor de zoom, haga clic en el botón Vista previa en la pantalla Editor de destinos de zoom y seleccione un visor de zoom en la pantalla Vista previa. Para obtener más información sobre esta pantalla, consulte [Vista previa de imágenes con distintos visores de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Edición de destinos de zoom  {#editing-zoom-targets}

Utilice estas técnicas en la pantalla Editor de destinos de zoom para editar destinos de zoom:

* ****
Cambio de posiciónCon el botón Seleccionar destino (la flecha), haga clic en el destino para seleccionarlo. A continuación, arrastre el destino a otra ubicación.

* ****
Cambiar tamañoCon el botón Seleccionar destino (la flecha), haga clic en el destino para seleccionarlo. A continuación, mueva el puntero por la esquina del destino de zoom y arrastre para ampliar o reducir el destino.

* ****
EliminaciónHaga clic en la imagen en miniatura del destino en la parte derecha de la pantalla. A continuación, haga clic en **[!UICONTROL Eliminar destino]**.

* ****
Cambio de nombreHaga clic en la imagen en miniatura del destino en la parte derecha de la pantalla. A continuación, introduzca un nombre en el campo de texto **[!UICONTROL Name]** y haga clic en **[!UICONTROL Save]**.

### Copia de destinos de zoom {#copying-zoom-targets}

Puede copiar destinos de zoom de una imagen a otra. Copie los destinos cuando dos imágenes presenten un contenido similar y sus destinos de zoom pertenezcan a las mismas ubicaciones. Siga estos pasos para copiar los destinos de zoom a otra imagen:

1. Abra la imagen con los destinos de zoom que desea copiar en la pantalla Editor de destinos de zoom.
1. Haga clic en **[!UICONTROL Copiar destinos a]**.
1. En el cuadro de diálogo Seleccionar imágenes, seleccione una imagen y haga clic en **[!UICONTROL Seleccionar]**.

