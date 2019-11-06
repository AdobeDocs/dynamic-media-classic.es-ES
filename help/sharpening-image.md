---
title: Enfoque de imágenes
seo-title: Enfoque de imágenes
description: nulo
seo-description: Aprenda a enfocar una imagen.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: referencia
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bbd-46a65a554409
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# Enfoque de imágenes {#sharpening-an-image}

El enfoque es una técnica de manipulación de imágenes para hacer más nítidos los contornos de una imagen digital. El enfoque aumenta el contraste entre los píxeles del borde y subraya la transición entre las áreas oscuras y claras. El enfoque aumenta el contraste local y resalta el detalle fino. No existe una fórmula estricta para enfocar correctamente todas las imágenes. Muy poco enfoque puede suavizar una imagen, pero demasiado añadirá halos, artefactos y ruido.

Dynamic Media Classic recomienda encarecidamente el uso de ajustes preestablecidos de imagen para todas las imágenes. Esto garantiza un tamaño uniforme y el enfoque se aplica a cualquier imagen llamada con un ajuste preestablecido de imagen. Además, puede editar y cambiar los parámetros de enfoque de un ajuste preestablecido de imagen con bastante facilidad. La siguiente vez que publique, todas las imágenes invocadas con dicho ajuste preestablecido reciben los nuevos valores.

Dynamic Media Classic también recomienda añadir enfoque a los ajustes preestablecidos de visor y, a continuación, llamar a un visor con ese ajuste preestablecido. Esto garantiza que las imágenes de los visores sean nítidas y atractivas.

Sin embargo, tanto si utiliza los ajustes preestablecidos de imagen y de visor o un método alternativo de enfoque, deberá enfocar las imágenes. Si no, las imágenes (y el sitio web) podrían tener un aspecto suave y borroso.

>[!NOTE]
>
>los comandos de Enfocar anulan los valores de Ajuste preestablecido, incluidos sus efectos de enfoque. Un ajuste preestablecido de imagen determina el tamaño y el formato con los que se entregan las imágenes desde los servidores de imágenes de Dynamic Media. Dynamic Media Classic recomienda encarecidamente el uso de ajustes preestablecidos de imagen para distribuir todas las imágenes y asegurarse de que las imágenes se distribuyen con un tamaño y enfoque uniformes. Una vez que se cambian los valores de enfoque de una imagen individual, sin embargo, los valores de enfoque del ajuste preestablecido de imagen dejarán de aplicarse a la imagen. Se distribuye sin los valores de enfoque del ajuste preestablecido de imagen.

A menudo es necesario enfocar imágenes. Los servidores de imágenes y SPS de Dynamic Media Classic ofrecen varias opciones de enfoque. Es importante entender cómo afecta el enfoque a una imagen y el grado de enfoque que necesita. La mayoría de las imágenes necesitan algo de enfoque pero la cantidad necesaria depende de la imagen.

El enfoque de imágenes aumenta el contraste de los píxeles para crear el efecto de bordes acentuados. Los seres humanos perciben esta mejora del contraste de los bordes como un enfoque. Si bien es fácil mejorar una imagen mediante filtros de enfoque aplicados a la imagen, también es fácil enfocar una imagen demasiado.

Al enfocar una imagen demasiado se crea un efecto de halo o bandas de las líneas del borde.

Puede seguir las prácticas recomendadas para optimizar el enfoque de las imágenes en Scene7 Publishing System y en el servidor de imágenes de Dynamic Media.

Consulte [Prácticas recomendadas para enfocar imágenes en Scene7 Publishing System y en el servidor](/help/assets/s7_sharpening_images.pdf)de imágenes de Dynamic Media.

**Para enfocar una imagen**

To sharpen an image, click its rollover **Edit** button and choose Sharpen, or open it in the Browse Panel in Detail view, then click **Sharpen**. Se abrirá la pantalla Editor de enfoque con comandos de enfoque. Elija comandos y haga clic en **Guardar**.

>[!NOTE]
>
>Antes de enfocar una imagen, puede seleccionar el menú Aplicar ajuste preestablecido y elegir un ajuste preestablecido de imagen para ver sus efectos de enfoque. Los efectos de enfoque de un ajuste preestablecido de imagen pueden resultar adecuados para la imagen. El menú Aplicar ajuste preestablecido se encuentra en la parte inferior de la pantalla Editor de enfoque.

