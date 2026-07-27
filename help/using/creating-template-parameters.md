---
title: Crear parámetros de plantilla
description: Obtenga información sobre cómo crear parámetros de plantilla en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
autotag-review: '2026-05-13T18:18:48.978Z'
TQID: 'https://experienceleague.adobe.com/OER2DJaRg4M20aJ1hlimXCf-yAqBrr27un4ZCPov4GA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 6e5910c1120d980bd60343c7e6feb76bbd8e289a
workflow-type: tm+mt
source-wordcount: 829
ht-degree: 29%

---

# Creación de los parámetros de plantilla{#creating-template-parameters}

Los parámetros permiten utilizar plantillas con la máxima flexibilidad; permiten personalizar dinámicamente una imagen de plantilla. Puede decidir cuál de las capas de imagen y texto desea incluir en la plantilla, y en cada capa, qué parámetros desea mostrar. Por ejemplo, para resaltar un producto que está a la venta, puede crear una capa de texto En venta. Posteriormente podrá quitar el parámetro Rebajado para quitar esta capa manteniendo el resto de la imagen de plantilla.

Cuando cree parámetros de plantilla, declare a qué partes de la plantilla llamar en una cadena URL. Una URL compuesta de parámetros revela esos elementos en la cadena URL. Con los parámetros expuestos, puede crear resultados personalizados de la manera en que la plantilla de la imagen se construye de forma dinámica en el servidor de imágenes. Así se puede cambiar una plantilla de forma dinámica ya que se puede llamar a todos los parámetros o solo algunos de una URL.

Con parámetros de capa de texto, la cadena de texto también puede ser un campo dinámico vinculado a valores en una base de datos. La vinculación de texto a una base de datos puede ser útil en casos como las promociones, por ejemplo. Para que las imágenes de plantilla muestren nombres de clientes o clientes, puede personalizarlas. Para mostrar el precio de un artículo en una imagen de plantilla, también puede vincular un parámetro de capa de texto a una base de datos de precios.

Puede hacer referencia a un parámetro más de una vez. Use el cuadro combinado de cada comando del cuadro de diálogo de parámetros para seleccionar cualquier parámetro que coincida con el comando en cuestión. Por ejemplo, todos los parámetros de tamaño están disponibles para el comando `size=`. Puede reasignar la referencia de parámetro a cualquier parámetro que ya se encuentre en el cuadro combinado y cambiarle el nombre por otro que no esté en el cuadro combinado. En este último caso, el nombre debe ser único. De lo contrario, un error indica que el parámetro existe. Al eliminar una referencia de parámetro, este se elimina de la dirección URL si no se hace referencia a él en ningún otro sitio. Al cambiar el valor predeterminado de un parámetro de texto, se actualizan todas las referencias a dicho parámetro. Puede ver la actualización en la tabla de capas, la renderización de la plantilla y la dirección URL. Cuando se cambia un atributo de capa manipulando los controles de cambio de tamaño o escribiendo valores en el panel de propiedades, el valor del parámetro se actualiza y todas las referencias al parámetro se actualizan. Por ejemplo, si se ha parametrizado el tamaño de dos capas mediante un parámetro, ambos tamaños de capa se actualizarán cuando se cambie alguno de los tamaños de capa. Si obtiene la vista previa de una plantilla y modifica un parámetro, se actualizan todas las referencias a dicho parámetro.

Vea también [Fundamentos de la plantilla](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vídeo de formación.

## Parametrizar una capa {#parameterizing-a-layer}

Para crear parámetros de plantilla para cada capa de la plantilla, siga estos pasos:

1. En la lista Capas (Layers), seleccione el botón Parámetros (Parameters) situado junto al nombre de la capa para la que desea crear parámetros. Se abre la pantalla Parámetros. Enumera el nombre de cada parámetro en la capa, su valor y su tipo.
1. Seleccione la opción Activado junto al nombre de cada parámetro que desee incluir en la imagen de plantilla.
1. Seleccione **[!UICONTROL Cerrar]** para salir de la pantalla Parámetros.

>[!NOTE]
>
>En la pantalla Parámetros puede cambiar el nombre de éstos. El cambio de nombre de un parámetro puede hacerlo más fácil de identificar en cadenas URL y más fácil de usar como valor de base de datos. Para cambiar el nombre de un parámetro, seleccione su opción **[!UICONTROL Activado]**, seleccione su nombre e introduzca un nuevo nombre en el campo Nombre.

Para ver una lista de los parámetros que ha creado para la plantilla, seleccione el botón Resumen de parámetros en la pantalla Plantilla. En la pantalla Resumen de parámetros, se muestra el nombre de cada capa y, si se han creado parámetros para una capa, se muestran los nombres y valores de los parámetros.

## Crear parámetros de texto dinámico {#creating-dynamic-text-parameters}

Para las capas de texto, también puede hacer que la cadena de texto sea un campo dinámico vinculado a un valor de base de datos. Siga estos pasos:

1. En la pantalla Plantilla, seleccione el botón Parámetros junto al nombre de la capa de texto para la que desea crear parámetros de texto dinámico. Se abre la página Parámetros.
1. Seleccione la opción **[!UICONTROL Activado]** junto al nombre del atributo de texto (textAttr).
1. Seleccione la ficha **[!UICONTROL Texto]** en la pantalla Parámetros.
1. Seleccione **[!UICONTROL Agregar parámetro]**. Aparecerá un nombre de parámetro predeterminado. Puede reemplazar este nombre seleccionándolo e introduciendo un nombre nuevo. La cadena de texto actual se convierte en el nuevo nombre del parámetro.
1. Seleccione **[!UICONTROL Cerrar]** para cerrar la página Parámetros.

Para que el nombre del parámetro use un valor de base de datos, añada la siguiente cadena al final de la URL de la plantilla:

```as3
?$_2(parameter name)=(database value)
```

Los nombres de un campo de base de datos o código Java™ reemplazan los nombres de parámetros. Esta funcionalidad indica, por ejemplo, el precio actual de un artículo o el nombre de un cliente.
