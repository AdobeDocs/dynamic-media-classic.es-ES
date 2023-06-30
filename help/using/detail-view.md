---
title: Trabajar en vista de detalles
description: Aprenda a trabajar en la Vista de detalles en Adobe Dynamic Media Classic.
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 21%

---

# Trabajar en vista de detalles{#working-in-detail-view}

Puede trabajar con un recurso y obtener más información sobre él abriéndolo en la Vista de detalles. En la Vista de detalles, verá el tamaño del recurso, los atributos, los derivados y los metadatos. También verá si el recurso se publicó y cuándo, y podrá obtener la URL de los recursos publicados. Dependiendo del tipo de recurso, pueden ser viables diversas operaciones como, por ejemplo, visualización en distintos tamaños, aplicación de zoom, enfoque, recorte y otras operaciones de formato.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Vista de detalles](/help/using/assets/image_0.img.png)
*Vista de detalles con el panel Biblioteca de recursos oculto de la vista en el lado izquierdo.*

>[!NOTE]
>
>Para abrir la carpeta en la que está almacenado el recurso, puede seleccionar la ruta de la carpeta en la parte superior del panel Información.

## Abrir un recurso en la Vista de detalles {#open-an-asset-in-detail-view}

Para examinar, previsualizar o trabajar de cerca en un recurso, puede mostrarlo en la Vista de detalles.

1. En el panel Examinar, realice una de las acciones siguientes:

   * Seleccione el recurso. Cerca de la esquina superior derecha de Adobe Dynamic Media Classic, seleccione la opción **[!UICONTROL Vista de detalles]** icono .
   * Haga doble clic en el recurso.
   * Seleccione el recurso y vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Detalles]**.

>[!NOTE]
>
>Puede pasar de un recurso a otro en la misma carpeta en la Vista de detalles seleccionando **[!UICONTROL Recurso anterior]** o **[!UICONTROL Siguiente recurso]**. Estos botones se encuentran en la esquina superior derecha de la Vista de detalles.

## Obtener información en la Vista de detalles {#getting-information-in-detail-view}

La Vista de detalles proporciona información sobre un recurso o un archivo. Muestra esta información sobre un elemento: la carpeta donde se almacena, su nombre de archivo, la fecha en que se cargó el elemento en Adobe Dynamic Media Classic y su historial de publicación. También puede ver y editar metadatos y agregar palabras clave para un recurso en la Vista de detalles.

Puede obtener una URL de recurso en la Vista de detalles; sin embargo, la URL no estará activa hasta que publique el recurso. En el caso de las imágenes, la vista de detalles también proporciona una lista de recursos y metadatos de compilación y derivados, como destinos de zoom y conjuntos de imágenes.

## Trabajo con recursos en la Vista de detalles {#working-with-assets-in-detail-view}

La Vista de detalles ofrece herramientas para trabajar con el recurso que ha abierto. Las herramientas disponibles dependen del tipo de recurso con el que trabaje, pero la Vista de detalles siempre ofrece estas funciones:

* **elementos para publicar** - Seleccione el **[!UICONTROL Publish]** a la izquierda del nombre o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Publish]** o **[!UICONTROL Archivo]** > **[!UICONTROL Cancelar publicación]**.

* **Cambiar el nombre del recurso** - Seleccione el nombre e introduzca uno nuevo.

* **Edición y adición de metadatos** : seleccione el panel Metadatos y cámbielo como desee. Consulte [Visualización, adición y exportación de metadatos](/help/using/viewing-adding-exporting-metadata.md).

* **Editar y añadir palabras clave** - Seleccione Palabras clave y añádalas o elimínelas como desee. Consulte [Adición o edición de palabras clave](/help/using/viewing-adding-exporting-metadata.md).

* **Eliminar el recurso** - Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]**.

Para archivos discretos (imágenes, conjuntos de imágenes y fuentes, por ejemplo) puede ver el historial de publicación y edición y comprobar los detalles del trabajo en la Vista de detalles.

Esta tabla muestra qué otras opciones están disponibles con diferentes tipos de recursos en la Vista de detalles.

| Tipo de recurso | Edición/Ajustes | Vista previa |
| --- | --- | --- |
| Imágenes | Agregar mapas de imagen<br>Añadir destinos de zoom<br>Recorte<br>Enfoque<br>Creación de vistas ajustadas | Sí; ajustes preestablecidos de zoom e imagen |
| Imágenes de armario y ventanas | No | Miniatura |
| Catálogos electrónicos | Editar | Sí<br>El panel de información también está disponible |
| Fuentes | Editar información de fuente | No |
| Archivos FXG | Editar | Sí |
| Perfiles ICC | Editar información de perfil | No |
| Archivos de Illustrator | No (a menos que se convierta a FXG) | No |
| Conjuntos de imágenes | Editar | Sí |
| Archivos de InDesign | No (a menos que se convierta a FXG) | No |
| Archivos PDF | No | No |
| Archivos PSD | Sí, para capas individuales | Sí, para capas individuales |
| Conjuntos de giros | Editar | Sí |
| Archivos SVG | No | No |
| Plantillas | Editar | Sí |
| Vídeos | No | Sí |
| Viñetas y viñetas procesadas | No | Se muestra la imagen<br>Puede ver el contenido y la estructura de los elementos procesables de la viñeta en formato XML |
| Archivos XML | No | Se muestra el contenido |
| Archivos ZIP | No | El contenido no se muestra |

>[!MORELIKETHIS]
>
>* [Visualización, adición y exportación de metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
