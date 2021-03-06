---
title: Crear destinos de zoom para zoom guiado
description: Aprenda a crear destinos de zoom para la zoom guiada en Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 44%

---

# Crear destinos de zoom para zoom guiado{#creating-zoom-targets-for-guided-zoom}

Los destinos de zoom guían a ciertas partes de una imagen. Además del zoom de forma libre, los espectadores pueden seleccionar una miniatura de destino de zoom y hacer zoom en la parte de la imagen en la que desea que se centren. Los destinos de zoom permiten resaltar las partes atractivas o interesantes de una imagen.

![Crear destinos de zoom para zoom guiado](/help/assets/zo_guided_zoom.png)

## Acerca de los destinos de zoom {#about-zoom-targets}

El valor máximo de zoom en los destinos de zoom es 100%. El porcentaje mínimo de zoom varía según la combinación de los tamaños del visor y la imagen, como se muestra en esta tabla:

| Tamaño de imagen | Tamaño de visor | Porcentaje de zoom |
| --- | --- | --- |
| Grande | Menor | Mínimo más pequeño |
| Pequeño | Mayor | Mínimo más grande |

Puede cambiar el tamaño del visor de zoom para que corresponda al que se usa en la página web. Para modificar este valor de forma definitiva, puede cambiar el tamaño del visor en la pantalla Ajustes (si es administrador). Consulte [Configurar ajustes preestablecidos de visor de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Crear y editar destinos de zoom {#creating-and-editing-zoom-targets}

Cree y edite destinos de zoom en la pantalla Editor de destinos de zoom. Para abrir esta pantalla, seleccione una imagen y realice una de las acciones siguientes:

* Seleccione el botón de rollover **[!UICONTROL Edit]** y elija Destinos de zoom.
* En el panel Examinar, muestre la imagen en **[!UICONTROL Vista de detalles]** y, a continuación, seleccione **[!UICONTROL Destinos de zoom]**.

En la pantalla Editor de destinos de zoom, seleccione el botón **[!UICONTROL Select Target]** (flecha) para seleccionar un objetivo antes de cambiar su tamaño o posición. Para crear un objetivo de zoom en la imagen, seleccione **[!UICONTROL Add Targets]** (rectángulo). La página Editor de destinos de zoom también ofrece herramientas para eliminar, copiar y dar nombre a los destinos de zoom.

### Creación de un objetivo de zoom {#creating-a-zoom-target}

Para crear un objetivo de zoom, abra la página Editor de destinos de zoom y haga lo siguiente:

1. Seleccione **[!UICONTROL Add Targets]** (rectángulo), mueva el puntero sobre la imagen y seleccione dónde desea que esté el objetivo de zoom.

   Aparece una imagen de miniatura del destino de zoom en el panel de la derecha de la pantalla.

1. Elija **[!UICONTROL Seleccione Target]** (flecha) y, a continuación, seleccione el objetivo de zoom que ha creado y ajuste el tamaño y la posición del objetivo.

   * **Cambiar tamaño** : mueva el puntero sobre una esquina del destino de zoom y arrástrelo para ampliar o reducir el destino.

   * **Posición** : mueva el puntero sobre el destino de zoom y arrástrelo a una ubicación diferente.

1. Escriba un nombre para el destino de zoom en el cuadro Nombre. 

   >[!NOTE]
   >
   >lo que introduzca en el cuadro Nombre es mucho más que un nombre. Cuando los usuarios mueven el puntero por el destino de zoom, ven lo que se ha introducido en el cuadro Nombre. Introduzca una breve descripción del destino de zoom en el cuadro Nombre para que los usuarios sepan en qué pueden hacer zoom.

1. También puede introducir datos de usuario en el campo Datos de usuario. Este campo permite que los diseñadores de sitios web agreguen información en el destino de zoom.
1. Seleccione **[!UICONTROL Guardar]**.

   Se guardarán las coordenadas y el nivel de zoom correspondientes al destino de zoom. A la derecha de la pantalla aparece una imagen de miniatura del destino de zoom con el nombre introducido.

>[!NOTE]
>
>Para ver el aspecto de los destinos de zoom en un visor de zoom, seleccione el botón **[!UICONTROL Preview]** en la pantalla Editor de destinos de zoom y elija un visor de zoom en la pantalla Vista previa. Para obtener información sobre esta pantalla, consulte [Vista previa de imágenes con diferentes visores de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar destinos de zoom {#editing-zoom-targets}

Para editar destinos de zoom, utilice las siguientes técnicas en la página Editor de destinos de zoom :

* **Cambiar posición** : con el botón Seleccionar destino (la flecha), seleccione el destino. A continuación, arrastre el destino a otra ubicación.

* **Cambiar tamaño** : con el botón Seleccionar destino (la flecha), seleccione el destino. Para ampliar o reducir el destino, mueva el puntero sobre una esquina del destino de zoom y arrastre.

* **Eliminar** : seleccione la imagen en miniatura del destino en el lado derecho de la pantalla. A continuación, seleccione **[!UICONTROL Eliminar destino]**.

* **Cambio de nombre** : seleccione la imagen en miniatura del destino en el lado derecho de la pantalla. A continuación, introduzca un nombre en el campo de texto **[!UICONTROL Name]** y seleccione **[!UICONTROL Save]**.

### Copiar destinos de zoom {#copying-zoom-targets}

Puede copiar destinos de zoom de una imagen a otra. Copie los destinos cuando dos imágenes presenten un contenido similar y sus destinos de zoom pertenezcan a las mismas ubicaciones. Para copiar destinos de zoom en otra imagen, haga lo siguiente:

1. Abra la imagen con los destinos de zoom que desea copiar en la pantalla Editor de destinos de zoom.
1. Seleccione **[!UICONTROL Copiar destinos a]**.
1. En el cuadro de diálogo Seleccionar imágenes, seleccione una imagen y elija **[!UICONTROL Seleccionar]**.
