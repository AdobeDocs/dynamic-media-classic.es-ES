---
title: Creación de destinos de zoom para zoom guiado
seo-title: Creación de destinos de zoom para zoom guiado
description: nulo
seo-description: Aprenda a crear destinos de zoom para zoom guiado.
uuid: 501 ea 37 b-adc 5-4290-87 eb -52 a 3501 e 5 d 26
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categorías/zoom
discoiquuid: e 7 b 4673 c -8681-4741-912 e -9 a 31 cf 106449
translation-type: tm+mt
source-git-commit: 2f99190eb0c346b87402e69c4067e94365042339

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

## Creación y edición de destinos de zoom {#creating-and-editing-zoom-targets}

Cree y edite destinos de zoom en la pantalla Editor de destinos de zoom. Para abrir esta pantalla, seleccione una imagen y realice una de las acciones siguientes:

* Click the rollover **Edit** button and choose Zoom Targets.
* In the Browse Panel, display the image in Detail view and click **Zoom Targets**.

On the Zoom Target Editor screen, click **Select Targe** t button (the arrow) to select a target before changing its size or position. Click **Add Targets** (the rectangle) to create a zoom target on the image. La pantalla Editor de destinos de zoom también proporciona herramientas para eliminar, copiar y asignar nombre a los destinos de zoom.

### Creación de un destino de zoom {#creating-a-zoom-target}

Abra la pantalla Editor de destinos de zoom y siga estos pasos para crear un destino de zoom:

1. Click **Add Targets** (the rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   Aparece una imagen de miniatura del destino de zoom en el panel de la derecha de la pantalla.

1. Click **Select Target** (the arrow), click to select the zoom target you created, and adjust the size and position of the target.

   **Cambiar tamaño** Mueva el puntero sobre una esquina del destino de zoom y arrastre para ampliar o reducir el destino.

   **Posicionar** mueve el puntero sobre el destino de zoom y arrástrelo a una ubicación diferente.

1. Escriba un nombre para el destino de zoom en el cuadro Nombre. 

   >[!NOTE]
   >
   >lo que introduzca en el cuadro Nombre es mucho más que un nombre. Cuando los usuarios mueven el puntero por el destino de zoom, ven lo que se ha introducido en el cuadro Nombre. Introduzca una breve descripción del destino de zoom en el cuadro Nombre para que los usuarios sepan en qué pueden hacer zoom.

1. También puede introducir datos de usuario en el campo Datos de usuario. Este campo permite que los diseñadores de sitios web agreguen información en el destino de zoom.
1. Haga clic en **Guardar**.

   Se guardarán las coordenadas y el nivel de zoom correspondientes al destino de zoom. A la derecha de la pantalla aparece una imagen de miniatura del destino de zoom con el nombre introducido.

>[!NOTE]
>
>Para ver el aspecto de los destinos de zoom en un visor de zoom, haga clic en el botón Vista previa en la pantalla Editor de destinos de zoom y seleccione un visor de zoom en la pantalla Vista previa. Para obtener más información sobre esta pantalla, consulte [Vista previa de imágenes con distintos visores de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Edición de destinos de zoom {#editing-zoom-targets}

Utilice estas técnicas en la pantalla Editor de destinos de zoom para editar destinos de zoom:

**Cambio de posición** con el botón Seleccionar destino (la flecha), haga clic en el destino para seleccionarlo. A continuación, arrastre el destino a otra ubicación.

**Cambio de tamaño** con el botón Seleccionar destino (la flecha), haga clic en el destino para seleccionarlo. A continuación, mueva el puntero por la esquina del destino de zoom y arrastre para ampliar o reducir el destino.

**Eliminación** de clic Haga clic en la imagen en miniatura del destino en el lado derecho de la pantalla. A continuación, haga clic en Eliminar destino.

**Cambio de nombre** Haga clic en la imagen en miniatura del destino en el lado derecho de la pantalla. A continuación, introduzca un nombre en el cuadro Nombre y haga clic en Guardar.

### Copia de destinos de zoom {#copying-zoom-targets}

Puede copiar destinos de zoom de una imagen a otra. Copie los destinos cuando dos imágenes presenten un contenido similar y sus destinos de zoom pertenezcan a las mismas ubicaciones. Siga estos pasos para copiar los destinos de zoom a otra imagen:

1. Abra la imagen con los destinos de zoom que desea copiar en la pantalla Editor de destinos de zoom.
1. Haga clic en **Copiar destinos a**.
1. In the Select Images dialog box, select an image and click **Select**.

