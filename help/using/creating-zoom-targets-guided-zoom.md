---
title: Creación de destinos de zoom para el zoom guiado
description: Obtenga información sobre cómo crear destinos de zoom para el zoom guiado en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 27%

---

# Creación de destinos de zoom para el zoom guiado{#creating-zoom-targets-for-guided-zoom}

Los destinos de zoom guían a ciertas partes de una imagen. Además del zoom de forma libre, los visualizadores pueden seleccionar una miniatura de destino de zoom y hacer zoom en la parte de la imagen en la que desea que se centren. Los destinos de zoom permiten resaltar las partes atractivas o interesantes de una imagen.

![Crear destinos de zoom para el zoom guiado](/help/using/assets/zo_guided_zoom.png)

## Acerca de los destinos de zoom {#about-zoom-targets}

El porcentaje de zoom máximo de Destinos de zoom es 100 por ciento. El porcentaje mínimo de zoom varía según la combinación de los tamaños del visor y la imagen, como se muestra en esta tabla:

| Tamaño de imagen | Tamaño de visor | Porcentaje de zoom |
| --- | --- | --- |
| Grande | Menor | Mínimo más pequeño |
| Pequeño | Mayor | Mínimo más grande |

Puede cambiar el tamaño del Visor de zoom para que coincida con el tamaño que se está utilizando en la página Web. Puede cambiar esta configuración de forma permanente cambiando el tamaño del visor en la pantalla Configuración (si es administrador). Consulte [Configurar ajustes preestablecidos del visor de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creación y edición de destinos de zoom {#creating-and-editing-zoom-targets}

Cree y edite Destinos de zoom en la pantalla del Editor de destinos de zoom. Para abrir esta pantalla, seleccione una imagen y realice una de las acciones siguientes:

* Seleccione el botón de rollover **[!UICONTROL Editar]** y elija Destinos de zoom.
* En el panel Examinar, muestre la imagen en **[!UICONTROL Vista de detalles]** y, a continuación, seleccione **[!UICONTROL Destinos de zoom]**.

En la pantalla Editor de destinos de zoom, seleccione el botón **[!UICONTROL Seleccionar destino]** (flecha) para seleccionar un destino antes de cambiar su tamaño o posición. Para crear un destino de zoom en la imagen, seleccione **[!UICONTROL Agregar destinos]** (rectángulo). La página Editor de Destinos de Zoom también ofrece herramientas para eliminar, copiar y nombrar los destinos de zoom.

### Creación de un destino de zoom {#creating-a-zoom-target}

Para crear un destino de zoom, abra la página Editor de destinos de zoom y haga lo siguiente:

1. Seleccione **[!UICONTROL Agregar destinos]** (rectángulo), mueva el puntero sobre la imagen y seleccione dónde desea que esté el destino de zoom.

   Aparece una imagen de miniatura del destino de zoom en el panel de la derecha de la pantalla.

1. Elija **[!UICONTROL Seleccionar destino]** (flecha) y, a continuación, seleccione el destino de zoom que ha creado y ajuste el tamaño y la posición del destino.

   * **Cambiar tamaño**: mueva el puntero sobre una esquina del destino de zoom y arrástrelo para aumentar o reducir el destino.

   * **Posición**: mueva el puntero sobre el destino de zoom y arrástrelo a una ubicación diferente.

1. Escriba un nombre para el destino de zoom en el cuadro Nombre. 

   >[!NOTE]
   >
   >lo que introduzca en el cuadro Nombre es mucho más que un nombre. Cuando los usuarios mueven el puntero por el destino de zoom, ven lo que se ha introducido en el cuadro Nombre. Introduzca una breve descripción del destino de zoom en el cuadro Nombre para que los usuarios sepan en qué pueden hacer zoom.

1. También puede introducir datos de usuario en el campo Datos de usuario. Este campo es para que los diseñadores de sitios Web agreguen información al destino de zoom.
1. Seleccione **[!UICONTROL Guardar]**.

   Se guardarán las coordenadas y el nivel de zoom correspondientes al destino de zoom. A la derecha de la pantalla aparece una imagen de miniatura del destino de zoom con el nombre introducido.

>[!NOTE]
>
>Para ver el aspecto de los destinos de zoom en un visor de zoom, seleccione el botón **[!UICONTROL Vista previa]** en la pantalla Editor de destinos de zoom. A continuación, elija un Visor de zoom en la pantalla Vista previa. Para obtener más información sobre esta pantalla, consulte [Vista previa de imágenes con diferentes visores de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editar destinos de zoom {#editing-zoom-targets}

Para editar Destinos de zoom, utilice las técnicas siguientes en la página Editor de destinos de zoom:

* **Cambiar posición**: Con el botón Seleccionar destino (la flecha), seleccione el destino. A continuación, arrastre el destino a otra ubicación.

* **Cambiar tamaño**: con el botón Seleccionar destino (la flecha), seleccione el destino. Para aumentar o reducir el destino, mueva el puntero sobre una esquina del destino de zoom y arrastre.

* **Eliminar**: seleccione la imagen en miniatura de destino a la derecha de la pantalla. Luego selecciona **[!UICONTROL Eliminar destino]**.

* **Cambiando el nombre**: seleccione la imagen en miniatura de destino en el lado derecho de la pantalla. Luego escribe un nombre en el campo de texto **[!UICONTROL Nombre]** y selecciona **[!UICONTROL Guardar]**.

### Copiar destinos de zoom {#copying-zoom-targets}

Puede copiar destinos de zoom de una imagen a otra. Copie los destinos cuando dos imágenes presenten contenido similar y sus destinos de zoom pertenezcan a las mismas ubicaciones. Para copiar destinos de zoom en otra imagen, haga lo siguiente:

1. Abra la imagen con destinos de zoom que desee copiar en la pantalla Editor de destinos de zoom.
1. Seleccionar **[!UICONTROL Copiar Destinos A]**.
1. En el cuadro de diálogo Seleccionar imágenes, seleccione una imagen y elija **[!UICONTROL Seleccionar]**.
