---
title: Trabajar en vista de detalles
description: Aprenda a trabajar en la Vista de detalles en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 20%

---

# Trabajar en vista de detalles{#working-in-detail-view}

Puede trabajar con un recurso y obtener más información sobre él abriéndolo en la Vista de detalles. En la Vista de detalles, verá el tamaño del recurso, los atributos, los derivados y los metadatos. También puede ver si el recurso se publicó y cuándo, y puede obtener la URL de los recursos publicados. Dependiendo del tipo de recurso, pueden ser viables diversas operaciones como, por ejemplo, visualización en distintos tamaños, aplicación de zoom, enfoque, recorte y otras operaciones de formato.

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![Vista de detalles](/help/using/assets/image_0.img.png)
*Vista de detalles con el panel Biblioteca de recursos oculto en la vista del lado izquierdo.*

>[!NOTE]
>
>Para abrir la carpeta en la que está almacenado el recurso, puede seleccionar la ruta de la carpeta en la parte superior del panel Información.

## Abrir un recurso en la Vista de detalles {#open-an-asset-in-detail-view}

Puede mostrar un recurso en la Vista de detalles para que pueda examinarlo, previsualizarlo o trabajar en él de cerca.

1. En el panel Examinar, realice una de las acciones siguientes:

   * Seleccione el recurso. Cerca de la esquina superior derecha de Adobe Dynamic Media Classic, seleccione el icono **[!UICONTROL Vista de detalles]**.
   * Haga doble clic en el recurso.
   * Seleccione el recurso y, a continuación, vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Detalles]**.

>[!NOTE]
>
>Puede pasar de un recurso a otro en la misma carpeta en la Vista de detalles. Simplemente haga clic en **[!UICONTROL Recurso anterior]** o en **[!UICONTROL Recurso siguiente]**. Estos botones se encuentran en la esquina superior derecha de la Vista de detalles.

## Obtener información en la Vista de detalles {#getting-information-in-detail-view}

La Vista de detalles proporciona información sobre un recurso o un archivo. Esta información se muestra sobre un elemento: la carpeta donde se almacena, su nombre de archivo, la fecha en que se cargó el elemento en Adobe Dynamic Media Classic y su historial de publicación. También puede ver y editar metadatos y agregar palabras clave para un recurso en la Vista de detalles.

Puede obtener una URL de recurso en la Vista de detalles; sin embargo, la URL no estará activa hasta que publique el recurso. En el caso de las imágenes, la vista de detalles también proporciona una lista de recursos y metadatos creados y derivados, como destinos de zoom y conjuntos de imágenes.

## Trabajo con recursos en la Vista de detalles {#working-with-assets-in-detail-view}

La Vista de detalles ofrece herramientas para trabajar con el recurso que ha abierto. Las herramientas disponibles dependen del tipo de recurso con el que trabaje, pero la Vista de detalles siempre ofrece estas funciones:

* **elementos para la publicación**: seleccione el icono **[!UICONTROL `Publish`]** a la izquierda del nombre o vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Publish]** o **[!UICONTROL Archivo]** > **[!UICONTROL Cancelar la publicación]**.

* **Cambiar el nombre del recurso**: seleccione el nombre e introduzca uno nuevo.

* **Editar y agregar metadatos**: seleccione el panel Metadatos y cámbielo como desee. Ver [Ver, agregar y exportar metadatos](/help/using/viewing-adding-exporting-metadata.md).

* **Editar y agregar palabras clave**: seleccione Palabras clave y agréguelas o quítelas como desee. Consulte [Adición o edición de palabras clave](/help/using/viewing-adding-exporting-metadata.md).

* **Eliminar el recurso**: Vaya a **[!UICONTROL Archivo]** > **[!UICONTROL Eliminar]**.

Para archivos discretos (imágenes, conjuntos de imágenes y fuentes, por ejemplo) puede ver el historial de publicación y edición y comprobar los detalles del trabajo en la Vista de detalles.

Esta tabla muestra qué otras opciones están disponibles con diferentes tipos de recursos en la Vista de detalles.

| Tipo de recurso | Edición/Ajustes | Vista previa |
| --- | --- | --- |
| Imágenes | Agregar mapas de imagen<br>Agregar destinos de zoom<br>Recortar<br>Enfoque<br>Crear vistas ajustadas | Sí; ajustes preestablecidos de zoom e imagen |
| Imágenes de cobertura de ventana y armario | No | Miniatura |
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
| Archivos ZIP | No | No se muestra el contenido |

>[!MORELIKETHIS]
>
>* [Ver, agregar y exportar metadatos](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
