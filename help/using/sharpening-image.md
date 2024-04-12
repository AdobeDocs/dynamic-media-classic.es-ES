---
title: Enfocar una imagen
description: Obtenga información sobre cómo enfocar una imagen en Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '2199'
ht-degree: 35%

---

# Enfocar una imagen {#sharpening-an-image}

El enfoque es una técnica de manipulación de imágenes para hacer más nítidos los contornos de una imagen digital. El enfoque aumenta el contraste entre los píxeles del borde y subraya la transición entre las áreas oscuras y claras. El enfoque aumenta el contraste local y resalta el detalle fino. No existe una fórmula estricta para enfocar correctamente todas las imágenes. Muy poco enfoque puede suavizar una imagen, pero demasiado añadirá halos, artefactos y ruido.

Adobe Dynamic Media Classic recomienda encarecidamente utilizar ajustes preestablecidos de imagen para todas las imágenes. Garantizan un tamaño uniforme y el enfoque se aplica a cualquier imagen que se llame con un ajuste preestablecido de imagen. Además, puede editar y cambiar fácilmente los parámetros de enfoque de un ajuste preestablecido de imagen. La siguiente vez que publique, todas las imágenes invocadas con dicho ajuste preestablecido reciben los nuevos valores.

Adobe Dynamic Media Classic también recomienda enfocar los ajustes preestablecidos del visualizador y llamar a un visualizador con ese ajuste preestablecido. Al hacerlo, las imágenes de los espectadores resultan nítidas y atractivas.

Sin embargo, tanto si utiliza ajustes preestablecidos de imagen y ajustes preestablecidos del visualizador como si utiliza algún método de enfoque, la conclusión es que debe enfocar las imágenes. Si no lo hace, las imágenes (y el sitio web) pueden tener un aspecto suave y difuso.

>[!NOTE]
>
>los comandos de Enfocar anulan los valores de Ajuste preestablecido, incluidos sus efectos de enfoque. Un ajuste preestablecido de imagen determina el tamaño y el formato con el que se envían las imágenes desde los servidores de imágenes de Dynamic Media. Adobe Dynamic Media Classic recomienda encarecidamente utilizar ajustes preestablecidos de imagen para ofrecer todas las imágenes y garantizar que las imágenes se envíen con un tamaño y enfoque uniformes. Una vez que se cambian los valores de enfoque de una imagen individual, sin embargo, los valores de enfoque del ajuste preestablecido de imagen dejarán de aplicarse a la imagen. Se distribuye sin los valores de enfoque del ajuste preestablecido de imagen.

A menudo es necesario enfocar imágenes. Adobe Dynamic Media Classic y los servidores de imágenes ofrecen varias opciones de enfoque. Es importante entender cómo afecta el enfoque a una imagen y el grado de enfoque que necesita. La mayoría de las imágenes necesitan algo de enfoque pero la cantidad necesaria depende de la imagen.

El enfoque de imágenes aumenta el contraste de los píxeles para crear el efecto de bordes acentuados. Los seres humanos perciben esta mejora del contraste de los bordes como un enfoque. Si bien es fácil mejorar una imagen mediante filtros de enfoque aplicados a la imagen, también es fácil enfocar una imagen demasiado.

Al enfocar excesivamente una imagen, se crea un efecto de halo o una banda de las líneas del borde.

Hay prácticas recomendadas que puede seguir para optimizar el enfoque de las imágenes en Adobe Dynamic Media Classic y en Dynamic Media Image Server.