**Opciones de enfoque**

La siguiente tabla muestra las opciones de enfoque del servidor de imágenes.

| Nombre | Protocolo de URL | Valores | Ejemplo |
|--- |--- |--- |--- |
| Enfoque simple | op_sharpen | `0 | 1` | op_sharpen=1 |
| Modo de remuestreo | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: selecciona la interpolación bilineal estándar. Método de remuestreo más rápido; pueden verse algunos defectos de solapamiento.<br>bicub: selecciona la interpolación bicúbica. Aumenta el uso de CPU con respecto a bilin, pero genera imágenes más enfocadas en las que los defectos de solapamiento son menos evidentes.<br><br>sharp2: selecciona una función de ventana Lanczos modificada como un algoritmo de interpolación. Puede producir unos resultados algo más enfocados que la opción bicúbica con un uso mayor de CPU.<br><br>trilin: selecciona una interpolación trilineal modificada, que utiliza tanto resoluciones mayores como menores, si están disponibles. Solo se recomienda su uso cuando el solapamiento suponga un problema. Reducirá los tamaños de JPEG debido a la disminución de datos de alta frecuencia. | resMode=sharp2 |
| Máscara de enfoque | op_usm | cantidad, radio, umbral,<br><br>monocromo: factor de intensidad del filtro (0...5 real)<br><br>radio: radio del núcleo del filtro en píxeles ( <br><br>umbral real 0...250): nivel de umbral de filtro (int 0...255)<br><br>monocromo: definido en 0 para aplicar máscara de enfoque a cada componente de color por separado, definido en 1 para aplicar máscara de enfoque al brillo (intensidad) de la imagen | op_usm=1,1,10,0 |

Seleccione el menú Enfoque y elija una opción:

**Ninguno** Desactiva el enfoque.

**Enfocar** Ejecuta un enfoque simple en el archivo después de cambiarlo de tamaño. Es similar al filtro "Enfocar" de Photoshop y no admite ningún parámetro de usuario. Normalmente, utilizaría este filtro o Máscara de enfoque pero no ambos. Como práctica recomendada, no se recomienda utilizar este método, pero puede ayudar a compensar el desenfoque. (URL: op_sharpen)

**Máscara** de enfoque Permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución. Puede controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se ignorará. Este efecto utiliza las mismas opciones que el filtro "Máscara de enfoque" de Photoshop. (URL: op_usm)

Elija estas opciones para precisar el enfoque con Máscara de enfoque:

**Cantidad** Controla la cantidad de contraste aplicado a los píxeles del borde. El valor predeterminado es 0,0. En las imágenes de alta resolución, puede aumentarse hasta 5,0. La cantidad equivaldría a la medida de la intensidad del filtro. Tenga en cuenta que la configuración Cantidad de Dynamic Media Classic no es la misma que la de Cantidad de Photoshop. Photoshop utiliza una cantidad en el rango de 1% a 500%, mientras que Dynamic Media Classic escala de 0,0 a 5,0. (5,0 equivale aproximadamente al 500% en Photoshop, 0,9 es similar al 90 % y así sucesivamente).

**Radio** Determina el número de píxeles que rodean los píxeles del borde que afectan al enfoque. El efecto se ejecuta en todos los píxeles de la imagen e irradia en todas las direcciones. 

El valor de radio óptimo depende del tamaño de la imagen. Un valor bajo enfoca sólo los píxeles del borde. Un valor alto enfoca una banda más ancha de píxeles. 

Por ejemplo, para obtener un efecto de enfoque similar para una imagen de 2000 x 2000 píxeles y una imagen de 500 x 500 píxeles, podría establecer un valor de radio de dos píxeles en la imagen de 2000 x 2000 píxeles. A continuación, defina un valor de radio de un píxel en la imagen de 500 x 500 píxeles (un valor mayor para una imagen con más píxeles).

**Umbral** Determina el rango de contraste que se debe ignorar al aplicar el filtro de máscara de enfoque. Esta opción determina cómo deben ser de distintos los píxeles enfocados del área que los rodea para poder considerarse píxeles de borde y por tanto enfocarse.

