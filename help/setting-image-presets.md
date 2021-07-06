---
title: Configuración de ajustes preestablecidos de imagen
description: Aprenda a configurar ajustes preestablecidos de imagen.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Ajustes preestablecidos de imagen
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 64%

---

# Configuración de ajustes preestablecidos de imagen{#setting-up-image-presets}

Un ajuste preestablecido de imagen, que se guarda con un nombre exclusivo, es similar a una macro y se compone de una serie de comandos de formato y tamaño predefinidos. Para entender cómo se usan los ajustes preestablecidos de imagen, supongamos que su sitio web requiere que la imagen de cada producto aparezca en dos tamaños distintos: 500 x 500 píxeles y 150 x 150 píxeles. Así pues, crea dos ajustes preestablecidos de imagen, uno denominado “Ampliación” para mostrar imágenes de 500 x 500 píxeles y otro denominado “Miniatura” para mostrar imágenes de 150 x 150 píxeles. Para enviar imágenes con los tamaños &quot;Ampliar&quot; y &quot;Miniatura&quot;, un servidor de imágenes de Dynamic Media busca en la definición del ajuste preestablecido de imagen ampliable y el ajuste preestablecido de imagen en miniatura. El servidor generará dinámicamente una imagen con las especificaciones de tamaño y formato de cada ajuste preestablecido de imagen.

Dynamic Media Classic incluye varios ajustes preestablecidos de imagen &quot;recomendados&quot; que ya están configurados para su uso. Los administradores también pueden crear nuevos ajustes preestablecidos de imagen. Para crear un nuevo ajuste preestablecido, puede empezar desde cero o tomar uno existente como punto de partida y guardarlo con un nombre nuevo.

Téngase en cuenta que las imágenes de tamaño reducido pueden sufrir pérdidas de enfoque y detalles al distribuirse dinámicamente desde un servidor. Por esta razón, cada ajuste preestablecido de imagen contiene controles de formato para optimizar una imagen cuando se distribuye con un tamaño concreto. Estos controles garantizan la nitidez de las imágenes al llegar al sitio web o la aplicación de destino.

## Creación de un ajuste preestablecido de imagen {#creating-an-image-preset}

Los administradores pueden crear ajustes preestablecidos de imagen. Puede crear nuevos ajustes preestablecidos de imagen o empezar con un ajuste preestablecido de imagen predeterminado que proporciona Dynamic Media Classic, editarlo y guardarlo con un nuevo nombre.

**Para crear un ajuste preestablecido de imagen:**

1. Haga clic en **Ajustes** > **Ajustes preestablecidos de imagen**.

   Puede buscar el nombre de uno de ellos aquí para obtener una vista previa. Al seleccionar el nombre de un ajuste preestablecido, cambia el tamaño y el aspecto de la imagen de muestra en la ventana Vista previa.

1. Realice una de las siguientes acciones:

   * **Creación de un**
ajuste preestablecido de imagenHaga clic en Agregar.

   * **Edición de un**
ajuste preestablecido de imagenBusque el ajuste preestablecido de imagen que se asemeje más al que desea crear y, a continuación, haga clic en Editar.

1. Asigne un nombre al ajuste.
1. Indique los valores de altura y anchura en píxeles. Estas medidas determinan el tamaño en que se distribuirán las imágenes.
1. Introduzca los datos requeridos en la pantalla Agregar ajuste preestablecido o Editar ajuste preestablecido. Para obtener más información, consulte [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options).

   Dynamic Media Classic recomienda estas opciones de &quot;prácticas recomendadas&quot; para comenzar:

   * ****
FormatoElija JPEG u otro formato que cumpla sus necesidades. Todos los navegadores web admiten el formato de imagen JPEG; ofrece un buen equilibrio entre los tamaños de archivos pequeños y la calidad de imagen. Sin embargo, las imágenes en formato JPEG utilizan un esquema de compresión con pérdidas que puede introducir artefactos de imagen no deseados si el ajuste de compresión es demasiado bajo. Por este motivo, Dynamic Media Classic recomienda establecer la calidad de compresión (en el control deslizante) en 75. Este ajuste ofrece un buen equilibrio entre la calidad de imagen y el tamaño de archivo pequeño.

   * ****
EnfoqueNo seleccione Enfoque (este filtro de enfoque ofrece menos control que la configuración de Enmascaramiento de enfoque).

   * **Volver a muestrear**
ModoElegir bicúbico.

   * **Opciones de máscara de enfoque (USM)**
Introduzca la configuración que se muestra aquí:
   | Tipo de ajuste preestablecido | Tamaño | Máscara: Cantidad | Máscara: Radio | Máscara: Umbral |
   |--- |--- |--- |--- |--- |
   | Venta cruzada (miniatura mini) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principal | 350 x 350 | 3 | 3 | 6 |
   | Ampliación | 500 x 500 | 1,2 | 1,2 | 5 |

1. Haga clic en **Guardar**.

Las opciones de &quot;prácticas recomendadas&quot; de Dynamic Media Classic para crear ajustes preestablecidos de imagen que se enumeran a continuación son recomendaciones generales; el enfoque es altamente subjetivo. Las “prácticas recomendadas” se basan en una imagen principal de 2000 x 2000. Las opciones deseables para imágenes mayores o menores pueden ser diferentes. Si desea ajustar la configuración de máscara de enfoque, Dynamic Media Classic recomienda estos intervalos:

* ****
AmountEntre 0,8 y 1,5.

* ****
RadioEntre .6 y 2.

* ****
Umbral: de 1 a 6.

Para eliminar un ajuste preestablecido de imagen, selecciónelo en la pantalla Ajustes preestablecidos de imagen y seleccione el botón Eliminar.

>[!MORELIKETHIS]
>
>* [Creación y edición de ajustes preestablecidos de imagen](application-setup.md#creating_and_editing_image_presets)
* [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options)
* [Vista previa de un recurso de imagen en su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

