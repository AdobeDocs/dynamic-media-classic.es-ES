---
title: Enfoque de imágenes
description: Aprenda a enfocar una imagen.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Administración de recursos
role: Business Practitioner
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '2169'
ht-degree: 46%

---

# Enfoque de imágenes {#sharpening-an-image}

El enfoque es una técnica de manipulación de imágenes para hacer más nítidos los contornos de una imagen digital. El enfoque aumenta el contraste entre los píxeles del borde y subraya la transición entre las áreas oscuras y claras. El enfoque aumenta el contraste local y resalta el detalle fino. No existe una fórmula estricta para enfocar correctamente todas las imágenes. Muy poco enfoque puede suavizar una imagen, pero demasiado añadirá halos, artefactos y ruido.

Dynamic Media Classic recomienda encarecidamente utilizar ajustes preestablecidos de imagen para todas las imágenes. Garantizan un tamaño uniforme y el enfoque se aplica en cualquier imagen llamada con un ajuste preestablecido de imagen. Además, puede editar y cambiar fácilmente los parámetros de nitidez de un ajuste preestablecido de imagen. La siguiente vez que publique, todas las imágenes invocadas con dicho ajuste preestablecido reciben los nuevos valores.

Dynamic Media Classic también recomienda añadir nitidez a los ajustes preestablecidos de visualizador y, a continuación, llamar a un visualizador con ese ajuste preestablecido. Al hacerlo, se garantiza que las imágenes de los espectadores sean nítidas y atractivas.

Sin embargo, tanto si utiliza ajustes preestablecidos de imagen y ajustes preestablecidos de visualizador como si utiliza algún método alternativo de nitidez, la conclusión es que debe enfocar las imágenes. Si no lo hace, las imágenes (y el sitio web) pueden verse suaves y borrosas.

>[!NOTE]
>
>los comandos de Enfocar anulan los valores de Ajuste preestablecido, incluidos sus efectos de enfoque. Los ajustes preestablecidos de imagen rigen el tamaño y el formato con que se entregan las imágenes desde los servidores de imágenes de Dynamic Media. Dynamic Media Classic recomienda encarecidamente utilizar ajustes preestablecidos de imagen para entregar todas las imágenes con el fin de garantizar que se entreguen a un tamaño y un enfoque uniformes. Una vez que se cambian los valores de enfoque de una imagen individual, sin embargo, los valores de enfoque del ajuste preestablecido de imagen dejarán de aplicarse a la imagen. Se distribuye sin los valores de enfoque del ajuste preestablecido de imagen.

A menudo es necesario enfocar imágenes. Los servidores de imágenes y Dynamic Media Classic ofrecen varias opciones de enfoque. Es importante entender cómo afecta el enfoque a una imagen y el grado de enfoque que necesita. La mayoría de las imágenes necesitan algo de enfoque pero la cantidad necesaria depende de la imagen.

El enfoque de imágenes aumenta el contraste de los píxeles para crear el efecto de bordes acentuados. Los seres humanos perciben esta mejora del contraste de los bordes como un enfoque. Si bien es fácil mejorar una imagen mediante filtros de enfoque aplicados a la imagen, también es fácil enfocar una imagen demasiado.

Al enfocar una imagen demasiado se crea un efecto de halo o bandas de las líneas del borde.

Puede seguir algunas prácticas recomendadas para optimizar el enfoque de las imágenes en Dynamic Media Classic y en Dynamic Media Image Server.

Consulte [Prácticas recomendadas para enfocar imágenes en Dynamic Media Classic y en Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**Para enfocar una imagen:**

Para enfocar una imagen, haga clic en su botón de rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Enfocar]**, o ábrala en el panel Examinar de la vista de detalles y, a continuación, haga clic en **[!UICONTROL Enfocar]**. Se abre la página Editor de nitidez con comandos de nitidez. Elija los comandos y, a continuación, haga clic en **[!UICONTROL Save]**.

>[!NOTE]
>
>Antes de enfocar una imagen, puede seleccionar el menú Aplicar ajuste preestablecido y elegir un ajuste preestablecido de imagen para ver sus efectos de enfoque. Los efectos de nitidez de un ajuste preestablecido de imagen son adecuados para su imagen. El menú **[!UICONTROL Aplicar ajuste preestablecido]** se encuentra en la parte inferior de la página Editor de enfoque.

