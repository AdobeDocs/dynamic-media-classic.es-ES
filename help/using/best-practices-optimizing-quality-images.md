---
title: Prácticas recomendadas para optimizar la calidad de las imágenes
description: Conozca las prácticas recomendadas para optimizar la calidad de las imágenes.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '1601'
ht-degree: 45%

---

# Prácticas recomendadas para optimizar la calidad de las imágenes{#best-practices-for-optimizing-the-quality-of-your-images}

Optimizar la calidad de la imagen puede consumir mucho tiempo. Muchos factores contribuyen a obtener resultados aceptables. El resultado es en parte subjetivo porque distintas personas perciben la calidad de las imágenes de forma distinta. La clave es la experimentación estructurada.

Adobe Dynamic Media Classic incluye más de 100 comandos de servidor de imágenes para ajustar y optimizar imágenes y procesar resultados. Las directrices siguientes pueden ayudarle a agilizar el proceso y a obtener buenos resultados con rapidez utilizando ciertos comandos esenciales y prácticas recomendadas.

Consulte también [Imágenes inteligentes](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Pruebe y descubra las ventajas de los modificadores de imagen de Dynamic Media y de las imágenes inteligentes con Dynamic Media [_Instantánea_](https://snapshot.scene7.com/).
>
> Snapshot es una herramienta de demostración visual diseñada para ilustrar la potencia de Dynamic Media para la entrega de imágenes optimizadas y dinámicas. Experimente con imágenes de prueba o direcciones URL de Dynamic Media para observar visualmente la salida de varios modificadores de imagen de Dynamic Media y optimizaciones de imágenes inteligentes para lo siguiente:
>* Tamaño de archivo (con envío WebP y AVIF)
>* Ancho de banda de red
>* DPR (proporción de píxeles del dispositivo)
>
>Para aprender lo fácil que es usar Snapshot, juegue el [Vídeo de formación de instantáneas](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 minutos y 17 segundos).


## Prácticas recomendadas para el formato de imágenes (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Los formatos JPG o PNG son las mejores opciones para distribuir imágenes con una buena calidad y con un tamaño y peso manejables.
* Si no se proporciona ningún comando de formato en la dirección URL, el servicio de imágenes de Dynamic Media toma el valor predeterminado de JPG para la entrega.
* JPG comprime en una proporción de 10:1 y generalmente ofrece tamaños de archivo de imagen más pequeños. PNG comprime a una proporción de aproximadamente 2:1, excepto a veces cuando las imágenes contienen un fondo vacío. Normalmente, los tamaños de archivo PNG son mayores que los archivos JPG.
* JPG utiliza compresión con pérdidas, lo que significa que elementos de la imagen (píxeles) se eliminan durante la compresión. PNG utiliza la compresión sin pérdidas.
* JPG a menudo comprime imágenes fotográficas con una mejor fidelidad que las imágenes sintéticas con contraste y bordes y nítidos.
* Si las imágenes contienen transparencias, utilice PNG porque JPG no admite transparencias.

Como práctica recomendada para el formato de imagen, comience con la configuración más común `&fmt=JPG`.

## Prácticas recomendadas para el tamaño de imagen {#best-practices-for-image-size}

La reducción dinámica del tamaño de la imagen es una de las tareas más comunes que realiza el servicio de imágenes de Dynamic Media. Requiere especificar el tamaño y, opcionalmente, el modo de disminución de resolución que se utiliza para reducir el tamaño de la imagen.

* Para el tamaño de la imagen, el enfoque mejor y más directo es utilizar `&wid=<value>` y `&hei=<value>` o simplemente `&hei=<value>`. Estos parámetros establecen la anchura de la imagen automáticamente según la proporción de aspecto.
* `&resMode=<value>` controla el algoritmo utilizado para la disminución de resolución. Comience por `&resMode=sharp2`. Este valor proporciona la mejor calidad de imagen. Al utilizar el valor de disminución de resolución `=bilin` es más rápido, a menudo resulta en el solapamiento de artefactos.

Como práctica recomendada para el tamaño de imágenes, utilice `&wid=<value>&hei=<value>&resMode=sharp2` o `&hei=<value>&resMode=sharp2`

## Prácticas recomendadas para el enfoque de imágenes {#best-practices-for-image-sharpening}

El enfoque de imágenes es el aspecto más complejo del control de imágenes en su sitio Web y en el que se producen muchos errores. Tómese el tiempo necesario para obtener más información sobre el funcionamiento del enfoque y el enmascaramiento de enfoque en Adobe Dynamic Media Classic consultando los siguientes recursos útiles:

Documentación técnica sobre prácticas recomendadas [Enfoque de imágenes en Adobe Dynamic Media Classic y en el servidor de imágenes](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Con Adobe Dynamic Media Classic, puede enfocar las imágenes durante la ingesta, la entrega o ambas cosas. Sin embargo, normalmente las imágenes se enfocan con un solo método o con el otro, pero no con ambos. Normalmente, el enfoque de imágenes durante la distribución, en una URL, ofrece los mejores resultados.

Existen dos métodos de enfoque de imágenes que puede utilizar:

* Enfoque simple ( `&op_sharpen`): similar al filtro de enfoque utilizado en Photoshop, el enfoque simple aplica un enfoque básico a la vista final de la imagen después del cambio de tamaño dinámico. Sin embargo, este método no puede configurarse. La práctica recomendada es no utilizar `&op_sharpen` a menos que sea necesario.
* Máscara de enfoque ( `&op_USM`) - Máscara de enfoque es un filtro estándar de la industria para el enfoque. La práctica recomendada es enfocar imágenes con la máscara de enfoque siguiendo las directrices siguientes. Las máscaras de enfoque permiten controlar los tres parámetros siguientes:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, intensidad del efecto.)
      * `radius` (0-250, anchura de las &quot;líneas de enfoque&quot; dibujadas alrededor del objeto enfocado, medida en píxeles.)

        Tenga en cuenta que los parámetros de `radius` y `amount` trabajar unos contra otros. Reducción `radius` puede compensarse aumentando el `amount`. `Radius` permite un control más preciso, ya que un valor más bajo enfoca únicamente los píxeles del borde, mientras que un valor más alto enfoca una banda más ancha de píxeles.

      * `threshold` (0-255, sensibilidad del efecto.)

        Este parámetro determina hasta qué punto deben ser distintos los píxeles enfocados respecto al área que los rodea para poder considerarse píxeles de borde y por tanto enfocarse. El umbral ayuda a evitar el exceso de áreas de enfoque con colores similares, como los tonos de piel. Por ejemplo, un valor de umbral 12 ignora las ligeras variaciones de brillo en el tono de la piel para no agregar “ruido” y, simultáneamente, agrega contraste al borde de las áreas contrastadas, por ejemplo, donde las pestañas tocan la piel.

        Para obtener más información sobre cómo configurar estos tres parámetros, incluidas las prácticas recomendadas para su uso con el filtro, consulte [Enfoque de imágenes en Adobe Dynamic Media Classic y en el servidor de imágenes](/help/using/assets/s7_sharpening_images.pdf).

      * Adobe Dynamic Media Classic también permite controlar un cuarto parámetro: monocromo ( `0,1`). Este parámetro determina si se aplica máscara de enfoque a cada componente de color por separado utilizando el valor `0` o a la intensidad/brillo de la imagen con el valor `1`.

La práctica recomendada es comenzar con el parámetro de radio de máscara de enfoque. Puede comenzar con las configuraciones de radio siguientes:

* Sitio web: 0,2-0,3 píxeles
* Impresión fotográfica (250-300 ppp): 0,3-0,5 píxeles
* Impresión en offset (266-300 ppp): 0,7-1,0 píxeles
* Impresión de lienzo (150 ppp): 1,5-2,0 píxeles

Aumente gradualmente la cantidad de 1,75 a 4. Si el enfoque aún no aparece como desea, aumente el radio en un decimal y ejecute de nuevo la cantidad de 1,75 a 4. Repita el proceso tantas veces como sea necesario.

Deje la configuración del parámetro monocromo en 0.

## Prácticas recomendadas para la compresión de JPEG (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Este parámetro controla la calidad de codificación de JPG. Un valor más alto significa una mejor calidad de imagen pero un tamaño mayor de archivo; por lo contrario, un valor inferior significa una imagen de menor calidad pero un tamaño de archivo más pequeño. El rango de este parámetro es 0-100.
* Para optimizar la calidad, no defina el valor del parámetro a 100. La diferencia entre un ajuste de 90 o 95 y 100 es casi imperceptible, pero 100 aumenta innecesariamente el tamaño de archivo de la imagen. Por lo tanto, para optimizar la calidad pero evitar que los archivos de imagen se vuelvan demasiado grandes, establezca el `qlt=` valor 90 o 95.
* Para optimizar para un tamaño de archivo de imagen pequeño pero mantener la calidad de imagen en un nivel aceptable, establezca el `qlt=` valor 80. Los valores por debajo de 70 a 75 degradan considerablemente la calidad de imagen.
* Como práctica recomendada, para permanecer en el medio, configure el `qlt=` valor de 85 para permanecer en el medio.
* Uso del indicador de croma en `qlt=`

   * El `qlt=` El parámetro tiene un segundo ajuste que permite activar la disminución de resolución de cromaticidad del RGB utilizando el valor normal `,0` (predeterminado) o desactívelo con el valor `,1`.
   * Para que sea sencillo, comience con la disminución de resolución de cromaticidad RGB desactivada ( `,1`). Este ajuste normalmente ofrece una mejor calidad de imagen, especialmente en imágenes sintéticas con muchos bordes nítidos y contraste.

Como práctica recomendada para el uso de compresión JPG `&qlt=85,0`.

## Prácticas recomendadas para el tamaño JPEG (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

El parámetro `jpegSize` es útil si desea garantizar que una imagen no supere un tamaño determinado para su entrega a dispositivos con memoria limitada.

* Este parámetro se establece en kilobytes ( `jpegSize=<size_in_kilobytes>`). Define el tamaño máximo permitido para la distribución de imágenes.
* `&jpegSize=` interactúa con el parámetro de compresión del JPG `&qlt=`. Si la respuesta del JPG con el parámetro de compresión del JPG especificado ( `&qlt=`) no supera el `jpegSize` , la imagen se devuelve con `&qlt=` como se define. De lo contrario, `&qlt=` disminuye gradualmente hasta que la imagen se ajusta al tamaño máximo permitido o hasta que el sistema determina que no se ajusta y devuelve un error.

Como práctica recomendada, establezca `&jpegSize=` y añada el parámetro `&qlt=` si ofrece imágenes JPG a dispositivos con memoria limitada.

## Resumen de prácticas recomendadas {#best-practices-summary}

Como práctica recomendada, para lograr una alta calidad de imagen y un tamaño de archivo pequeño, comience con esta combinación de parámetros:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Esta combinación da resultados excelentes en la mayoría de circunstancias.

Si necesita optimizar la imagen aún más, ajuste gradualmente los parámetros de enfoque (la máscara de enfoque) comenzando con un radio definido en 0,2 o 0,3. A continuación, aumente gradualmente la cantidad desde 1,75 a 4 (equivalente al 400% en Photoshop). Compruebe si se ha obtenido el resultado deseado.

Si los resultados de enfoque aún no son satisfactorios, aumente el radio en incrementos decimales. Tras cada incremento decimal, vuelva a ajustar la cantidad en 1,75 y auméntela gradualmente a 4. Repita este proceso hasta lograr el resultado deseado. Aunque los valores anteriores son un método validado por los estudios creativos, recuerde que puede empezar con otros valores y seguir otras estrategias. Si los resultados son satisfactorios o no es una cuestión subjetiva y, por lo tanto, la clave es la experimentación estructurada.

A medida que experimenta, las siguientes sugerencias generales son útiles para optimizar el flujo de trabajo:

* Pruebe diferentes parámetros en tiempo real, ya sea directamente en una dirección URL o utilizando la funcionalidad de ajuste de imagen de Adobe Dynamic Media Classic. Este último proporciona previsualizaciones en tiempo real para operaciones de ajuste.
* Como práctica recomendada, recuerde que puede agrupar comandos del servicio de imágenes de Dynamic Media en un ajuste preestablecido de imagen. Un ajuste preestablecido de imagen son básicamente macros de comandos de URL con nombres de ajustes preestablecidos personalizados como `$thumb_low$` y `&product_high$`. El nombre del ajuste preestablecido personalizado en una ruta URL llama a estos ajustes preestablecidos. Esta funcionalidad le ayudará a administrar comandos y ajustes de calidad para diferentes modelos de uso de imágenes en su sitio web y reducirá la longitud total de la URL.
* Adobe Dynamic Media Classic también proporciona formas más avanzadas de ajustar la calidad de la imagen, como aplicar enfoque de imagen al ingerir. En los casos de uso avanzados en los que una opción es seguir ajustando y optimizando los resultados procesados, Adobe Professional Services puede ayudarle con información personalizada y prácticas recomendadas.
