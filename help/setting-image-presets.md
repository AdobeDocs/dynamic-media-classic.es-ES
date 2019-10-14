---
title: Configuración de ajustes preestablecidos de imagen
seo-title: Configuración de ajustes preestablecidos de imagen
description: nulo
seo-description: Obtenga información sobre cómo configurar ajustes preestablecidos de imagen.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_size
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Configuración de ajustes preestablecidos de imagen{#setting-up-image-presets}

Un ajuste preestablecido de imagen, que se guarda con un nombre exclusivo, es similar a una macro y se compone de una serie de comandos de formato y tamaño predefinidos. Para entender cómo se usan los ajustes preestablecidos de imagen, supongamos que su sitio web requiere que la imagen de cada producto aparezca en dos tamaños distintos: 500 x 500 píxeles y 150 x 150 píxeles. Así pues, crea dos ajustes preestablecidos de imagen, uno denominado “Ampliación” para mostrar imágenes de 500 x 500 píxeles y otro denominado “Miniatura” para mostrar imágenes de 150 x 150 píxeles. Para distribuir imágenes con los tamaños "Ampliación" y "Miniatura", un servidor de imágenes de Dynamic Media busca la definición del ajuste preestablecido de imagen Ampliación y el ajuste preestablecido de imagen en miniatura. El servidor generará dinámicamente una imagen con las especificaciones de tamaño y formato de cada ajuste preestablecido de imagen.

Dynamic Media Classic incluye varios ajustes preestablecidos de imagen "recomendados" que ya están configurados para su uso. Los administradores también pueden crear nuevos ajustes preestablecidos de imagen. Para crear un nuevo ajuste preestablecido, puede empezar desde cero o tomar uno existente como punto de partida y guardarlo con un nombre nuevo.

Téngase en cuenta que las imágenes de tamaño reducido pueden sufrir pérdidas de enfoque y detalles al distribuirse dinámicamente desde un servidor. Por esta razón, cada ajuste preestablecido de imagen contiene controles de formato para optimizar una imagen cuando se distribuye con un tamaño concreto. Estos controles garantizan la nitidez de las imágenes al llegar al sitio web o la aplicación de destino.

## Creación de un ajuste preestablecido de imagen {#creating-an-image-preset}

Los administradores pueden crear ajustes preestablecidos de imagen. Puede crear nuevos ajustes preestablecidos de imagen o empezar con un ajuste preestablecido de imagen predeterminado que proporciona Dynamic Media Classic, editarlo y guardarlo con un nombre nuevo.

**Para crear un ajuste preestablecido de imagen**

1. Haga clic en **Ajustes** &gt; **Ajustes preestablecidos de imagen**.

   Puede buscar el nombre de uno de ellos aquí para obtener una vista previa. Al seleccionar el nombre de un ajuste preestablecido, cambia el tamaño y el aspecto de la imagen de muestra en la ventana Vista previa.

1. Realice una de las siguientes acciones:

   * **Creación de un ajuste preestablecido** de imagen Haga clic en Agregar.

   * **Edición de un ajuste preestablecido** de imagen Busque el ajuste preestablecido de imagen más parecido al que desea crear y, a continuación, haga clic en Editar.

1. Asigne un nombre al ajuste.
1. Indique los valores de altura y anchura en píxeles. Estas medidas determinan el tamaño en que se distribuirán las imágenes.
1. Introduzca los datos requeridos en la pantalla Agregar ajuste preestablecido o Editar ajuste preestablecido. Para obtener más información, consulte [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options).

   Dynamic Media Classic recomienda estas opciones de "prácticas recomendadas" para comenzar:

   * **Formato** Elija JPEG u otro formato que cumpla sus requisitos. Todos los exploradores web admiten el formato de imagen JPEG, que ofrece un buen equilibrio entre tamaños de archivo pequeños y calidad de imagen. Pero las imágenes JPEG usan un esquema de compresión con pérdida que implica riesgos de defectos de imagen si el valor de compresión es demasiado bajo. Por este motivo, Dynamic Media Classic recomienda establecer la calidad de compresión (en el control deslizante) en 75. Este valor ofrece un buen equilibrio entre la calidad de imagen y el tamaño de archivo pequeño.

   * **Enfoque** No seleccione Enfoque (este filtro de enfoque ofrece menos control que la configuración de Enmascaramiento de enfoque).

   * **Volver a muestrear Modo** Elija Bicúbico.

   * **Opciones** de Máscara de enfoque (USM) Introduzca la configuración que se muestra aquí:
   | Tipo de ajuste preestablecido | Tamaño | Máscara: Cantidad | Máscara: Radio | Máscara: Umbral |
   |--- |--- |--- |--- |--- |
   | Venta cruzada (miniatura mini) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 x 150 | 1,1 | 1 | 5 |
   | Principal | 350 x 350 | 1 | 1 | 6 |
   | Ampliación | 500 x 500 | 1,2 | 1,2 | 5 |

1. Haga clic en **Guardar**.

Las opciones de "prácticas recomendadas" de Dynamic Media Classic para crear ajustes preestablecidos de imagen que se enumeran a continuación son recomendaciones generales; el enfoque es altamente subjetivo. Las “prácticas recomendadas” se basan en una imagen principal de 2000 x 2000. Las opciones deseables para imágenes mayores o menores pueden ser diferentes. Si desea ajustar la configuración de Máscara de enfoque, Dynamic Media Classic recomienda estos intervalos:

* **Importe** entre 0,8 y 1,5.

* **Radio** entre 0,6 y 2.

* **Umbral** De 1 A 6.

Para eliminar un ajuste preestablecido de imagen, selecciónelo en la pantalla Ajustes preestablecidos de imagen y seleccione el botón Eliminar.

>[!MORELIKETHIS]
>
>* [Creación y edición de ajustes preestablecidos de imagen](application-setup.md#creating_and_editing_image_presets)
>* [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options)
>* [Vista previa de un recurso de imagen en su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