**Opciones de enfoque**

La siguiente tabla muestra las opciones de enfoque del servidor de imágenes.

| Nombre | Protocolo de URL | Valores | Ejemplo |
|--- |--- |--- |--- |
| Enfoque simple | op_sharpen | `0 | 1` | op_sharpen=1 |
| Modo de remuestreo | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: selecciona la interpolación bilineal estándar. Método de remuestreo más rápido; a menudo se pueden apreciar algunos artefactos de aliasing.<br>bicub: selecciona la interpolación bicúbica. Aumenta el uso de CPU con respecto a bilin, pero genera imágenes más enfocadas en las que los defectos de solapamiento son menos evidentes.<br><br>agudo2: Selecciona una función Windows® de Lanczos modificada como algoritmo de interpolación. Puede producir resultados ligeramente más nítidos que los bicúbicos a un mayor costo de CPU.<br><br>trilin: selecciona una interpolación trilineal modificada, que utiliza tanto resoluciones mayores como menores, si están disponibles. Solo se recomienda su uso cuando el solapamiento suponga un problema. Reducirá los tamaños de JPEG debido a la disminución de datos de alta frecuencia. | resMode=sharp2 |
| Máscara de enfoque | op_usm | cantidad, radio, umbral, monocromo<br><br>cantidad: factor de intensidad del filtro (real 0...5)<br><br>radio: filtro radio del núcleo en píxeles (real 0...250) <br><br>umbral: nivel de umbral de filtro (int 0...255)<br><br>monocromo: se establece en 0 para aplicar máscara de enfoque a cada componente de color por separado, se establece en 1 para aplicar máscara de enfoque al brillo (intensidad) de la imagen | op_usm=1,1,10,0 |

Seleccione el menú **[!UICONTROL Sharpening]** y elija una opción:

* **Ninguno** : deshabilita el enfoque.

* **Enfoque** : ejecuta un paso de enfoque simple en el archivo después de cambiar su tamaño. Es similar al filtro &quot;Perfilar&quot; de Adobe Photoshop y admite cualquier parámetro de usuario. Normalmente, utilizaría este filtro o **[!UICONTROL Máscara de enfoque]**, pero no ambos. Como práctica recomendada, no se recomienda utilizar este método, pero puede ayudar a compensar el desenfoque. (URL: `op_sharpen`)

* **Máscara de enfoque** : le permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución. Puede controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se ignora. Este efecto utiliza las mismas opciones que el filtro “Máscara de enfoque” de Photoshop. (URL: `op_usm`)

Elija estas opciones para ajustar el enfoque con Máscara de enfoque:

* **Cantidad** : controla la cantidad de contraste aplicado a los píxeles de borde. El valor predeterminado es 0,0. En las imágenes de alta resolución, puede aumentarse hasta 5,0. La cantidad equivaldría a la medida de la intensidad del filtro. La configuración **[!UICONTROL Amount]** de Dynamic Media Classic no es la misma que la configuración de Amount de Adobe Photoshop. Adobe Photoshop utiliza una cantidad del rango del 1 % al 500 %, mientras que Dynamic Media Classic escala de 0,0 a 5,0. (5,0 equivale aproximadamente al 500% en Photoshop, 0,9 es similar al 90 % y así sucesivamente).

* **Radio** : determina el número de píxeles que rodean los píxeles de borde que afectan al enfoque. El efecto se ejecuta en todos los píxeles de la imagen e irradia en todas las direcciones. 

El valor de radio óptimo depende del tamaño de la imagen. Un valor bajo enfoca sólo los píxeles del borde. Un valor alto enfoca una banda más ancha de píxeles. 

Por ejemplo, para obtener un efecto de nitidez similar para una imagen de 2000 x 2000 píxeles y una imagen de 500 x 500 píxeles, puede establecer un valor de radio de dos píxeles en la imagen de 2000 x 2000 píxeles. A continuación, defina un valor de radio de un píxel en la imagen de 500 x 500 píxeles (un valor mayor para una imagen con más píxeles).

* **** UmbralDetermina el intervalo de contraste que se debe ignorar cuando se aplica el filtro de máscara de enfoque. Esta opción determina cómo deben ser de distintos los píxeles enfocados del área que los rodea para poder considerarse píxeles de borde y por tanto enfocarse.