Consulte [Prácticas recomendadas para enfocar imágenes en Adobe Dynamic Media Classic y en Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Consulte también [Enfoque](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) vídeo de formación.

**Para enfocar una imagen:**

Para enfocar una imagen, seleccione su rollover **[!UICONTROL Editar]** y elija **[!UICONTROL Enfoque]**, o ábralo en el panel Examinar en la Vista de detalles y, a continuación, seleccione **[!UICONTROL Enfoque]**. Se abrirá la página Editor de enfoque con comandos de enfoque. Elija comandos y, después, seleccione **[!UICONTROL Guardar]**.

>[!NOTE]
>
>Antes de enfocar una imagen, puede seleccionar el menú Aplicar ajuste preestablecido y elegir un ajuste preestablecido de imagen para ver sus efectos de enfoque. Los efectos de enfoque de un ajuste preestablecido de imagen son adecuados para su imagen. El **[!UICONTROL Aplicar ajuste preestablecido]** se encuentra en la parte inferior de la página Editor de enfoque.

**Opciones de enfoque**

La siguiente tabla muestra las opciones de enfoque del servidor de imágenes.

| Nombre | Protocolo de URL | Valores | Ejemplo |
| --- | --- | --- | --- |
| Enfoque simple | `op_sharpen` | `0` o `1` | `op_sharpen=1` |
| Modo de remuestreo | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: selecciona la interpolación bilineal estándar. Método de remuestreo más rápido; a menudo pueden verse algunos defectos de solapamiento.<br>`bicub`: selecciona la interpolación bicúbica. Más CPU que `bilin`, pero ofrece imágenes más nítidas con defectos de solapamiento menos evidentes.<br><br>`sharp2`: selecciona una función de Lanczos Windows® modificada como algoritmo de interpolación. Puede producir resultados ligeramente más nítidos que los bicúbicos a un mayor coste de CPU.<br><br>`trilin`: selecciona una interpolación trilineal modificada, que utiliza resoluciones más altas y más bajas, si están disponibles. Solo se recomienda su uso cuando el solapamiento suponga un problema. Reducirá los tamaños de JPEG debido a la disminución de datos de alta frecuencia. | `resMode=sharp2` |
| Máscara de enfoque | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: factor de intensidad del filtro (real 0...5)<br><br>`radius`: radio del núcleo del filtro en píxeles (real 0...250) <br><br>`threshold`: nivel de umbral del filtro (int 0...255)<br><br>`monochrome`: establezca en `0` para aplicar máscara de enfoque a cada componente de color por separado, establezca como `1` para desenfocar el brillo (intensidad) de la imagen de la máscara | `op_usm=1,1,10,0` |

Seleccione el **[!UICONTROL Enfoque]** y elija una opción:

* **Ninguno** - Desactiva el enfoque.

* **Enfoque** : ejecuta una pasada de enfoque simple en el archivo después de cambiar su tamaño. Es similar al filtro &quot;Enfoque&quot; de Adobe Photoshop y no admite parámetros de usuario. Normalmente, utilizaría este filtro o **[!UICONTROL Máscara de enfoque]**, pero no ambas. Como práctica recomendada, no se recomienda utilizar este método, pero puede ayudar a compensar el desenfoque. (URL: `op_sharpen`)

* **Máscara de enfoque** - Permite ajustar un efecto de filtro de enfoque en la imagen final con disminución de resolución. Puede controlar la intensidad del efecto, el radio del efecto (medido en píxeles) y un umbral de contraste que se ignora. Este efecto utiliza las mismas opciones que el filtro &quot;Máscara de enfoque&quot; de Photoshop. (URL: `op_usm`)

Elija estas opciones para ajustar el enfoque con la máscara de enfoque:

* **Cantidad** - Controla la cantidad de contraste aplicado a los píxeles del borde. El valor predeterminado es 0,0. En las imágenes de alta resolución, puede aumentarse hasta 5,0. La cantidad equivaldría a la medida de la intensidad del filtro. El **[!UICONTROL Cantidad]** La configuración de Adobe Dynamic Media Classic no es la misma que la configuración de Importe de Adobe Photoshop. Adobe Photoshop utiliza una cantidad en el rango del 1 % al 500 %, mientras que Adobe Dynamic Media Classic escala del 0,0 al 5,0. (5,0 equivale aproximadamente al 500% en Photoshop, 0,9 es similar al 90 % y así sucesivamente).

* **Radio** : Determina el número de píxeles adyacentes a los píxeles de borde que afectan al enfoque. El efecto se ejecuta en todos los píxeles de la imagen e irradia en todas las direcciones. 

El valor de radio óptimo depende del tamaño de la imagen. Un valor bajo enfoca sólo los píxeles del borde. Un valor alto enfoca una banda más ancha de píxeles. 

Por ejemplo, para obtener un efecto de enfoque similar para una imagen de 2000 × 2000 píxeles e imagen de 500 × 500 píxeles, puede establecer un valor de radio de dos píxeles en la imagen de 2000 × 2000 píxeles. A continuación, defina un valor de radio de un píxel en la imagen de 500 × 500 píxeles (un valor mayor para una imagen con más píxeles).

* **Umbral** - Determina el intervalo de contraste que debe omitirse cuando se aplica el filtro de máscara de enfoque. Esta opción determina cómo deben ser de distintos los píxeles enfocados del área que los rodea para poder considerarse píxeles de borde y por tanto enfocarse.

Umbral utiliza un valor de 0 a 255, que es el número de pasos de brillo de una imagen en escala de grises. 0 = negro, 128 = 50% gris y 255 = blanco. Por ejemplo, el valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar ruido, al mismo tiempo que agrega contraste del borde a las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel. 

Por ejemplo, supongamos que tiene una foto de la cara de alguien. La máscara de enfoque afecta a las partes de la imagen con mayor contraste y a la piel lisa. Incluso la piel más suave presenta cambios sutiles en los valores de brillo. Si no usa un valor de umbral, el filtro acentúa estos cambios sutiles en los píxeles de la piel, lo que crea un efecto de ruido (algo probablemente no deseable) y aumenta el contraste en las pestañas, mejorando el enfoque (algo probablemente deseable). Para evitarlo, utilice un valor de umbral que indique al filtro que ignore los píxeles que no cambian de contraste considerablemente, como la piel lisa. Para evitar la introducción de ruido o imágenes de posterización con tonos de carne, por ejemplo, pruebe a experimentar con **[!UICONTROL Umbral]** valores del dos al 20. El valor predeterminado **[!UICONTROL Umbral]** el valor 0 enfoca todos los píxeles de la imagen.

* **Aplicar a** - Elegir **[!UICONTROL Cada color]** si desea aplicar el enfoque por separado a cada componente de color, elija **[!UICONTROL Brillo]** si desea aplicar enfoque a las áreas de brillo de la imagen.

**Remuestreo**

Seleccione el **[!UICONTROL Remuestreo]** y elija una opción. Estas opciones pueden enfocar la imagen cuando se disminuye su resolución:

* **[!UICONTROL Ninguno]** - Desactiva el remuestreo.

* **[!UICONTROL Bilinear]** : el método de remuestreo más rápido; pueden verse algunos defectos de solapamiento.

* **[!UICONTROL Bicúbico]** : Aumenta el uso de la CPU en el servidor de imágenes, pero genera imágenes más nítidas con artefactos de solapamiento menos evidentes.

* **[!UICONTROL `Sharpen 2`]** - Produce resultados ligeramente más nítidos que **[!UICONTROL Bicúbico]**, pero con un coste de CPU aún mayor en el servidor de imágenes.

* **[!UICONTROL Trilinear]** : Utiliza resoluciones más altas y más bajas si está disponible; recomendado solo cuando el solapamiento es un problema. Este método reduce el tamaño JPEG debido a la reducción de datos de alta frecuencia.

**Enfoque y ajustes preestablecidos de imagen**

Puede incorporar los tres efectos de enfoque para lograr el resultado final. Sin embargo, no se recomienda este método. Adobe Dynamic Media Classic recomienda guardar los efectos de enfoque como parte de un ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen permiten empaquetar los modificadores de imagen más utilizados para crear una imagen cuyo tamaño se ha cambiado dinámicamente en una cadena de texto pequeña. Un ajuste preestablecido de imagen contiene valores para el formato de archivo (normalmente JPEG para la web), el recuento de píxeles y el enfoque de imagen. En lugar de anexar la dirección URL con cada modificador de imagen que deba utilizar para crear un tipo específico de tamaño de imagen, cree un ajuste preestablecido de imagen con nombre, como &quot;miniatura&quot;. A continuación, configure el ajuste preestablecido de imagen en miniatura con el tamaño, el formato de archivo y las opciones de enfoque adecuados. Llame a la imagen con el nombre del ajuste preestablecido de imagen. Los ajustes preestablecidos de imagen acortan la longitud de la URL general. Estas dos direcciones URL producen la misma imagen de JPEG de 350 x 350 con enfoque:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Los ajustes preestablecidos de imagen se pueden cambiar y actualizar en cualquier momento. Verá los resultados de un cambio en un ajuste preestablecido de imagen después de publicar y después de que se borre la caché de la URL.

Si utiliza un ajuste preestablecido para cada imagen de una categoría de tamaño, cualquier administrador de empresa puede actualizar la definición de dicho ajuste preestablecido de imagen, volver a publicar y aplicar cambios a todas las imágenes con ese formato sin necesidad de cambiar ningún código web. La práctica recomendada es utilizar un ajuste preestablecido de imagen para cada tamaño único en el sitio. Para añadir un ajuste preestablecido de imagen, en la barra de navegación global, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Ajustes preestablecidos de imagen]**. A continuación seleccione **[!UICONTROL Añadir]** o seleccione **[!UICONTROL Editar]** para cambiar un ajuste preestablecido existente. El único campo requerido es el nombre del ajuste preestablecido. Sin embargo, es mejor incluir algún nivel de enfoque en cada ajuste preestablecido.

