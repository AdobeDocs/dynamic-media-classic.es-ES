---
title: Configurar ajustes preestablecidos de imagen
description: Obtenga información sobre cómo configurar ajustes preestablecidos de imagen en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:12:02.112Z'
TQID: 'https://experienceleague.adobe.com/a4ns4AjIZccBHisG5jIf7Wkm0iK5TNp2q4xSZit-RrQ'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: e692b0e39f641db097413710611d19dc30ad42b7
workflow-type: tm+mt
source-wordcount: 670
ht-degree: 29%

---

# Configurar ajustes preestablecidos de imagen{#setting-up-image-presets}

Un ajuste preestablecido de imagen, que se guarda con un nombre exclusivo, es similar a una macro y se compone de una serie de comandos de formato y tamaño predefinidos. Para comprender cómo funcionan los ajustes preestablecidos de imagen, supongamos que el sitio Web requiere que cada imagen de producto aparezca en dos tamaños diferentes: 500 × 500 píxeles y 150 × 150 píxeles. Puede crear dos ajustes preestablecidos de imagen, uno denominado &quot;Ampliar&quot; para mostrar imágenes a 500x500 píxeles y otro denominado &quot;Miniatura&quot; para mostrar imágenes a 150 × 150 píxeles. Para ofrecer imágenes con los tamaños &quot;Ampliar&quot; y &quot;Miniatura&quot;, un servidor de imágenes de Dynamic Media busca la definición de los ajustes preestablecidos &quot;Ampliar imagen&quot; y &quot;Miniatura de imagen&quot;. El servidor generará dinámicamente una imagen con las especificaciones de tamaño y formato de cada ajuste preestablecido de imagen.

Adobe Dynamic Media Classic incluye varios ajustes preestablecidos de imagen de prácticas recomendadas que ya están configurados para que los utilice. Los administradores también pueden crear ajustes preestablecidos de imagen. Para crear un ajuste preestablecido de imagen, puede crear uno nuevo o puede empezar desde uno existente y guardarlo con un nombre nuevo.

Téngase en cuenta que las imágenes de tamaño reducido pueden sufrir pérdidas de enfoque y detalles al distribuirse dinámicamente desde un servidor. Por esta razón, cada ajuste preestablecido de imagen contiene controles de formato para optimizar una imagen cuando se distribuye con un tamaño concreto. Estos controles garantizan la nitidez de las imágenes al llegar a la página o aplicación de destino.

## Crear un ajuste preestablecido de imagen {#creating-an-image-preset}

Puede crear sus propios ajustes preestablecidos de imagen si es administrador de la empresa. Puede crear ajustes preestablecidos de imagen o utilizar un ajuste preestablecido de imagen predeterminado que proporciona Adobe Dynamic Media Classic, editarlo y guardarlo con un nombre nuevo.

**Para crear un ajuste preestablecido de imagen:**

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes preestablecidos de imagen]**.

   Para previsualizar un ajuste preestablecido de imagen existente, puede buscar un nombre de ajuste preestablecido de imagen en esta pantalla. Al seleccionar el nombre de un ajuste preestablecido, cambia el tamaño y el aspecto de la imagen de muestra en la ventana Vista previa.

1. Realice una de las siguientes acciones:

   * **Crear un ajuste preestablecido de imagen**: seleccione **[!UICONTROL Agregar]**.
   * **Editar un ajuste preestablecido de imagen**: busque el ajuste preestablecido de imagen más similar al que desea crear y, a continuación, seleccione **[!UICONTROL Editar]**.

1. Asigne un nombre al ajuste.
1. Indique los valores de altura y anchura en píxeles. Estas medidas determinan el tamaño en que se distribuirán las imágenes.
1. Introduzca los datos requeridos en la pantalla Agregar ajuste preestablecido o Editar ajuste preestablecido. Para obtener más información, consulte [Opciones de ajuste preestablecido de imagen](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic recomienda estas opciones de &quot;práctica recomendada&quot; para comenzar:

   * **[!UICONTROL Formato]**: Elija JPEG u otro formato que cumpla sus requisitos. Todos los navegadores web admiten el formato de imagen JPEG; ofrece un buen equilibrio entre los tamaños de archivo pequeños y la calidad de imagen. Sin embargo, las imágenes de JPEG utilizan un esquema de compresión con pérdidas que puede introducir artefactos de imagen no deseados si el ajuste de compresión es demasiado bajo. Por este motivo, Adobe Dynamic Media Classic recomienda establecer la calidad de compresión (en el control deslizante) en 75. Este valor ofrece un buen equilibrio entre la calidad de imagen y el tamaño de archivo pequeño.

   * **[!UICONTROL Enfoque]**: No seleccione Enfoque (este filtro de enfoque ofrece menos control que la configuración de **[!UICONTROL Máscara de enfoque]**).

   * **[!UICONTROL Modo de remuestreo]**: Elija **[!UICONTROL Bicúbico]**.

   * **[!UICONTROL Máscara de enfoque]** (USM): introduzca la siguiente configuración:

   | Tipo de ajuste preestablecido | Tamaño | Máscara: Cantidad | Máscara: Radio | Máscara: Umbral |
   | --- | --- | --- | --- | --- |
   | Venta cruzada (miniatura mini) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniatura | 150 × 150 | 1,1 | 1 | 5 |
   | Principal | 350 × 350 | 1 | 1 | 6 |
   | Ampliación | 500 × 500 | 1,2 | 1,2 | 5 |

1. Seleccione **[!UICONTROL Guardar]**.

Las opciones de &quot;práctica recomendada&quot; de Adobe Dynamic Media Classic para crear ajustes preestablecidos de imagen que se enumeran a continuación son recomendaciones generales; el enfoque es muy subjetivo. Esta configuración de &quot;prácticas recomendadas&quot; se basó en una imagen principal de 2000 × 2000; la configuración de los archivos principales más grandes o más pequeños puede ser diferente. Si desea ajustar la configuración de la máscara de enfoque, Adobe Dynamic Media Classic recomienda estos intervalos:

* **[!UICONTROL Importe]**: entre `.8` y `1.5`.

* **[!UICONTROL Radio]**: Entre `.6` y `2`.

* **[!UICONTROL Umbral]**: Desde `1` hasta `6`.

Para eliminar un ajuste preestablecido de imagen, selecciónelo en la pantalla Ajustes preestablecidos de imagen y, a continuación, seleccione **[!UICONTROL Eliminar]**.

>[!MORELIKETHIS]
>
>* [Crear y editar ajustes preestablecidos de imagen](application-setup.md#creating_and_editing_image_presets)
>* [Opciones de ajustes preestablecidos de imagen](application-setup.md#image_preset_options)
>* [Previsualizar un recurso de imagen en función de su ajuste preestablecido de imagen](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