El umbral utiliza un valor entre 0 y 255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. Por ejemplo, el valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar ruido, al mismo tiempo que agrega contraste del borde a las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel. 

Como ejemplo, supongamos que tiene una fotografía de una cara. La máscara de enfoque afecta a las partes de la imagen con mayor contraste y a la piel lisa. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no usa un valor de umbral, el filtro acentúa estos cambios sutiles en los píxeles de la piel, lo que crea un efecto de ruido (algo probablemente no deseable) y aumenta el contraste en las pestañas, mejorando el enfoque (algo probablemente deseable). Para evitarlo, utilice un valor de umbral que indique al filtro que ignore los píxeles que no cambian de contraste considerablemente, como la piel lisa. Para evitar la introducción de ruido o poserización en imágenes con tonos de carne, por ejemplo, intente experimentar con los valores **[!UICONTROL Umbral]** de dos a 20. El valor predeterminado **[!UICONTROL Umbral]** de 0 enfoca todos los píxeles de la imagen.

* **Aplicar a** : elija  **[!UICONTROL cada]** color si desea aplicar enfoque por separado a cada componente de color; seleccione  **** Brightnessisi si desea aplicar nitidez a las áreas de brillo de la imagen.

**Remuestreo**

Haga clic en el menú **[!UICONTROL Remuestreo]** y seleccione una opción. Estas opciones pueden enfocar la imagen cuando se disminuye su resolución:

* **Ninguno** : desactiva el remuestreo.

* **Bilinear** : el método de remuestreo más rápido; se pueden apreciar algunos artefactos de aliasing.

* **Bicúbico** : Aumenta el uso de CPU en el servidor de imágenes, pero genera imágenes más nítidas con artefactos de alias menos visibles.

* **Enfoque2** : produce resultados ligeramente más nítidos que los de  **[!UICONTROL Bicúbico]**, pero a un costo de CPU aún mayor en el servidor de imágenes.

* **Trilineal** : utiliza resoluciones más altas y más bajas si están disponibles; recomendado solo cuando el alias sea un problema. Este método reduce el tamaño JPEG debido a la reducción de datos de alta frecuencia.

**Enfoque y ajustes preestablecidos de imagen**

Puede incorporar los tres efectos de nitidez para lograr su resultado final. Sin embargo, no se recomienda este método. Dynamic Media Classic recomienda guardar los efectos de enfoque como parte de un ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen le permiten empaquetar los modificadores de imagen más utilizados para crear una imagen cuyo tamaño se ha cambiado dinámicamente en una pequeña cadena de texto. Un ajuste preestablecido de imagen contiene valores para el formato de archivo (normalmente JPEG para la Web), el recuento de píxeles y el enfoque de la imagen. En lugar de anexar la URL con cada modificador de imagen que debe utilizar para crear un tipo específico de tamaño de imagen, cree un ajuste preestablecido de imagen con nombre, como &quot;miniatura&quot;. A continuación, configure el ajuste preestablecido de imagen en miniatura con el tamaño, el formato de archivo y las opciones de nitidez adecuados. Llame a la imagen con el nombre del ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen acortan la longitud de la dirección URL general. Estas dos direcciones URL producen la misma imagen JPEG de 350 x 350 con nitidez:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Los ajustes preestablecidos de imagen se pueden cambiar y actualizar en cualquier momento. Verá los resultados de un cambio en un ajuste preestablecido de imagen después de publicar y después de que se borre la caché de la URL.

Si utiliza un ajuste preestablecido para cada imagen de una categoría de tamaño, cualquier administrador de empresa puede actualizar la definición de dicho ajuste preestablecido de imagen, volver a publicar y aplicar cambios a todas las imágenes con ese formato sin necesidad de cambiar ningún código web. La práctica recomendada es utilizar un ajuste preestablecido de imagen para cada tamaño único en el sitio. Para agregar un ajuste preestablecido de imagen, en la barra de navegación global, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Ajustes preestablecidos de imagen]**. A continuación, haga clic en **[!UICONTROL Agregar]** o haga clic en **[!UICONTROL Editar]** para cambiar un ajuste preestablecido existente. El único campo requerido es el nombre del ajuste preestablecido. Sin embargo, es mejor incluir algún nivel de nitidez en cada ajuste preestablecido.

**Calidad JPG**

Las opciones de Calidad JPG controlan el nivel de compresión JPG:

