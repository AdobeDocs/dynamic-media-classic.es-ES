---
title: Opciones de ajuste de imagen al cargar
description: Obtenga información sobre las opciones de ajuste de imagen disponibles en el momento de la carga en Adobe Dynamic Media Classic.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 54%

---

# Opciones de ajuste de imagen al cargar{#image-editing-options-at-upload}

A la hora de cargar archivos de imágenes, incluidos archivos AI, EPS y PSD, podrá realizar las siguientes tareas de edición desde el cuadro de diálogo Opciones de trabajo de carga:

* Recortar el espacio en blanco del borde de imágenes.
* Recortar manualmente de los lados de imágenes.
* Elegir un perfil de color.
* Crear una máscara a partir de una ruta de recorte.
* Enfoque de imágenes con las opciones de máscara de enfoque
* Fondo de cobertura

Estas opciones se encuentran en la página Cargar en el encabezado **[!UICONTROL Opciones de edición de imágenes]**.

## Recortar espacio en blanco de imágenes

Para recortar automáticamente píxeles de espacio en blanco de una imagen, en el cuadro de diálogo Opciones de carga de trabajo, seleccione **[!UICONTROL Opciones de recorte]**. En la lista desplegable **[!UICONTROL Recortar]**, elija **[!UICONTROL Recortar]**. Elija a continuación estas opciones:

* **[!UICONTROL Recortar según]** : en esta lista desplegable, elija si recortar según el color o la transparencia:

   * **[!UICONTROL Color]** : elija la opción  **** Color. A continuación, en la lista desplegable **[!UICONTROL Esquina]**, seleccione la esquina de la imagen con el color que mejor represente el color del espacio en blanco que desea recortar.

   * **[!UICONTROL Transparencia]** : elija la opción Transparencia.

* **[!UICONTROL Tolerancia]** : arrastre el control deslizante para especificar una tolerancia de 0 a 1:

   * **Recorte basado en el color** : especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.

   * **Recorte basado en la transparencia** : especifique 0 para recortar píxeles solo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recortar manualmente de los lados de imágenes

Para recortar manualmente de los lados de una imagen, seleccione el menú Recortar y elija Manual. A continuación, introduzca el número de píxeles que recortar de uno o ambos lados de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, si la imagen muestra 150 ppp y se introduce 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, se recortará media pulgada de cada lado.

## Elegir un perfil de color

Para seleccionar un espacio de color para la imagen, elija una opción Perfil de color :

* **[!UICONTROL Convertir a sRGB]** : convierte a sRGB (azul verde rojo estándar). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

* **[!UICONTROL Mantener espacio de color original]** : conserva el espacio de color original.

* **[!UICONTROL Personalizar de]**  >  **[!UICONTROL A]** : abre los menús para que pueda elegir un espacio de color Convertir de y Convertir en. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Crear una máscara a partir de una ruta de recorte

Para crear una máscara para la imagen en función de su información de ruta de recorte, seleccione **[!UICONTROL Crear máscara a partir de ruta de recorte]**. Esta opción es aplicable a imágenes creadas con aplicaciones de edición de imágenes en que se ha creado una ruta de recorte.

## Enfoque de una imagen mediante una máscara sin enfoque

Este filtro permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución. Ayuda a controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se ignora.

Este efecto utiliza las mismas opciones que el filtro Máscara de enfoque de Photoshop. Máscara de enfoque es un filtro de enfoque.

En Máscara de enfoque, establezca las opciones que desee. Las opciones de configuración se describen en la siguiente tabla:

