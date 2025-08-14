---
title: Opciones de ajuste de imagen al cargar
description: Obtenga información acerca de las opciones de ajuste de imágenes disponibles en el momento de la carga en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 28%

---

# Opciones de ajuste de imagen al cargar{#image-editing-options-at-upload}

A la hora de cargar archivos de imágenes, incluidos archivos AI, EPS y PSD, podrá realizar las siguientes tareas de edición desde el cuadro de diálogo Opciones de trabajo de carga:

* Recorte el espacio en blanco desde el borde de las imágenes.
* Recortar manualmente de los lados de imágenes.
* Elegir un perfil de color.
* Crear una máscara a partir de una ruta de recorte.
* Enfoque de imágenes con las opciones de máscara de enfoque
* Fondo de cobertura

Estas opciones se encuentran en la página Cargar bajo el encabezado **[!UICONTROL Opciones de edición de imágenes]**.

## Recortar espacio en blanco de las imágenes

Puede recortar automáticamente los píxeles del espacio en blanco de una imagen. En el cuadro de diálogo Cargar opciones del trabajo, seleccione **[!UICONTROL Opciones de recorte]**. En la lista desplegable **[!UICONTROL Recortar]**, elija **[!UICONTROL Recortar]**. Elija a continuación estas opciones:

* **[!UICONTROL Recortar basándose en]**: en esta lista desplegable, elija si desea recortar basándose en el color o en la transparencia:

   * **[!UICONTROL Color]**: elige la opción **[!UICONTROL Color]**. A continuación, en la lista desplegable **[!UICONTROL Esquina]**, seleccione la esquina de la imagen con el color que mejor represente el color del espacio en blanco que desee recortar.

   * **[!UICONTROL Transparencia]**: elija la opción Transparencia.

* **[!UICONTROL Tolerancia]**: arrastre el control deslizante para especificar una tolerancia de 0 a 1:

   * **Recorte basado en el color**: especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.

   * **Recorte basado en la transparencia**: especifique 0 para recortar píxeles sólo si son transparentes; los números más cercanos a 1 permiten una mayor transparencia.

## Recortar manualmente desde los lados de las imágenes

Para recortar manualmente de los lados de una imagen, seleccione el menú Recortar y elija Manual. A continuación, introduzca el número de píxeles que recortar de uno o ambos lados de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, supongamos que la imagen muestra 150 ppp. A continuación, escriba 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda. En este punto, cada lado se recorta 0,5 pulgadas.

## Elija un perfil de color

Para seleccionar un espacio de color para la imagen, elija una opción de Perfil de color:

* **[!UICONTROL Convertir a sRGB]**: Convierte a sRGB (azul rojo y verde estándar). sRGB es el espacio de color recomendado para mostrar imágenes en páginas Web.

* **[!UICONTROL Conservar el espacio de color original]**: conserva el espacio de color original.

* **[!UICONTROL Personalizar desde]** > **[!UICONTROL hasta]**: abre menús para que pueda elegir un espacio de color Convertir desde y Convertir a. Puede elegir un espacio de color estándar de Photoshop o un espacio de color que haya cargado en Adobe Dynamic Media Classic.

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

## Creación de una máscara a partir de un trazado de recorte

Para crear una máscara para la imagen basada en la información de ruta de recorte, seleccione **[!UICONTROL Crear máscara a partir de ruta de recorte]**. Esta opción es aplicable a imágenes creadas con aplicaciones de edición de imágenes en que se ha creado una ruta de recorte.

## Enfoque de una imagen mediante la máscara de enfoque

Este filtro le permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución. Ayuda a controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se ignora.

Este efecto utiliza las mismas opciones que el filtro Máscara de enfoque de Photoshop. Máscara de enfoque es un filtro de enfoque.

En Máscara de enfoque, establezca las opciones que desee. Las opciones de configuración se describen en la siguiente tabla:

| Opciones de Máscara de enfoque | Descripción |
| --- | --- |
| Cantidad | Cantidad controla la cantidad de contraste que se aplica a los píxeles del borde.<br><br>Considérelo como la intensidad del efecto. Hay una diferencia entre los valores de cantidad de Máscara de enfoque en Dynamic Media Classic y en Adobe Photoshop. La principal diferencia es que Photoshop tiene un rango de cantidades de 1% a 500%. Mientras que en Adobe Dynamic Media Classic, el rango de valores es de 0,0 a 5,0. Un valor de 5,0 en Adobe Dynamic Media Classic es el equivalente aproximado de 500% en Photoshop; un valor de 0,9 es el equivalente de 90%, y así sucesivamente. |
| Radio | Controla el radio del efecto. <br><br>El intervalo de valores es de 0 a 250. El efecto se ejecuta en todos los píxeles de una imagen e irradia desde todos los píxeles en todas las direcciones. El radio se mide en píxeles. Por ejemplo, para obtener un efecto de enfoque similar para una imagen de 2000 × 2000 píxeles e imagen de 500 × 500 píxeles, debe establecer un radio de dos píxeles en la imagen de 2000 × 2000 píxeles. A continuación, defina un valor de radio de un píxel en la imagen de 500 × 500 píxeles. Para una imagen que tenga más píxeles, se utilizará un valor más alto. |
| Umbral | El umbral es un rango de contraste que se omite cuando se aplica el filtro Máscara de enfoque. Este efecto es importante para que no se introduzca ningún &quot;ruido&quot; en una imagen cuando se utilice este filtro. El rango de valores es 0-255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. <br><br>Por ejemplo, un valor de umbral de 12 ignora las ligeras variaciones en el brillo del tono de la piel para evitar agregar ruido, pero agrega contraste al borde de las áreas de contrastes, como cuando las pestañas tocan la piel.<br><br>Por ejemplo, si tiene una foto de la cara de alguien, la máscara de enfoque afecta a las partes de contraste de la imagen. Por ejemplo, donde las pestañas y la piel se juntan para crear una zona obvia de contraste, y la piel lisa en sí misma. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no utiliza un valor de umbral, el filtro enfatiza estos cambios sutiles en píxeles de piel. A su vez, se crea un efecto ruidoso e indeseable mientras el contraste en las pestañas se aumenta, lo que aumenta el enfoque.<br><br>Para evitar este problema, se introduce un valor de umbral que indica al filtro que ignore los píxeles que no cambian drásticamente el contraste, como la apariencia suave. <br><br>En el gráfico de cremallera mostrado anteriormente, observe la textura junto a las cremalleras. El ruido de la imagen se muestra porque los valores de umbral son demasiado bajos para suprimir el ruido. |
| Monocromo | Selecciónelo para aplicar una máscara de enfoque al brillo (intensidad) de la imagen.<br><br>Anule la selección para aplicar máscara de enfoque a cada componente de color por separado. |

Consulte también [Enfoque de una imagen](sharpening-image.md#sharpening_an_image).

Vea también [Enfoque de imágenes en Adobe Dynamic Media y en Image Server](/help/using/assets/s7_sharpening_images.pdf).

## Fondo de cobertura

Utilice Fondo de cobertura para poder eliminar automáticamente el fondo de una imagen cuando la cargue. Esta técnica es útil para resaltar un objeto concreto y hacer que destaque en un fondo recargado.

| Opciones de fondo de cobertura | Descripción |
| --- | --- |
| Fondo de cobertura | Seleccione esta opción para activar o &quot;activar&quot; la función y las opciones de Fondo de cobertura. |
| Esquina | Obligatorio.<br>Esquina de la imagen que se usa para definir el color de fondo que se va a noquear.<br>Puede elegir entre <b>Superior izquierdo, Inferior izquierdo, Superior derecho o Inferior derecho</b>. |
| Método de relleno | Requerido. <br>Controla la transparencia de píxeles desde la ubicación de Corner que haya establecido.<br>Puede elegir entre los siguientes métodos de relleno:<br>· <b>Relleno de inundación</b>: convierte en transparentes todos los píxeles que coincidan con la Esquina que ha especificado y que estén conectados a ella.<br>· <b>Píxel coincidente</b>: vuelve transparentes todos los píxeles coincidentes, independientemente de su ubicación en la imagen. |
| Tolerancia | Opcional.<br>Controla la cantidad de variación permitida en la coincidencia de color de píxel en función de la ubicación de Esquina que haya establecido.<br>Use un valor de 0,0 para que coincida exactamente con los colores de los píxeles. O bien, use un valor de 1,0 para permitir la mayor variación. |

>[!MORELIKETHIS]
>
>* [Recortar una imagen](cropping-image.md#cropping_an_image)