**Calidad JPG**

Las opciones de Calidad JPG controlan el nivel de compresión JPG:

* **Calidad JPG** - Seleccione esta opción si desea controlar los niveles de compresión y la disminución de resolución de crominancia.

* **Regulador** - Determina el nivel de compresión del JPG. Esta configuración afecta tanto al tamaño como a la calidad de la imagen. La escala de la calidad JPG va de 1 a 100.

* **Activar disminución de resolución de crominancia de JPG** - Dado que el ojo es menos sensible a la información de color de alta frecuencia que la luminancia de alta frecuencia, las imágenes JPEG dividen la información de la imagen en componentes de luminancia y color. Al comprimir una imagen JPEG, el componente de luminancia conserva la totalidad de su resolución, mientras que la resolución de los componentes de color se disminuye mediante promedios de grupos de píxeles. La disminución de la resolución reduce el volumen de datos en la mitad o en un tercio, y casi no afecta a la calidad percibida. La disminución de resolución no se aplica a las imágenes en escala de grises. Esta técnica reduce la cantidad de compresión, lo cual resulta útil para las imágenes de mayor contraste (por ejemplo, las imágenes con texto superpuesto).

**Definir opciones de enfoque para toda la empresa**

Si no ha utilizado un ajuste preestablecido de imagen ni ha pasado protocolos de enfoque específicos del servidor de imágenes a lo largo de la cadena URL, la imagen no se enfoca cuando se reduce su resolución. Sin embargo, si no se produce este enfoque, puede establecer los valores predeterminados de enfoque para garantizar que cualquier imagen tenga siempre algún enfoque.

