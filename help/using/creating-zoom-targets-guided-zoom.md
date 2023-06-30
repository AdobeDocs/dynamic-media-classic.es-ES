---
title: Creación de destinos de zoom para el zoom guiado
description: Aprenda a crear destinos de zoom para el zoom guiado en Adobe Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 41%

---

# Creación de destinos de zoom para el zoom guiado{#creating-zoom-targets-for-guided-zoom}

Los destinos de zoom guían a ciertas partes de una imagen. Además del zoom de forma libre, los visualizadores pueden seleccionar una miniatura de destino de zoom y hacer zoom en la parte de la imagen en la que desea que se centren. Los destinos de zoom permiten resaltar las partes atractivas o interesantes de una imagen.

![Creación de destinos de zoom para el zoom guiado](/help/using/assets/zo_guided_zoom.png)

## Acerca de los destinos de zoom {#about-zoom-targets}

El valor máximo de zoom en los destinos de zoom es 100%. El porcentaje mínimo de zoom varía según la combinación de los tamaños del visor y la imagen, como se muestra en esta tabla:

| Tamaño de imagen | Tamaño de visor | Porcentaje de zoom |
| --- | --- | --- |
| Grande | Menor | Mínimo más pequeño |
| Pequeño | Mayor | Mínimo más grande |

Puede cambiar el tamaño del visor de zoom para que corresponda al que se usa en la página web. Para modificar este valor de forma definitiva, puede cambiar el tamaño del visor en la pantalla Ajustes (si es administrador). Consulte [Configurar ajustes preestablecidos del visor de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creación y edición de destinos de zoom {#creating-and-editing-zoom-targets}

Cree y edite destinos de zoom en la pantalla Editor de destinos de zoom. Para abrir esta pantalla, seleccione una imagen y realice una de las acciones siguientes:

* Selección de la sustitución **[!UICONTROL Editar]** y seleccione Destinos de zoom.
* En el panel Examinar, muestre la imagen en **[!UICONTROL Vista de detalles]**, luego seleccione **[!UICONTROL Destinos de zoom]**.

En la pantalla Editor de destinos de zoom, seleccione **[!UICONTROL Seleccionar destino]** (flecha) para seleccionar un destino antes de cambiar su tamaño o posición. Para crear un objetivo de zoom en la imagen, seleccione **[!UICONTROL Añadir destinos]** (rectángulo). La página Editor de Destinos de Zoom también ofrece herramientas para eliminar, copiar y nombrar destinos de zoom.

### Creación de un destino de zoom {#creating-a-zoom-target}

Para crear un destino de zoom, abra la página Editor de destinos de zoom y haga lo siguiente:

1. Seleccionar **[!UICONTROL Añadir destinos]** (rectángulo), mueva el puntero sobre la imagen y seleccione dónde desea que esté el destino de zoom.

   Aparece una imagen de miniatura del destino de zoom en el panel de la derecha de la pantalla.

1. Seleccionar **[!UICONTROL Seleccionar destino]** (flecha) y, a continuación, seleccione el destino de zoom que ha creado y ajuste el tamaño y la posición del destino.

   * **Redimensionar** - Mueva el puntero sobre una esquina del destino de zoom y arrástrelo para agrandar o reducir el destino.

   * **Posición** - Mueva el puntero sobre el destino de zoom y arrástrelo a una ubicación diferente.

1. Escriba un nombre para el destino de zoom en el cuadro Nombre. 

   >[!NOTE]
   >
   >lo que introduzca en el cuadro Nombre es mucho más que un nombre. Cuando los usuarios mueven el puntero por el destino de zoom, ven lo que se ha introducido en el cuadro Nombre. Introduzca una breve descripción del destino de zoom en el cuadro Nombre para que los usuarios sepan en qué pueden hacer zoom.

1. También puede introducir datos de usuario en el campo Datos de usuario. Este campo permite que los diseñadores de sitios web agreguen información en el destino de zoom.
1. Seleccionar **[!UICONTROL Guardar]**.

   Se guardarán las coordenadas y el nivel de zoom correspondientes al destino de zoom. A la derecha de la pantalla aparece una imagen de miniatura del destino de zoom con el nombre introducido.

>[!NOTE]
>
>Para ver el aspecto de los destinos de zoom en un visor de zoom, seleccione la **[!UICONTROL Previsualizar]** en la pantalla Editor de destinos de zoom y elija un visor de zoom en la pantalla Vista previa. Para obtener más información sobre esta pantalla, consulte [Vista previa de imágenes con diferentes visores de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar destinos de zoom {#editing-zoom-targets}

Para editar destinos de zoom, utilice las técnicas siguientes en la página Editor de destinos de zoom:

* **Cambiar posición** : Con el botón Seleccionar destino (la flecha), seleccione el destino. A continuación, arrastre el destino a otra ubicación.

* **Redimensionar** : Con el botón Seleccionar destino (la flecha), seleccione el destino. Para aumentar o reducir el destino, mueva el puntero sobre una esquina del destino de zoom y arrastre.

* **Eliminar** - Seleccione la imagen en miniatura de destino en la parte derecha de la pantalla. A continuación seleccione **[!UICONTROL Eliminar destino]**.

* **Cambiando nombre** - Seleccione la imagen en miniatura de destino en la parte derecha de la pantalla. A continuación, introduzca un nombre en la **[!UICONTROL Nombre]** Campo de texto y seleccione **[!UICONTROL Guardar]**.

### Copiar destinos de zoom {#copying-zoom-targets}

Puede copiar destinos de zoom de una imagen a otra. Copie los destinos cuando dos imágenes presenten un contenido similar y sus destinos de zoom pertenezcan a las mismas ubicaciones. Para copiar destinos de zoom en otra imagen, haga lo siguiente:

1. Abra la imagen con destinos de zoom que desee copiar en la pantalla Editor de destinos de zoom.
1. Seleccionar **[!UICONTROL Copiar destinos en]**.
1. En el cuadro de diálogo Seleccionar imágenes, seleccione una imagen y elija **[!UICONTROL Seleccionar]**.