El umbral utiliza un valor entre 0 y 255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. Por ejemplo, el valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar ruido, al mismo tiempo que agrega contraste del borde a las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel. 

Como ejemplo, supongamos que tiene una fotografía de una cara. La máscara de enfoque afecta a las partes de la imagen con mayor contraste y a la piel lisa. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no usa un valor de umbral, el filtro acentúa estos cambios sutiles en los píxeles de la piel, lo que crea un efecto de ruido (algo probablemente no deseable) y aumenta el contraste en las pestañas, mejorando el enfoque (algo probablemente deseable). Para evitarlo, utilice un valor de umbral que indique al filtro que ignore los píxeles que no cambian de contraste considerablemente, como la piel lisa. Para evitar la introducción de ruido o posterización (en imágenes con tonos de carne, por ejemplo), intente experimentar con valores de umbral entre 2 y 20. El valor de umbral predeterminado 0 enfoca todos los píxeles de la imagen.

**Aplicar para** elegir cada color para aplicar enfoque por separado a cada componente de color; elija Brillo para aplicar enfoque a las áreas de brillo de la imagen.

**Remuestreo**

Seleccione el menú Remuestreo y elija una opción. Estas opciones pueden enfocar la imagen cuando se disminuye su resolución:

**Ninguno** Desactiva el remuestreo.

**Bilineal** El método de remuestreo más rápido; se pueden apreciar algunos artefactos de solapamiento.

**Bicúbico** Aumenta el uso de CPU en el servidor de imágenes, pero genera imágenes más nítidas con artefactos de solapamiento menos notables.

**El enfoque2** puede producir resultados ligeramente más enfocados que la opción Bicúbico, pero con un costo de CPU aún mayor en el servidor de imágenes.

**Trilineal** Utiliza tanto resoluciones altas como resoluciones inferiores si están disponibles; solo se recomienda cuando el solapamiento sea un problema. Este método reduce el tamaño JPEG debido a la reducción de datos de alta frecuencia.

**Enfoque y ajustes preestablecidos de imagen**

Puede mezclar los tres efectos de enfoque para obtener el resultado final. Sin embargo, esto no es recomendable. Dynamic Media Classic recomienda guardar los efectos de enfoque como parte de un ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen le permiten empaquetar los modificadores de imagen más utilizados para crear una imagen cuyo tamaño cambia dinámicamente en una pequeña cadena de texto. Un ajuste preestablecido de imagen contiene valores para el formato de archivo (por lo general, JPEG para la Web), recuento de píxeles y enfoque de imagen. En lugar de agregar la URL con cada modificador de imagen necesario para crear un tipo específico de tamaño de imagen, cree un ajuste preestablecido de imagen con un nombre como “miniatura”, configure el ajuste preestablecido de imagen de la miniatura con el tamaño, el formato de archivo y las opciones de enfoque adecuados y, a continuación, invoque la imagen mediante el nombre del ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen reducen la longitud total de la URL. Estas dos URL producen la misma imagen JPEG de 350 x 350 con enfoque:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Los ajustes preestablecidos de imagen se pueden cambiar y actualizar en cualquier momento. Verá los resultados de un cambio en un ajuste preestablecido de imagen después de publicar y después de que se borre la caché de la URL.

Si utiliza un ajuste preestablecido para cada imagen de una categoría de tamaño, cualquier administrador de empresa puede actualizar la definición de dicho ajuste preestablecido de imagen, volver a publicar y aplicar cambios a todas las imágenes con ese formato sin necesidad de cambiar ningún código web. La práctica recomendada es utilizar un ajuste preestablecido de imagen para cada tamaño único en el sitio. Para agregar un ajuste preestablecido de imagen, vaya a Ajustes &gt; Configuración de la aplicación &gt; Ajustes preestablecidos de imagen. A continuación, agregue o edite un ajuste preestablecido existente. El único campo requerido es el nombre del ajuste preestablecido. Sin embargo, se debe incluir algún nivel de enfoque en cada ajuste preestablecido. 

**Calidad JPG**

Las opciones de Calidad JPG controlan el nivel de compresión JPG:

**Calidad** JPG Seleccione esta opción si desea controlar los niveles de compresión y la disminución de resolución de crominancia.