Para establecer las opciones de enfoque predeterminadas de su empresa, vaya a **[!UICONTROL Configurar]** > **[!UICONTROL Ajustes de aplicación]** > **[!UICONTROL Ajustes de publicación]** > **[!UICONTROL Servidor de imágenes]**. Si establece el modo de remuestreo predeterminado en **`Sharp2`**, siempre enfoca la imagen cuando se reduce su resolución.

**Añadir enfoque a los ajustes preestablecidos del visor**

A menos que haya agregado modificadores de imagen de enfoque al ajuste preestablecido, la pequeña imagen de carga inicial puede parecer suave porque se ha reducido su resolución para ajustarse a la ventana del visor sin necesidad de enfoque.

Los ajustes preestablecidos del visualizador (como los ajustes preestablecidos de imagen) le permiten centralizar muchas opciones en una ubicación, incluidas las opciones de aspecto y del visualizador (como incluir un botón de impresión o controlar la velocidad de la animación de zoom). Los ajustes preestablecidos del visor se encuentran en la misma sección que los ajustes preestablecidos de imagen, en **[!UICONTROL Configurar]** > **[!UICONTROL Configuración de aplicación]** > **[!UICONTROL Ajustes preestablecidos de visor]**.

Consulte [Ajustes preestablecidos de visor](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) vídeo de formación.

La opción Modificadores se encuentra en la sección Configuración básica de todos los ajustes preestablecidos de visor de catálogos electrónicos, de conjunto de giros y de zoom personalizado. Al agregar comandos de enfoque de URL al cuadro Modificadores, se agrega enfoque cada vez que se llama a ese visor con ese ajuste preestablecido de visor.

Para llamar al ajuste preestablecido de visor, utilice el `config=` en la dirección URL del visor. A continuación, se muestra un ejemplo de llamada a un conjunto de imágenes (zapatos) con un ajuste preestablecido de visualizador (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

El ajuste preestablecido enfoca y cambia la apariencia predeterminada del visor.

**Crear invalidaciones específicas de la imagen**

El último método de enfoque (y el menos recomendado) consiste en crear anulaciones de enfoque imagen por imagen. Este método anula el enfoque de un ajuste preestablecido de imagen con sus propios valores específicos. Sin embargo, este método también anula todos los demás métodos de enfoque en cualquier tamaño. El mejor caso de uso de este método es si algunas de las imágenes no son de alta resolución y los valores de los ajustes preestablecidos de imagen son demasiado altos para estas imágenes pequeñas. En este caso, es posible que sea necesario enfocar un poco la imagen.

En Adobe Dynamic Media Classic, seleccione cualquier imagen y vaya a la Vista de detalles (haciendo doble clic o presionando ) **[!UICONTROL Vista de detalles]** ) y seleccione **[!UICONTROL Enfoque]**. Cambie cualquier parámetro y seleccione **[!UICONTROL Guardar]**. Este proceso indica al servidor de imágenes que utilice estos parámetros de enfoque en lugar de cualquier comando que se llame en la dirección URL, como un modificador de enfoque o un ajuste preestablecido de imagen. Asegúrese de publicar para ver que los cambios surten efecto.
