---
title: Opciones de edición de imágenes al cargarlas
seo-title: Opciones de edición de imágenes al cargarlas
description: nulo
seo-description: Obtenga información sobre las opciones de edición de imágenes disponibles en el momento de la carga.
uuid: 0912 ae 6 f -41 c 9-41 b 5-94 d 1-e 266 face 782 e
contentOwner: admin
content-type: referencia
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: d 3 f 21 cdf -2 cb 3-46 e 8-955 a-b 8 daf 0 b 233 bc
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Opciones de edición de imágenes al cargarlas{#image-editing-options-at-upload}

A la hora de cargar archivos de imágenes, incluidos archivos AI, EPS y PSD, podrá realizar las siguientes tareas de edición desde el cuadro de diálogo Opciones de trabajo de carga:

* Recortar el espacio en blanco del borde de imágenes.
* Recortar manualmente de los lados de imágenes.
* Elegir un perfil de color.
* Crear una máscara a partir de una ruta de recorte.
* Enfoque de imágenes con las opciones de máscara de enfoque
* Fondo de cobertura

Estas opciones se encuentran en la pantalla Cargar, en Opciones de edición de imágenes.

**Recorte de espacio en blanco de imágenes**

Para recortar automáticamente píxeles de espacio en blanco de una imagen, seleccione el menú Recortar y elija Recortar. Elija a continuación estas opciones:

**Recortar
basándose en** elegir si se desea recortar según color o transparencia:

**Color** Elija la opción Color. A continuación, en la lista desplegable Esquina, seleccione la esquina de la imagen que mejor represente el color de espacio en blanco que desea recortar.

**Transparencia Elija** la opción Transparencia.

**Tolerancia** Arrastre el control deslizante para especificar una tolerancia de 0 a 1:

**Recorte basado en color** Especifique 0 para recortar píxeles solo si coinciden exactamente con el color seleccionado en la esquina de la imagen. Los números más cercanos a 1 permiten una mayor diferencia de color.

**Recorte basado en transparencia** Especifique 0 para recortar píxeles solo si son totalmente transparentes; los números más cercanos a 1 permiten una mayor transparencia.

**Recorte manual de los lados de imágenes**

Para recortar manualmente de los lados de una imagen, seleccione el menú Recortar y elija Manual. A continuación, introduzca el número de píxeles que recortar de uno o ambos lados de la imagen. La cantidad de imagen que se recorte dependerá del valor ppp (píxeles por pulgada) en el archivo de imagen. Por ejemplo, si la imagen muestra 150 ppp y se introduce 75 en los cuadros de texto Superior, Derecha, Inferior e Izquierda, se recortará media pulgada de cada lado.

**Selección de un perfil de color**

Elija una opción Perfil de color para seleccionar un espacio de color para la imagen:

**Convertir a SRGB** Convierte a SRGB (Standard Red Green Blue). SRGB es el espacio de color que se recomienda para mostrar imágenes en páginas web.

**Mantener espacio de color original** Conserva el espacio de color original.

**Personalizar &gt; Para** abrir menús para que pueda elegir un espacio de color Convertir de y Convertir a. Puede elegir un espacio de color estándar de Photoshop o uno que haya cargado en SPS. 

Consulte [Perfiles ICC](icc-profiles.md#icc_profiles).

**Creación de una máscara a partir de una ruta de recorte**

Seleccione **Crear máscara a partir de ruta de recorte** para crear una máscara para la imagen a partir de la información sobre su ruta de recorte. Esta opción es aplicable a imágenes creadas con aplicaciones de edición de imágenes en que se ha creado una ruta de recorte.

**Enfoque de una imagen con la máscara de enfoque**

Este filtro permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución, controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se omite.

Este efecto utiliza las mismas opciones que el filtro Máscara de enfoque de Photoshop. Máscara de enfoque es un filtro de enfoque.

En Máscara de enfoque, establezca las opciones que desee. Las opciones de configuración se describen en la siguiente tabla:

| Opciones de Máscara de enfoque | Descripción |
|--- |--- |
| Cantidad | Controla el contraste que se aplica a los píxeles de bordes.<br><br>Considérelo como la intensidad del efecto. La principal diferencia entre los valores de cantidad de la máscara de enfoque en SPS y los valores de cantidad en Adobe Photoshop, es que Photoshop tiene un rango de cantidad de 1% a 500%. En cambio, en SPS, el rango de valores es de 0,0 a 5,0. Un valor de 5,0 en SPS equivale aproximadamente a 500% en Photoshop; un valor de 0,9 equivale a 90%, y así sucesivamente. |
| Radio | Controla el radio del efecto. <br><br>El rango de valores es 0-250. El efecto se ejecuta en todos los píxeles de una imagen e irradia desde todos los píxeles en todas las direcciones. El radio se mide en píxeles. Por ejemplo, para obtener un efecto de enfoque similar para una imagen de 2000 x 2000 píxeles y una imagen de 500 x 500 píxeles, podría establecer un valor de radio de dos píxeles en la imagen de 2000 x 2000 píxeles y un valor de radio de un píxel en la imagen de 500 x 500 píxeles. Para una imagen que tenga más píxeles, se utilizará un valor más alto. |
| Umbral | El umbral es un rango de contraste que se omite cuando se aplica el filtro Máscara de enfoque. Es importante no introducir ningún “ruido” en la imagen cuando se utiliza este filtro. El rango de valores es 0-255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. <br><br>Por ejemplo, un valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar ruido y, simultáneamente, agrega contraste al borde de las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel.<br><br>Así pues, en una fotografía de una cara, la máscara de enfoque afecta a las áreas contrastadas de la imagen, por ejemplo donde las pestañas tocan la piel para crear un área obvia de contraste y la piel lisa. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no utiliza un valor de umbral, el filtro enfatiza estos cambios sutiles en píxeles de piel. A su vez, se crea un efecto ruidoso e indeseable mientras el contraste en las pestañas se aumenta, lo que aumenta el enfoque.<br><br>Para evitarlo, se introduce un valor de umbral que indica al filtro que omita los píxeles que no cambien el contraste considerablemente, como la piel lisa. <br><br>En el gráfico de la cremallera mostrado anteriormente, observe la textura junto a las cremalleras. Se muestra ruido en la imagen porque los valores de umbral eran demasiado bajos para eliminar el ruido. |
| Monocromo | Selecciónelo para aplicar una máscara de enfoque al brillo (intensidad) de la imagen.<br><br>Anule su selección para aplicar la máscara de enfoque a cada componente de color por separado. |

Consulte también [Enfoque de imágenes](sharpening-image.md#sharpening_an_image).

Consulte [también Enfoque de imágenes en Scene 7 Publishing System y en el servidor de imágenes](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Fondo de cobertura**

Puede utilizar el fondo de cobertura para eliminar automáticamente el fondo de una imagen al cargarla. Esta técnica es útil para resaltar un objeto concreto y hacer que destaque en un fondo recargado.

| Opciones de fondo de cobertura | Descripción |
|:--- |:--- |
| Fondo de cobertura | Seleccione esta opción para activar o “encender” la función y las opciones de fondo de cobertura. |
| Esquina | Obligatorio.<br><br>La esquina de la imagen que se utiliza para definir el color de fondo en la cobertura.<br><br>Puede elegir entre <b>Superior izquierda, Inferior izquierda, Superior derecha o Inferior derecha</b>. |
| Método de relleno | Obligatorio. <br><br>Controla la transparencia de píxeles desde la posición de esquina que defina.<br><br>Tiene la opción de elegir entre los siguientes métodos de relleno: <ul><li><b>Relleno de inundación</b>: hace que todos los píxeles que coincidan con la esquina especificada y que estén conectados con la misma sean transparentes.</li><li><b>Coincidir con píxeles</b>: hace que todos los píxeles coincidentes sean transparentes, independientemente de su ubicación en la imagen.</li></ul> |
| Tolerancia | Opcional.<br><br>Controla la cantidad de variación permitida en la coincidencia de colores de píxeles según la ubicación de esquina que haya definido.<br><br>Utilice un valor de 0,0 para coincidir con colores de píxeles exactamente, o bien utilice un valor de 1,0 para permitir la mayor variación posible. |

>[!MORELIKETHIS]
>
>* [Recorte de imágenes](cropping-image.md#cropping_an_image)