**Control deslizante** Determina el nivel de compresión JPG. Esta configuración afecta tanto al tamaño como a la calidad de la imagen. La escala de calidad JPG es de 1 a 100.

**Activar disminución de resolución** de crominancia JPG Debido a que el ojo es menos sensible a la información de color de alta frecuencia que la luminancia de alta frecuencia, las imágenes JPEG dividen la información de la imagen en componentes de color y luminancia. Al comprimir una imagen JPEG, el componente de luminancia conserva la totalidad de su resolución, mientras que la resolución de los componentes de color se disminuye mediante promedios de grupos de píxeles. La disminución de resolución le resta una mitad o un tercio al volumen de los datos sin tener casi ningún impacto en la calidad percibida. La disminución de resolución no se aplica a las imágenes en escala de grises. Esta técnica reduce la cantidad de compresión, lo cual resulta útil para las imágenes de mayor contraste (por ejemplo, las imágenes con texto superpuesto).

**Configuración de las opciones de enfoque en toda la empresa**

Si no utiliza un ajuste preestablecido de imagen o transfiere protocolos de enfoque específicos del servidor de imagen junto con la cadena URL, la imagen no se enfocará cuando disminuya su resolución. Sin embargo, si esto ocurre puede definir los valores de enfoque predeterminados y, a partir de entonces, cualquier imagen tendrá siempre algo de enfoque.

Para definir las opciones de enfoque predeterminadas de la empresa, vaya a Ajustes &gt; Ajustes de aplicación &gt; Ajustes de publicación &gt; Servidor de imágenes. Si define Modo de remuestreo predeterminado en Enfocado2, siempre se enfocará la imagen cuando disminuya la resolución.

**Adición de enfoque a ajustes preestablecidos de visor**

A no ser que se agreguen modificadores de imagen de enfoque al ajuste preestablecido, la pequeña imagen inicial de carga puede parecer suave porque se ha disminuido su resolución para que se ajuste a la ventana del visor sin enfocarla.

En SPS, los ajustes preestablecidos de visor (como los ajustes preestablecidos de imagen) permiten centralizar muchas opciones en una ubicación, como una selección de opciones de apariencia y visor (por ejemplo, un botón Imprimir o el control de la velocidad de la animación de zoom). Los ajustes preestablecidos de visor se encuentran en la misma sección que los ajustes preestablecidos de imagen, en Ajustes &gt; Ajustes de la aplicación &gt; Ajustes preestablecidos de visor.

La opción Modificadores se encuentra en la sección Configuración básica de todos los ajustes preestablecidos de visor de catálogos electrónicos, de conjunto de giros y de zoom personalizado. Al agregar comandos de enfoque de URL al cuadro Modificadores, se agrega enfoque cada vez que se llama a ese visor con ese ajuste preestablecido de visor.

Para llamar al ajuste preestablecido de visor, utilice el comando config= en la URL de visor. A continuación se muestra un ejemplo de cómo llamar a un conjunto de imágenes (zapatos) con un ajuste preestablecido de visor (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

El ajuste preestablecido enfoca y cambia la apariencia predeterminada del visor.

**Creación de anulaciones específicas de la imagen**

El último método de enfoque (y el menos recomendado) consiste en crear anulaciones de enfoque imagen por imagen. Esto anula el enfoque en un ajuste preestablecido de imagen con sus propios valores específicos. Sin embargo, anula todos los demás métodos de enfoque en cualquier tamaño. El mejor caso de uso de este método es si algunas de las imágenes no son de alta resolución y los valores de los ajustes preestablecidos de imagen son demasiado altos para estas imágenes pequeñas. En este caso, podría ser necesario aplicar algo de enfoque por imagen.

En SPS, seleccione cualquier imagen, vaya a la vista de detalles (haciendo doble clic o pulsando el botón Ver detalles) y haga clic en Enfocar. Cambie cualquier parámetro y, a continuación, haga clic en Guardar. Esto indica al servidor de imágenes que utilice estos parámetros de enfoque en lugar de cualquier comando al que se llame en la URL, como un modificador de enfoque o un ajuste preestablecido de imagen. Debe publicar para que los cambios surtan efecto.