* **Calidad JPG** : seleccione esta opción si desea controlar los niveles de compresión y la disminución de resolución de crominancia.

* **Control deslizante** : determina el nivel de compresión JPG. Esta configuración afecta tanto al tamaño como a la calidad de la imagen. La escala de calidad JPG es de 1 a 100.

* **Activar el muestreo descendente de crominancia JPG** : como el ojo es menos sensible a la información de color de alta frecuencia que la luminancia de alta frecuencia, las imágenes JPEG dividen la información de la imagen en componentes de luminancia y color. Al comprimir una imagen JPEG, el componente de luminancia conserva la totalidad de su resolución, mientras que la resolución de los componentes de color se disminuye mediante promedios de grupos de píxeles. La disminución de resolución le resta una mitad o un tercio al volumen de los datos sin tener casi ningún impacto en la calidad percibida. La disminución de resolución no se aplica a las imágenes en escala de grises. Esta técnica reduce la cantidad de compresión, lo cual resulta útil para las imágenes de mayor contraste (por ejemplo, las imágenes con texto superpuesto).

**Configuración de las opciones de enfoque en toda la empresa**

Si no utiliza un ajuste preestablecido de imagen o transfiere protocolos de enfoque específicos del servidor de imagen junto con la cadena URL, la imagen no se enfocará cuando disminuya su resolución. Sin embargo, si se produce esta falta de nitidez, puede establecer valores de nitidez predeterminados y, a continuación, cualquier imagen siempre tiene un enfoque.

Para establecer las opciones de enfoque predeterminadas de su empresa, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la aplicación]** > **[!UICONTROL Configuración de publicación]** > **[!UICONTROL Servidor de imágenes]**. Si establece el modo de remuestreo predeterminado en **[!UICONTROL Sharp2]**, siempre afilará la imagen al reducirla.

**Adición de enfoque a ajustes preestablecidos de visor**

A no ser que se agreguen modificadores de imagen de enfoque al ajuste preestablecido, la pequeña imagen inicial de carga puede parecer suave porque se ha disminuido su resolución para que se ajuste a la ventana del visor sin enfocarla.

Los ajustes preestablecidos de visor (como los ajustes preestablecidos de imagen) permiten centralizar muchas opciones en una ubicación, incluida la selección de opciones de aspecto y visor (como un botón de impresión o el control de la velocidad de la animación de zoom). Los ajustes preestablecidos de visor se encuentran en la misma sección que los ajustes preestablecidos de imagen, en **[!UICONTROL Configuración]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes preestablecidos de visor]**.

La opción Modificadores se encuentra en la sección Configuración básica de todos los ajustes preestablecidos de visor de catálogos electrónicos, de conjunto de giros y de zoom personalizado. Al agregar comandos de enfoque de URL al cuadro Modificadores, se agrega enfoque cada vez que se llama a ese visor con ese ajuste preestablecido de visor.

Para llamar al ajuste preestablecido de visualizador, utilice el comando `config=` en la dirección URL del visor. A continuación se muestra un ejemplo de cómo llamar a un conjunto de imágenes (zapatos) con un ajuste preestablecido de visor (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

El ajuste preestablecido enfoca y cambia la apariencia predeterminada del visor.

**Creación de anulaciones específicas de la imagen**

El último método de enfoque (y el menos recomendado) consiste en crear anulaciones de enfoque imagen por imagen. Este método anula el enfoque en un ajuste preestablecido de imagen con sus propios valores específicos. Sin embargo, este método también anula todos los demás métodos de nitidez a cualquier tamaño. El mejor caso de uso de este método es si algunas de las imágenes no son de alta resolución y los valores de los ajustes preestablecidos de imagen son demasiado altos para estas imágenes pequeñas. En este caso, es posible que se necesite un cierto enfoque por imagen.

En Dynamic Media Classic, seleccione cualquier imagen, vaya a la Vista de detalles (haciendo doble clic o pulsando el botón **[!UICONTROL Vista de detalles]**) y haga clic en **[!UICONTROL Enfocar]**. Cambie cualquier parámetro y haga clic en **[!UICONTROL Guardar]**. Este proceso indica al servidor de imágenes que utilice estos parámetros de nitidez en lugar de cualquier comando al que llame en la URL, como un modificador de nitidez o un ajuste preestablecido de imagen. Asegúrese de publicar para ver que los cambios surten efecto.
