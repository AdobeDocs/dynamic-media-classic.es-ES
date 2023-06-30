---
title: Previsualización de un recurso
description: Obtenga información sobre cómo previsualizar un recurso en Adobe Dynamic Media Classic.
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 36%

---

# Previsualización de un recurso{#previewing-an-asset}

Puede usar Vista previa para ver cómo aparece un recurso digital cuando lo ve un cliente. La Vista previa utiliza el visor predeterminado que tiene asignado el recurso. Los visores predeterminados se configuran en Ajustes de aplicación.

Consulte [Configuración de visores predeterminados](application-setup.md#configuring_default_viewers).

Si está previsualizando un recurso de plantilla con capas de parámetros, puede cambiar parámetros o el ajuste preestablecido de imagen. Debido a que los cambios se realizan en línea, los resultados pueden verse inmediatamente desde la propia ventana de vista previa.

Consulte también [Ejemplos de la biblioteca de referencia de visores de Adobe](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**Para obtener la vista previa de un recurso:**

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso cuya vista previa desea obtener.
1. Realice una de las acciones siguientes:

   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de cuadrícula]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de lista]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de detalles]**.

1. Según la vista que esté utilizando, realice una de las siguientes acciones:

   * En la ventana Recurso de la vista de cuadrícula o de la vista de lista, seleccione un único recurso y, a continuación, seleccione **[!UICONTROL Previsualizar]** cerca de la miniatura.
   * En la barra de herramientas situada encima de la ventana Activos de la vista de cuadrícula, vista de lista o vista de detalles, seleccione **[!UICONTROL Previsualizar]**.

## Previsualización de un recurso en función del tipo de plataforma del visor {#previewing-an-asset-based-on-viewer-platform-type}

Utilice la Lista del visor para previsualizar cómo se muestra un recurso en una plataforma de visor concreta como HTML5. Según el tipo de recurso y el visor asociado cuya vista previa haya seleccionado, no todas las plataformas se encuentran disponibles en Lista del visor.

También puede utilizar la Lista del visor para copiar la URL de un visor o para ver y copiar el código del visor para incorporarlo en sus páginas web.

En una plataforma de visor determinada, la ventana Lista de visores permite ver visualmente qué dispositivos, como tabletas y smartphones, están disponibles para utilizar.

**Para obtener la vista previa de un recurso en función del tipo de plataforma de visor:**

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso cuya vista previa desea obtener.
1. Realice una de las acciones siguientes:

   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de cuadrícula]**. En la ventana Recurso, seleccione un único recurso y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de lista]**. En la ventana Recurso, seleccione un único recurso y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista del visor]**.

1. (Opcional) En la ventana Lista de visores, seleccione el encabezado de la columna **[!UICONTROL Nombre]** o **[!UICONTROL Tipo de plataforma]** para ordenar la columna en orden ascendente o descendente.
1. En la ventana Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Previsualizar]** para ver cómo aparece el recurso para un visor seleccionado y el tipo de plataforma.

   Cerrar la vista previa mostrada.

1. (Opcional) En la ventana Lista del visor, en la lista desplegable inferior Codificación URL para la creación de copias URL, seleccione la codificación de URL que desee aplicar a la dirección URL del recurso cuando se copie.
1. (Opcional) Lleve a cabo uno de los procedimientos siguientes:

   * En la ventana Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Copiar URL]** para un visor y tipo de plataforma seleccionados.

     Al seleccionar **[!UICONTROL Copiar URL]**, su URL asociada se copia automáticamente en el portapapeles.

   * En la ventana Lista del visor, en la columna Acciones de la tabla, seleccione **[!UICONTROL Código incrustado]**.

     Al seleccionar **[!UICONTROL Código incrustado]**, se abrirá la ventana Código incrustado, donde podrá revisar el código del visor. El código no se puede editar en la ventana. También puede copiar el código en el portapapeles para pegarlo en sus páginas web.

     Cerrar la vista previa mostrada.

1. En la esquina inferior derecha de la ventana Lista de visualizadores, seleccione **[!UICONTROL Cerrar]** para volver a la pantalla Recursos.

## Previsualizar un recurso de imagen en función de su ajuste preestablecido de imagen {#previewing-an-image-asset-based-on-its-image-preset}

Puede previsualizar un recurso de imagen basándose en su ajuste preestablecido de imagen para ver el aspecto que tendrá la imagen al distribuirse dinámicamente y con distintos tamaños en su aplicación o sitio web.

Un ajuste preestablecido de imagen es una recopilación de ajustes predefinidos para cambiar el tamaño, la calidad de la imagen, el formato, la resolución y otros aspectos visuales de una imagen al exportarse.

Consulte [Configurar ajustes preestablecidos de imagen](setting-image-presets.md#setting_up_image_presets).

Consulte [Crear y habilitar ajustes preestablecidos de imagen](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**Para obtener la vista previa de un recurso de imagen en su ajuste preestablecido de imagen:**

1. En el panel Biblioteca de recursos del lado izquierdo, navegue a las carpetas de recursos que contienen el recurso de imagen cuya vista previa desea obtener.
1. Realice una de las acciones siguientes:

   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de cuadrícula]**. En la ventana Recurso, seleccione un único recurso de imagen y, debajo de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de lista]**. En la ventana Recurso, seleccione un único recurso de imagen y, a continuación, a la derecha de la imagen en miniatura, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.
   * Sobre la ventana Recursos, en la parte derecha de la barra de herramientas, seleccione **[!UICONTROL Vista de detalles]**. En la misma barra de herramientas, vaya a **[!UICONTROL Previsualizar]** > **[!UICONTROL Lista de ajustes preestablecidos de imagen]**.

1. En la tabla de la ventana Lista de ajustes preestablecidos de imagen, seleccione el nombre de un tipo de ajuste preestablecido cuyo recurso de imagen quiera previsualizar en línea en el panel derecho.
1. (Opcional) En la ventana Lista de ajustes preestablecidos de imagen, en el **[!UICONTROL Codificación URL para la generación de copias URL]** en la lista desplegable inferior, seleccione la codificación URL que se aplicará a la URL del recurso de imagen cuando se copie.
1. (Opcional) En la ventana Lista de ajustes preestablecidos de imagen, en el área superior derecha del panel de vista previa, seleccione **[!UICONTROL Copiar URL]** para el tipo de ajuste preestablecido seleccionado.

   Al seleccionar **[!UICONTROL Copiar URL]**, su URL asociada se copia automáticamente en el portapapeles.

1. En la esquina inferior derecha de la ventana Lista de ajustes preestablecidos de imagen, seleccione **[!UICONTROL Cerrar]** para volver a la pantalla Recursos.
