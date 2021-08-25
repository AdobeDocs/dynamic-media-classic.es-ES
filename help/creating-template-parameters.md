---
title: Creación de los parámetros de plantilla
description: Obtenga información sobre cómo crear parámetros de plantilla en Dynamic Media Classic.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: 976f739e5233ae9da24b06cffa729353a7d03c46
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 64%

---

# Creación de los parámetros de plantilla{#creating-template-parameters}

Los parámetros le permiten usar las plantillas con la máxima flexibilidad; puede personalizar de forma dinámica una plantilla de imagen. Puede decidir cuál de las capas de imagen y texto desea incluir en la plantilla, y en cada capa, qué parámetros desea mostrar. Por ejemplo, para llamar la atención sobre un producto que está en venta, puede crear una capa de texto En venta . Posteriormente podrá quitar el parámetro Rebajado para quitar esta capa manteniendo el resto de la imagen de plantilla.

La creación de parámetros de plantilla implica la definición de las partes de la plantilla a las que llamar en una cadena URL. Una URL compuesta de parámetros revela esos elementos en la cadena URL. Con los parámetros expuestos, puede crear resultados personalizados de la manera en que la plantilla de la imagen se construye de forma dinámica en el servidor de imágenes. Así se puede cambiar una plantilla de forma dinámica ya que se puede llamar a todos los parámetros o solo algunos de una URL.

Con parámetros de capa de texto, la cadena de texto también puede ser un campo dinámico vinculado a valores en una base de datos. La vinculación de texto a una base de datos puede ser útil en casos como las promociones, por ejemplo. Puede personalizar imágenes de plantilla para que muestren nombres de clientes. También puede vincular un parámetro de capa de texto a una base de datos de precios para mostrar el precio de un elemento en una imagen de plantilla.

Puede hacer referencia a un parámetro más de una vez. Use el cuadro combinado de cada comando del cuadro de diálogo de parámetros para seleccionar cualquier parámetro que coincida con el comando en cuestión. Por ejemplo, todos los parámetros de tamaño están disponibles para el comando `size=`. Puede reasignar la referencia de parámetro a cualquier parámetro que ya esté en el cuadro combinado y cambiar su nombre por otro que no aparezca. En este último caso, el nombre debe ser único. De lo contrario, se muestra un error que indica que el parámetro existe. Al eliminar una referencia de parámetro, este se elimina de la dirección URL si no se hace referencia a él en ninguna otra parte. Cuando se cambia el valor predeterminado de un parámetro de texto, todas las referencias a ese parámetro se actualizan. Puede ver la actualización en la tabla de capas, en la renderización de la plantilla y en la dirección URL. Cuando se cambia un atributo de capa manipulando los controladores de cambio de tamaño o escribiendo valores en el panel de propiedad, el valor del parámetro se actualiza y todas las referencias al parámetro se actualizan. Por ejemplo, si ha parametrizado el tamaño de dos capas con un solo parámetro, se actualiza el tamaño de ambas capas al cambiar cualquiera de ellas. Si obtiene la vista previa de una plantilla y modifica un parámetro, se actualizan todas las referencias a dicho parámetro.

## Parametrizar una capa {#parameterizing-a-layer}

Siga estos pasos con cada capa de la plantilla para crear parámetros de plantilla:

1. En la lista de capas, seleccione el botón Parámetros  situado junto al nombre de la capa para la que quiere crear parámetros. Se abre la pantalla Parámetros. Aquí aparecen los nombres de cada parámetro existente en la capa, con sus valores y sus tipos.
1. Seleccione la opción Activado de cada parámetro que quiera incluir en la imagen de plantilla.
1. Seleccione **[!UICONTROL Cerrar]** para salir de la pantalla Parámetros.

>[!NOTE]
>
>En la pantalla Parámetros puede cambiar el nombre de éstos. El cambio de nombre de un parámetro puede hacerlo más fácil de identificar en cadenas URL y más fácil de usar como valor de base de datos. Para cambiar el nombre de un parámetro, seleccione su opción **[!UICONTROL On]**, seleccione su nombre e introduzca un nuevo nombre en el campo Nombre.

Para ver una lista de los parámetros que ha creado para la plantilla, seleccione el botón Resumen de parámetros en la pantalla Plantilla. Aparecerá la pantalla Resumen de parámetros. Aquí aparecen los nombres de las capas y, si ha creado parámetros para alguna de ellas, los nombres y valores de los parámetros.

## Crear parámetros de texto dinámico {#creating-dynamic-text-parameters}

Para las capas de texto, también puede convertir la cadena de texto en un campo dinámico vinculado a un valor de base de datos. Siga estos pasos:

1. En la pantalla Plantilla, seleccione el botón Parámetros  situado junto al nombre de la capa de texto para la que quiere crear parámetros de texto dinámico. Se abre la página Parámetros.
1. Seleccione la opción **[!UICONTROL On]** junto al nombre del atributo text (textAttr).
1. Seleccione la pestaña **[!UICONTROL Text]** en la pantalla Parameters .
1. Seleccione **[!UICONTROL Agregar parámetro]**. Aparecerá un nombre de parámetro predeterminado. Si quiere modificar el nombre, selecciónelo y sobrescríbalo. La cadena de texto actual se convierte en el nuevo nombre del parámetro.
1. Seleccione **[!UICONTROL Cerrar]** para cerrar la página Parámetros.

Para que el nombre del parámetro use un valor de base de datos, añada la siguiente cadena al final de la URL de la plantilla:

```as3
?$_2(parameter name)=(database value)
```

El nombre del parámetro se sustituye por nombres en un campo de base de datos o código Java™ que indican, por ejemplo, el precio actual de un artículo o un nombre de cliente.