| Opciones de Máscara de enfoque | Descripción |
| --- | --- |
| Cantidad | Controla el contraste que se aplica a los píxeles de bordes.<br><br>Considérelo como la intensidad del efecto. La principal diferencia entre los valores de cantidad de Máscara de enfoque en Adobe Dynamic Media Classic y los valores de cantidad en Adobe Photoshop es que Photoshop tiene un rango de cantidad del 1% al 500%. Mientras que en Adobe Dynamic Media Classic, el intervalo de valores es de 0,0 a 5,0. Un valor de 5,0 en Adobe Dynamic Media Classic es el equivalente aproximado del 500 % en Photoshop; un valor de 0,9 es el equivalente a 90 %, etc. |
| Radio | Controla el radio del efecto. <br><br>El rango de valores es 0-250. El efecto se ejecuta en todos los píxeles de una imagen e irradia desde todos los píxeles en todas las direcciones. El radio se mide en píxeles. Por ejemplo, para obtener un efecto de nitidez similar para una imagen de 2000 x 2000 píxeles y una imagen de 500 x 500 píxeles, establecería un radio de dos píxeles en la imagen de 2000 x 2000 píxeles. Luego establezca un valor de radio de un píxel en la imagen de 500 x 500 píxeles. Para una imagen que tenga más píxeles, se utilizará un valor más alto. |
| Umbral | El umbral es un rango de contraste que se omite cuando se aplica el filtro Máscara de enfoque. Este efecto es importante para que no se introduzca ningún &quot;ruido&quot; en una imagen cuando se utilice este filtro. El rango de valores es 0-255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. <br><br>Por ejemplo, un valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar ruido y, simultáneamente, agrega contraste al borde de las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel.<br><br>Por ejemplo, si tiene una foto de la cara de alguien, la máscara de enfoque afecta a las partes contrastadas de la imagen. Por ejemplo, donde las pestañas y la piel se encuentran para crear un área obvia de contraste, y la piel suave en sí. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no utiliza un valor de umbral, el filtro enfatiza estos cambios sutiles en píxeles de piel. A su vez, se crea un efecto ruidoso e indeseable mientras el contraste en las pestañas se aumenta, lo que aumenta el enfoque.<br><br>Para evitarlo, se introduce un valor de umbral que indica al filtro que omita los píxeles que no cambien el contraste considerablemente, como la piel lisa. <br><br>En el gráfico de la cremallera mostrado anteriormente, observe la textura junto a las cremalleras. Se muestra ruido en la imagen porque los valores de umbral eran demasiado bajos para eliminar el ruido. |
| Monocromo | Selecciónelo para aplicar una máscara de enfoque al brillo (intensidad) de la imagen.<br><br>Anule su selección para aplicar la máscara de enfoque a cada componente de color por separado. |

Consulte también [Enfocar una imagen](sharpening-image.md#sharpening_an_image).

Consulte también [Enfoque de imágenes en Adobe Dynamic Media y en Image Server](/help/assets/s7_sharpening_images.pdf).

## Fondo de cobertura

Puede utilizar el fondo de cobertura para eliminar automáticamente el fondo de una imagen al cargarla. Esta técnica es útil para resaltar un objeto concreto y hacer que destaque en un fondo recargado.

| Opciones de fondo de cobertura | Descripción |
| --- | --- |
| Fondo de cobertura | Seleccione para habilitar o &quot;activar&quot; la función Fondo de Knockout y las opciones. |
| Esquina | Obligatorio.<br>La esquina de la imagen que se utiliza para definir el color de fondo en la cobertura.<br>Puede elegir entre <b>Superior izquierda, Inferior izquierda, Superior derecha o Inferior derecha</b>. |
| Método de relleno | Obligatorio. <br>Controla la transparencia de píxeles desde la posición de esquina que defina.<br>Puede elegir entre los siguientes métodos de relleno:<br> ・ Relleno <b> de </b> Flood: hace que todos los píxeles sean transparentes y coincidan con la Esquina que haya especificado y que estén conectados a ella.<br>• <b>Coincidir con píxeles</b>: hace que todos los píxeles coincidentes sean transparentes, independientemente de su ubicación en la imagen. |
| Tolerancia | Opcional.<br>Controla la cantidad de variación permitida en la coincidencia de colores de píxeles según la ubicación de esquina que haya definido.<br>Utilice un valor de 0,0 para coincidir con colores de píxeles exactamente, o bien utilice un valor de 1,0 para permitir la mayor variación posible. |

>[!MORELIKETHIS]
>
>* [Recortar una imagen](cropping-image.md#cropping_an_image)

